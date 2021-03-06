## Payment Gateways for Dummies

Payment gateways are integral to all online transactions. They are the channels through which virtual payments are fulfilled. The process of making an online payment consists of many steps having different components and contributors.
 
This article will serve as a guide to understanding a payment gateway, the services they offer, how it works and the parties to it.


## What is Payment Gateway?

It’s an online payments service that acts like an entrance or a channel. It’s usually integrated with an e-commerce platform. It can be used for both – receiving and making payments. It has a two-way traffic going through it.

The customer who uses an e-commerce website for purchases has to fill his details. These include – debit/credit card number, expiry date and the CVV number at the back of the card. By entering this data, the customer gives consent for the payment, implicitly.


## What is a payment service provider?
 
A payment service provider (PSP) is the one who stands between the customer and the seller. A merchant may have his bank account in one bank and the seller may have it in a different one. It would be difficult for such transactions to be fulfilled if they had to deal with the banks directly.
 
This is where a payment service provider comes in. It can connect multiple acquiring banks, financial institutions, payment networks and processors. All the integration between them is automatically handled by the PSP. This becomes very helpful in international transactions.
 

## What is a merchant account?

A merchant account is a bank account that holds the funds from online or card transactions. This is not the business bank account.

To open a merchant bank account, a seller can approach a payment gateway, payment processors, payment service provider; any acquiring banks etc. They can also get it from Independent Sales Organisations and High street banks etc

A merchant identification number is issued to a seller after the application. It’s known as MID which is also an account number for the merchant account. This is the holding account for the seller’s funds from card/online payments.  

Merchant accounts play a vital role in maintaining the chain of approval. It’s a long process because there’s a delay between the customer paying money and receiving the product.

The products can be returned due to any reason. In such cases, this money would have to be refunded to the customer. This is handled automatically by the acquiring bank by deducting money from the merchant account. Most businesses face the risk of returns depending upon the risk in transactions and the nature of your business.

A seller may have multiple sources of income – from card payments, online transactions, wallet payments etc. A merchant account simplifies this. The payment gateway collects all the payments in a merchant account. It transfers the money into the business bank account only on the date of settlement. All the payments are combined into one single deposit. This makes reconciliation easy for the business.

Payment reconciliation is carried out by checking bank statements against accounting records and the payment gateway, PSP, ISO or acquiring bank’s records to confirm that the payment amounts are correct.
 
## What is the difference between a payment gateway and a merchant account?

A payment gateway is a channel or a pathway for the transaction to occur. It’s the link between the customer’s account and the merchant account. This connection enables the free flow of money between the two bank accounts in a transaction.

As a seller, you cannot do an online transaction without a merchant account. This is not similar to a business bank account. It’s a holding account where funds are held till the verification is completed. The seller has little control over this account.

You can get a merchant account opened by your bank, a payment gateway or processor or by any other financial institution. Some payment gateways may not be doing payment processing. It’s preferable to opt for a service that combines both these functions. This brings us to the next question.


## What is the difference between a payment gateway and a payment processor/payment service provider?

The functions of a payment processor and a payment gateway may look alike. They are the channels or intermediaries to fulfil transactions between a merchant account and a customer account.
But they’re not the same. Here’s the difference:

- A payment gateway is helpful for e-commerce transactions. It’s also necessary for transactions like telephone purchases, digital wallet transactions, card on file payments etc. The point here is that it’s used for transactions which are CNP (Card Not Present).
- A payment gateway can honour a transaction without the need of a physical card.
- A payment processor, on the other hand, needs a physical card to fulfil a transaction. It’s necessary to have it in cases where a PoS (Point of Sales) machine is used. Card–swiping transactions can be honoured only if there’s a payment processor.
- There are four parties in this transaction – a customer, his issuing bank, the merchant’s account and the acquiring bank.


## What is the difference between an e-commerce platform and a payment gateway?

An e-commerce platform is an end to end software solution. It can be a website or a mobile application. Online shops and stores need an e-commerce platform to sell their goods or services.
 
An e-commerce store offers – User interface, Store management system, Security, Data consolidation, Support and Payment processing. Some examples of e-commerce platforms are Shopify, BigCommerce, WooCommerce, Wix Stores etc.
 
