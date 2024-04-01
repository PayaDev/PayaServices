# **WEB Authorization Requirements**

Merchant MUST receive a Customer authorization for internet initiated (WEB) entries prior to processing ACH debit transaction Requirements are below.
Authorization:
- MUST be readily identifiable as an authorization and have clear and readily understandable terms.
- MUST have the following verbiage (or substantially similar) text listed on the authorization page of their website.
- MUST provide the Receiver with the method to revoke the authorization by notifying the Originator in the manner prescribed, within a specified time
frame, even if processing time does not allow for revocation.
“By authorizing this transaction, customer agrees that <merchant name> may convert this transaction into an Electronic Funds Transfer (EFT) via ACH
transaction and to debit this bank account for the amount specified. Additionally, in the event this EFT is returned unpaid, a service fee, as allowable by
law, will be charged to this account via EFT or ACH. In the event you choose to revoke this authorization, please do so by contacting the <merchant name>
directly at <________>. Please note that processing times may not allow for revocation of this authorization.”
The following information must be included in the authorization record:
- Consumer IP Address of Origination
- Consumer Name
- Consumer Address (optional / industry recommended best practice)
- Consumer E-mail address (optional / industry recommended best practice)
- Consumer Banking information (Routing Number and Account Number)
- Transaction Amount
- Transaction Effective Date
- Signifying whether authorization is for a single or recurring/multiple debits, and debit schedule if recurring/multiple
Customer Authentication:
Merchants are required to use commercially reasonable methods to authenticate customer identity prior or during authorization.
- It is not commercially reasonable to have done nothing.
- Assigning password and customer authorizing in the SAME internet session is not commercially reasonable.
Possible methods to authenticate are below:
- Shared secrets
- User ID
- PIN
- Password
- Request identifying customer information to verify against outsourced databases.
- Ask challenge questions to verify against credit bureau or outsourced databases.
- Sending customer a specific piece of information, either online or offline, and then ask customer to verify or provide that information as a second step
in the authentication process.
Fraud Detection System:
Merchants are required to establish and implement a commercially reasonable fraudulent transaction detection system to screen the debit WEB Entry.
Such a fraudulent transaction detection system must, at a minimum have the following:
- Validate the customer bank account number for the first use and
- Validate the customer bank account number for any subsequent change(s) to the account number.
NACHA is neutral to specific methods or technologies to accomplish. It is not commercially reasonable to have done nothing. Suggested methods below:
- ACH Prenotification
- ACH Micro-transaction verification
- Commercially reasonable validation service
Authorization Retention:
Merchants are required to retain the customer’s original authorization or copy of the original authorization in its original form that can be reproduced.
Merchant MUST be able to reproduce and/or provide Processor with a copy of the customer authorization upon request. NACHA does not accept proof of
an authorization as being a listing of the information captured at time of authorization. Industry best practice for reproduction to appear the same as
presented to customer including all authorization verbiage, agreement terms, and revocation method as provided on the website at time of authorization.
The following information must be included in the authorization reproduced record:
- Consumer IP Address of Origination
- Consumer Name
- Consumer Address (optional / industry recommended best practice)
- Consumer E-mail address (optional / industry recommended best practice)
- Consumer Banking information (Routing Number and Account Number)
- Transaction Amount
- Transaction Effective Date
- Signifying whether authorization is for a single or recurring/multiple debits, and debit schedule if recurring/multiple
- Website address where payment was accepted
- Authorization verbiage, applicable terms, and revocation method (as shown to customer during authorization.)
- Statement of how the consumer’s identity was authenticated
Additional information not shown on the website can be included to document proof of authorization.


> [!IMPORTANT]
> The following screenshots are for demonstration purposes only.

Below is an example screen capture at time of consumer authorized transaction via the web.

<p align="center"> **For DEMONSTRATION purposes ONLY.**

<p align="center"> <img src=/Authorization%20Gateway/Assets/Images/Review.jpg width="500" height="500" border="10"/> 


Below is an example reproduction of the data saved at time of consumer authorized transaction via the web.

<p align="center">**For DEMONSTRATION purposes ONLY.**

<p align="center"> <img src=/Authorization%20Gateway/Assets/Images/Receipt.jpg width="500" height="500" border="10"/>

<p align="center"> <img src=/Authorization%20Gateway/Assets/Images/Results.jpg width="300" height="100" border="10"/>
