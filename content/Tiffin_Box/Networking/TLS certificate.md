#basic #networking #https 

A digital ID card for website which proves identity and enable encryption.

>[!info] Real life Example:
>Think of a "Passport" -- it's issued by a trusted authority, has an expiry date, and proves you are who you say you are.

### What is inside certificate??

- **Domain Name** --- which site it belongs to (e.g. `google.com`)
- **Issued by** --- the Certificate Authority (CA) who verified it
- **Valid from** --- expiry date
- **Public key** --- used to start the encrypted connection
- **Digital Signature** --- proves it hasn't been tampered with

### Types of certificates

1. DV *(Domain Validated)*: 
	-  Just proves ownership of the domain
	- Fast and cheap
	- Shows [[Padlock]] in browser
	- Used by most websites

2. OV *(Organization Validated)*
	- Proves the organization behind the domain is real
	- Manual verification process
	- Used by businesses and organizations

3. EV *(Extended Validation)* 
	- Deep verification of company identity
	- Used by banks, payment processors
	- Used to show green bar with company name — browsers removed this in 2019

>[!tip] Good to know
>[Let's Encrypt](https://en.wikipedia.org/wiki/Let%27s_Encrypt) made TLS free and automated — that's why most websites today use HTTPS.
