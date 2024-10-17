Three Datasets were collected for this capstone project. Each dataset indicate whether a transaction was fraud or not as well the other details that may help predict whether it was fraud or not. This document will describe each in detail. 

Dataset 1 

Dataset origin: https://www.openml.org/search?type=data&status=active&id=45955&sort=runs 

Dataset Name: card_transdata.csv

Description: This dataset captures transaction patterns and behaviors that could indicate potential fraud in card transactions. The data is composed of several features designed to reflect the transactional context such as geographical location, transaction medium, and spending behavior relative to the user's history.

#Attribute Description:

distance_from_home: This is a numerical feature representing the geographical distance in kilometers between the transaction location and the cardholder's home address.
distance_from_last_transaction: This numerical attribute measures the distance in kilometers from the location of the last transaction to the current transaction location.
ratio_to_median_purchase_price: A numeric ratio that compares the transaction's price to the median purchase price of the user's transaction history.
repeat_retailer: A binary attribute where '1' signifies that the transaction was conducted at a retailer previously used by the cardholder, and '0' indicates a new retailer.
used_chip: This binary feature indicates whether the transaction was made using a chip (1) or not (0).
used_pin_number: Another binary feature, where '1' signifies the use of a PIN number for the transaction, and '0' shows no PIN number was used.
online_order: This attribute identifies whether the purchase was made online ('1') or offline ('0').
fraud: A binary target variable indicating whether the transaction was fraudulent ('1') or not ('0').

Use Case: This dataset is particularly suited for developing machine learning models to detect potentially fraudulent transactions. 

Dataset shape: dataset has 1,000,000 rows and 8 columns. 

Dataset 2

Dataset Origin: https://www.kaggle.com/datasets/chitwanmanchanda/fraudulent-transactions-data 
Dataset Name: Fraud.csv
Discriptions: Data containing fraudulent transactions for a financial company

Attribute Description: 

step - maps a unit of time in the real world. In this case 1 step is 1 hour of time. Total steps 744 (30 days simulation).
type - CASH-IN, CASH-OUT, DEBIT, PAYMENT and TRANSFER.
amount - amount of the transaction in local currency.
nameOrig - customer who started the transaction
oldbalanceOrg - initial balance before the transaction
newbalanceOrig - new balance after the transaction
nameDest - customer who is the recipient of the transaction
oldbalanceDest - initial balance recipient before the transaction. Note that there is not information for customers that start with M (Merchants).
newbalanceDest - new balance recipient after the transaction. Note that there is not information for customers that start with M (Merchants).
isFraud - This is the transactions made by the fraudulent agents. 
isFlaggedFraud - The business model aims to control massive transfers from one account to another and flags illegal attempts. 

Use Case: In this specific dataset the fraudulent behavior of the agents aims to profit by taking control of customers accounts and try to empty the funds by transferring to another account and then cashing out of the system. An illegal attempt in this dataset is an attempt to transfer more than 200.000 in a single transaction.

Dataset shape: Dataset has 6,362,620 rows and 11 columns. 

Dataset 3

Dataset origin: https://www.kaggle.com/datasets/neharoychoudhury/credit-card-fraud-data/data?select=fraud_data.csv
Dataset Name: fraud_data.csv

Description: This dataset consists of credit card transactions in the western United States. 
It includes information about each transaction including customer details, the merchant and category of purchase, and whether or not the transaction was a fraud.

Attribute Description:

trans_date_trans_time  Transaction DateTime 
merchant               Merchant Name 
category               Category of Merchant 
amt                    Amount of Transaction
city                   City of Credit Card Holder 
state                  State of Credit Card Holder 
lat                    Latitude Location of Purchase 
long                   Longitude Location of Purchase 
city_pop               Credit Card Holder's City Population   
job                    Job of Credit Card Holder
dob                    Date of Birth of Credit Card Holder 
trans_num              Transaction Number 
merch_lat              Latitude Location of Merchant 
merch_long             Longitude location of Merchant 
is_fraud               Binary result of Fraud or not 


Use Case: The dataset can be used to identity fraudulent transaction and categorise them base on location. It can also be used to detect and predict future occurences of fraud 

Dataset shape: Dataset has 14,446 rows and 15 columns.
