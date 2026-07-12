## Introduction

The hallmark of a good payment transaction lies in how **easy and fogettable it is for the customers**. 
A hassle-free offline and online transaction guarantees customer retention and an enhanced experience. 
What looks like a few seconds of some number exchange and buttons tapping, is a mesh of detailed processes and systems that come togther to make every transaction successful and hassle-free. 
This article provides a glimpse into the two major pillars of payments; **Authorization** and **Settlement**.

| **Note** |
---|
| _This article considers credit card transactions only. Debit card or UPI transactions are out of scope._ |

## Authorization

This refers to the stage where a customer's transaction request is **_authorized_** by the **issuer** bank. A customer can perform any of the following:

- **Insert** the card into the merchant's POS terminal and **enter** the PIN manually
- **Tap** the card on the merchant's POS terminal and **return** it to the merchant
  (In this case, _tap-to-pay_ feature ensures the merchant's device reads the card data without any manual entry.)
- **Swipe** the card on the POS terminal (if EMV chip read does not work) and **enter** the PIN manually

The merchant's POS terminal transfers this data to the **issuer** through the **acquirer** and the **card network**. The issuer *verifies the transaction and responds with an **approve** or **decline** 
message, 
which is communicated to the merchant, through the same network and acquirer. This entire process, in a nutshell, constitutes Authorization.

| ***What does the issuer verify?** |
---|
| Credit limit/availability
| Card status (active/inactive)
| PIN validation
| Fraud indicators

_**Example of an Authorization**_: Mr. X buys an invisible suit from a sci-fi shop. He inserts his card, types the PIN, the POS terminal shows a transaction successful message, and a slip is generated. All within a few seconds. 
_What has happened_
Sci-fi shop's POS terminal sent the transaction details to its acquirer/processor (for example- XYZ), which validated the details entered, transferred the details to network (for example, Visa), which transferred the details to the issuer (for example, ABC Bank). ABC Bank checked the credibility of the transaction and returned a positive response message of "Approved", following the same route but in reverse.

## Settlement

Settlement refers to the process where funds are actually **transferred** and **settled** in the merchant's account. The funds transfer usually follow the reverse flow of authorization.

**_Issuer > Network > Processor/Acquirer > Merchant_**

| **Note** |
--- |
| The cardholder is **not** charged during settlement (as the cardholder is charged during the monthly billing cycle). Settlement is an **internal process** that ensures the timely transfer of funds amongst all the concerned entities. Each of the participating entity charges a portion of the fund as fee for facilitating the transaction. |