A payment gateway is a channel between the customer’s account and the merchant account. Today, most e-commerce platforms have built-in payment processors, like Shopify Payments is Shopify’s. There are other options like Stripe, Amazon Pay and PayPal too, which can be integrated with Shopify. These are 3rd party Payment Gateways.


## How does a payment gateway work?

A payment gateway provides the link for online transactions for money to flow. Now, this is how the payment gateway works to honour the transaction.

1.    The customer visits the eCommerce website or mobile app and selects a product. After filling in the details, they proceed to checkout and complete the transaction. There are a few options on how it can be done from here.

### A hosted payment page
This is a payment page where the customer will be redirected to, after checking out. They have to enter their card details on this page and complete the transaction over the payment gateway.
Here, the e-commerce platform does not store any payment data. There’s little need for complying with Payment Card Industry (PCI) standards in this case.

### A server to server integration
Here, there are two servers – a merchant’s server and a payment gateway’s server. This is used in cases where the merchant stores payment data before sending it for processing.
This provides a faster fulfilment, better interface and a controlled environment for the customer to enter his payment details. They are redirected to the payment gateway only after entering the payment data. There’s a need to strictly comply with PCI standards here.

### Encryption at source
This is similar to the server to server integration. But, here there’s a slight difference in how the payment data is stored by the merchant. It permits the merchant to accept payments through the e-commerce platform while encrypting sensitive card data.
This is done by the payment gateway’s encryption library at the browser level. The PCI compliance in this case is much simple than the one before.

2.    The next step for the customer would be to initiate the transaction. They have to enter their debit or credit card details in the columns on the payments page. This page asks the cardholder’s name, the card number, its expiration date and CSC (Card Security Code) or CVV number (Card Verification Value).

3.    This data is passed through secure channels onto the payment gateway. This depends on the type of integration in the first step (a hosted payment page, a server to server integration or encryption at source).

3.    The payment gateway encrypts the card details which were entered during checkout. It performs numerous checks to ensure and confirm the authenticity before sending the card data to the acquiring bank.

4.    The acquiring bank verifies this data and redirects the customer to the card schemes (Some examples of card schemes are Visa, American Express, and MasterCard etc).

5.    The card schemes receive this data and then perform a verification before sending the payment data to the issuing bank. This is the bank where the customer has his account.

6.    The issuing bank scrutinises this payment data and approves the transaction if all the details match. The approved payment message is sent from the card schemes to the acquiring bank. If it fails due to any reason, a decline message is sent.

7.    The acquiring bank sends the approval or decline message back to the payment gateway. If the payment was approved, the acquirer collects the payment amount from the issuing bank. This money is then held in the merchant account. If it was a decline message, the transaction failure error message would be displayed to the customer. Sometimes, they would be given another option to retry the transaction.

8.    The merchant account now has the money deposited in it. It does not go to the business bank account immediately. This is to safeguard the customer in case he has some issues with the product and would need a refund.

9.    The process of the business receiving its money in the bank account depends on the settlement agreement. This process is called settlement and it’s an agreement between the seller and the payment gateway. The money from different transactions is deposited into the business account a single time, depending on the agreement. In short, if there were 5 customers who bought something from the website in a month, the payment gateway would deposit it as only 1 lump sum amount, in the business bank account.

The payment gateway acts as a safeguard for a customer and makes the reconciliation for a seller easier. This whole process takes place in less than 4 – 5 seconds.


## What is a card scheme?
A card scheme is a payment network. This network consists of payment cards like debit and credit cards. The financial institutions become members of these networks to issue cards.
 
There are mainly 2 card schemes – open and closed.
 
The open card scheme has 3 parties – Cardholder, Merchant and Franchisee. A franchisee acts as an issuing bank and an acquiring bank. Diner’s club, American Express and Discover Card follow this model.
 
The closed scheme has 4 parties – cardholder, Issuer Bank, Merchant account and acquiring bank. Visa, MasterCard, UnionPay and RuPay follow this model.
 
## Payment gateway costs

Typical costs associated with payment gateways:

