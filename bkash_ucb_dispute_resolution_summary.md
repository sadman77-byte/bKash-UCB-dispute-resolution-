# Dispute Resolution: Stuck bKash-to-Bank Transfer Escalated to Bangladesh Bank

A real-world case study documenting a failed fund transfer between **bKash** (Mobile Financial Service) and **United Commercial Bank (UCB)**, the resulting customer support runaround, and how escalating the issue to the central regulatory authority (**Bangladesh Bank**) resolved the dispute within hours.

---

## 📌 Context & Overview

Transferring funds between Mobile Financial Services (MFS) and traditional banking channels usually relies on inter-bank API gateways. When an API transaction fails silently or gets stuck mid-process without proper reconciliation, users often face institutional shifting of responsibility. 

This document serves as an informational guide and post-mortem of how regulatory escalation can be used to resolve stuck financial transfers when standard customer service channels fail.

---

## 📅 Key Details & Transaction Data

* **Transaction Type:** bKash to Bank (United Commercial Bank PLC)
* **Initial Transfer Date:** October 28, 2026 (04:36 PM)
* **Transaction Amount:** BDT 15,000.00
* **Original Transaction ID:** `DJS6NW01U0`
* **Complaint Logged (bKash App):** October 28, 2026 (04:56 PM)
* **Unresolved Status Close Date:** November 02, 2026 (03:28 PM)
* **Escalation Date:** November 04, 2026 (10:00 AM)
* **Refund Received Date:** November 04, 2026 (02:59 PM)
* **Refund Transaction ID:** `DK411LEEL5`

---

## 🔍 The Incident Narrative

### 1. The Failure & False Resolution
On October 28, 2026, a transfer of BDT 15,000 was initiated from a bKash wallet to a UCB bank account. The funds were instantly debited from the bKash balance but failed to reflect in the UCB account. 

A formal dispute ticket was logged via the bKash Mobile App. A few days later, bKash closed the complaint status as **"Solved"** with the system remark:
> *"The amount has been transferred successfully to the desired bank account."*

Despite this status, the money had not been credited to the recipient's bank account.

### 2. Institutional Blame Game
* **bKash Customer Service (Live Chat, Call Center, Physical Customer Care):** Insisted the transfer was 100% successful on their end. When presented with official printed bank statements proving non-receipt, support agents refused liability and instructed the customer to deal with UCB.
* **UCB Bank Support:** Maintained that the transaction originated from bKash, labeling it a bKash-end technical issue and directing the customer back to bKash.
* **Procedural Stalling:** During a subsequent visit to the bKash service center, after demanding a deeper investigation, representatives refused to assist further on procedural grounds—citing that the wallet was registered under a relative's NID and requiring their physical presence, effectively ignoring the core technical failure.

---

## ⚡ The Resolution: Regulatory Escalation

Realizing that standard support channels were ineffective, a formal escalation path was taken.

### Step 1: Document Gathering
Collected all concrete digital evidence:
* bKash digital transaction statements & app complaint screenshots
* UCB official account statement confirming zero credit entry
* Transaction IDs (`DJS6NW01U0`) and timestamp logs

### Step 2: Central Regulatory Complaint
An email was sent directly to the **Financial Integrity and Customer Services Department (FICSD)** of **Bangladesh Bank** (the central bank of Bangladesh), placing senior officials from both bKash and UCB Bank in **CC**.

### Step 3: Immediate Impact & Refund
* **Within 30 Minutes:** Representatives from both bKash management and UCB Bank called the customer directly.
* **Inter-Institutional Coordination:** High-priority internal email communications commenced between bKash IT and UCB IT teams to perform manual database reconciliation.
* **Full Reversal:** By 02:59 PM (under 5 hours from the escalation email), the full BDT 15,000 refund was successfully credited to the bank account under Transaction ID `DK411LEEL5`.

---

## 💡 Key Takeaways for Financial Consumers

1. **Keep Evidence:** Always preserve Transaction IDs, digital statements, conversation timestamps, and app screenshots.
2. **Never Accept False Resolution:** If a ticket is marked "Solved" without actual resolution, demand formal audit trails.
3. **Know the Escalation Hierarchy:** When financial institutions refuse accountability or stall, escalate the issue directly to the central banking regulatory body (**Bangladesh Bank FICSD**).

---

## 🛠 Cyber Security & Technical Terminology

* **Stuck / Hanging Transaction:** A state where funds leave the source system (bKash) but fail to complete the handshake with the target API (UCB), leaving funds unallocated.
* **Financial Settlement Failure / Reconciliation Deficit:** A failure in backend automated settlement systems across payment switches (e.g., NPSB or proprietary bank APIs).
* **Regulatory Escalation:** Moving a consumer complaint from frontline operational support to a central regulatory oversight body to enforce compliance and SLA compliance.

---

## 📄 License

This repository and document are licensed under the **MIT License**.

```text
MIT License

Copyright (c) 2026 

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```