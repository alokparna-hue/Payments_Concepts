## Introduction

The hallmark of a good payment transaction lies in how **easy and fogettable it is for the customers**. 
A hassle-free offline and online transaction guarantees customer retention and an enhanced experience. 
What looks like a few seconds of some number exchange and buttons tapping, is a mesh of detailed processes and systems that come togther to make every transaction successful. 
This article provides a glimpse into the two major pillars of payments; **Authorization** and **Settlement**.

| **Note** |
---|
| This article considers credit card transactions only. Debit card or UPI transactions are out of scope. |

## Authorization

This refers to the stage where a customer's transaction request is **_authorized_** by the **issuer** bank. A customer can do any of the following:

- **Insert** the card into the merchant's POS terminal and **enter** the PIN manually
- **Tap** the card on the merchant's POS terminal and **return** it to the merchant
  (In this case, _tap-to-pay_ feature ensures the merchant's device reads the card data without any manual entry.)
- **Swipe** the card on the POS terminal (if EMV chip read does not work) and **enter** the PIN manually

The merchant's POS terminal transfers this data to the **issuer** through the **acquirer** and the **card network**. The issuer *verifies the transaction and responds with an **approve** or **decline** 
message, 
which is communicated to the merchant, through the same network and acquirer. This entire process, in a nutshell, constitutes Authorization.

| ***What does the issuer verify?** |
---|
| Account balance
| Account status (active/inactive)
| Card status (active/inactive)
| PIN number
| Cardholder status and so on.

_**Example**_: 