1. 	One time Set-up Fee: £0 - £30
This is a onetime fee during set-up of the payment gateway
2. 	Monthly Fee: £20 - £250
Recurring monthly fee
3. 	Transaction Flat Fee: 1.4% + 10p to 3.4% + 20p
It’s calculated per transaction and can vary depending on the volume of sales
4. 	PCI Annual Management Fee: Approx £30
Paid for storing data to comply with the PCI
5. 	Transaction Rate: 0.75% to 3%  
Charged by the merchant account provider


## How to choose a payment gateway provider?

Choosing a payment gateway or a payment service provider is a tough decision. It boils down to the needs of the business, its budgeting, margins and risk of returns. The following are some generic points to consider before opting for one.

1. When do you want to start accepting payments?
Having a merchant account is mandatory for many Payment gateway/Service providers. It may take 3 weeks to a month for all the procedures to be completed and get a merchant ID allotted.
But, some payment service providers like Strip and PayPal allow you to accept payments without a merchant account. That’s because they come with a built-in feature which works like a merchant account.

2. How much can you want to spend on a payment gateway?
The price of the service is important for a business. That’s because if the cost on a payment service exceeds the margins, it would affect its price. There are a lot of costs associated with online transactions, like:

·       Set-up costs
·       Transaction costs
·       Maintenance fees
·       Administration costs
·       Conversion Fees etc
 
Then there are some penalty fees for chargebacks. All of these can make it an expensive affair. A small business must consider direct debit as an alternative because it’s cheaper than this.
Popular Payment Gateway and Service Providers.

In a previous section, the difference between a PSP and a Payment Gateway was explained. In the real world, there are mostly pure payment gateways or payment service providers.  PSPs also perform the role of a payment gateway.
 
This is a list of popular payment gateways. They provide services only for online or non-card present transactions.
 
### Braintree
Braintree provides mobile and web payments for ecommerce stores. It provides merchant accounts for each individual seller.
 
### Authorize.net
It allows sellers to accept digital payments in their merchant accounts. It also allows them to accept electronic checks. It’s a subsidiary of Visa.

### Windcave (PaymentExpress)
Windcave is a PCI compliant payment gateway service. It’s an international service which accepts payments from debit and credit cards.

### TrustCommerce
TrustCommerce is known for its omni channel solutions. It lets users accept payments from cards, wallets and much more.
 
This is a list of popular payment service providers. They work in both cases – non card present transactions and the ones which need a card swipe.
 
### Stripe
Stripe was built exclusively for internet businesses. It’s a referred payments processor by many big brands. It lets you accept payments without a merchant account.

### PayPal
PayPal is a popular brand among most new players in the internet business. It’s the most convenient option for them as it lets them accept payments without a merchant account.

### Adyen
Adyen is known for its terminals. They are centralized with one platform for mobile, web and physical transactions. This acts as a crime deterrent.

### Sage Pay
Sage Pay is commonly used in Europe. It’s known for its security features.

### Venmo
It’s owned by PayPal and offers a social network as well. It’s a peer to peer digital service.


## What to Look For In a Payment Gateway:

These are the factors you need to look for in a Payment gateway, before choosing them. This is a purely technical aspect of looking at it.

## Uptime and Reliability
Ecommerce stores work round the clock. So, if the payment gateway fails, it is equivalent to the shop staying closed.

## Real-Time Status check
Some payment gateways and service providers offer real-time status of the business. This may not be part of all the packages. But, it becomes useful when the sellers want to analyse and solve problems in business.

## Accepting Multiple Payment Options and Currencies
Ecommerce stores see visitors from different countries having different payment gateway or service providers. So, this becomes essential to have this available.

## Integration
This is the flexibility of a payment gateway that permits integration to the e-commerce platform. Some websites have an e-commerce platform, a content management system and a shopping card together. This is where integration becomes pivotal.

## Fraud Detection
Payment gateways offer fraud detection too. No merchant would want a customer who buys something to use and return it. This happens in the case of informational products like books, movies etc.
At the same time, they would not want to drive away legitimate buyers. Payment gateways reject payments from such blacklisted customers by recognizing their cards.

## PCI DSS Compliance Level
They stand for Payment Card Industry Data Security Standard. These are standards that have to be followed to keep customer data safe. Loss of such data can adversely impact a business. Prefer a payment gateway provider that accepts PCI DSS Level 1 standards.

