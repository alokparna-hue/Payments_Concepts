## Introduction

The hallmark of a good payment transaction lies in how **easy and fogettable it is for the customers**. 
A hassle-free offline and online transaction guarantees customer retention and an enhanced experience. 
What looks like a few seconds of some number exchange and buttons tapping, is a mesh of detailed processes and systems that come togther to make every transaction successful. 
This article provides a glimpse into the two major pillars of payments; **Authorization** and **Settlement**.

| **Note** |
---|
| _This article considers credit card transactions only. Debit card or UPI transactions are out of scope._ |

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
| Credit limit/availability
| Card status (active/inactive)
| PIN validation
| Fraud indicators

_**Example of an Authorization**_: Mr. X buys an invisible suit from a sci-fi shop. He inserts his card, types the PIN, the POS terminal shows a transaction successful message, and a slip is generated. All within a few seconds. 
_What has happened_
Sci-fi shop's POS terminal sends the transaction details to its acquirer (for example- HDFC), which transfers the details to network (for example, Visa), which transfers the details to the issuer (for example, YES Bank). YES Bank validates the transaction and retuns a positive response message of "Approved", following the same route but in reverse.

## Settlement

This refers to the stage where actual funds transfer and **_settlement_** takes place among all the parties involved. While authorization mostly involves approving or declining a transaction, settlement involves movement of funds from:

**Issuer > Network > Acquirer/Payment Processor > Merchant**

The merchant's POS terminal **_sends a list of authorized transactions_** to its acquirer/payment processor (either real time or at the end of the day). 
The acquirer/processor validates these and passes this information to the issuer through the card network. The issuer validates these transactions  again and *disburses funds to the merchant through the card network and acquirer/processor. Before the amount is tranferred to the merchant's account, all the parties deduct certain fees (*the major part of it is charged by the issuer), after which the final amount is _settled_ into the merchant account.

| ***Why does the issuer deduct the highest fee**? |
---|
| Settlement usually happens on the same day of the transaction or day or two after the transaction (T+1, T+2). While a part of the customer's credit is blocked, the customer is billed at the end of every month. To fill this gap, the issuer takes the highest risk and transfers the amount to the merchant, before even the customer gets billed. Hence, it deducts the highest fee. |

_**Example of a Settlement**_: YES Bank transfers the transaction amount to the sci-fi shop's account, after deducting a part as fees. 
Visa also charges a fee for securing and faciliating the transaction. Acquirer/payment processor also charges a fee for providing the necessary payment infrastructure.
The final amount is what the merchant gets after every transaction.
