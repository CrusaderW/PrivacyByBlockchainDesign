#Usecases

A business needs access to personal data. The service will be providing data in an anonymized form if possible.

##Prerequisites
The assumptions of the classification of the personal data (plain/psedonymous/anonymous) is based on the mutual agreement, that the Service stores no data about the user permanenetly.
This means the data is only processed for exactly one specific reason and will be deleted after this process is successfull or fails.

Based on the fact, that the Provider of the Service stores no data about the user, we can assume some data to be completly anonymous.

##1. Age Oracle (most likely anonymous)
An Service needs to know if the user fits a certain age-category.
###example requests:
- <= 18
- \>= 16
- \> 18
- \> 21
- \>= 60

##2. Address (Not anonymous)
An Service needs the Adress of a user
###example request:
- request following fields:
	- First Name
	- Last Name
	- Street
	- House Number
	- PLZ
	- City
	- Country

**(Find standards for address-object)**

##3. E-Mailaddress (most likely anonymous)
An Service needs the E-Mailaddress of a user
###example request:
- e-mailadress

##4. Phone number (most likely anonymous)
An Service needs the Phone Number of a user
###example request:
- Phone number

##5. Current Location (most likely anonymous)
An Service requests the current location of the user.
###example request:
- request following fields:
	- Latitude
	- Logitude

##6. Driver License Details (most likely anonymous)
An Service requests some drivers license details of the user.
###example request:
- request following fields:
	- Date Issued
	- valid until
	- Classes
	- Issuing Authority
	- ...

##7. Credit Card Details (most likely not anonymous)
An Service requests credit card details of the user.
###example request:
- request following fields:
	- Full Name (could be anonymous if possible without the name)
	- valid until
	- Credit card Number
	- CSV

##n. find more relevant usecases