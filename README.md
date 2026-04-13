🛒 Retail Customer Analysis — Case Study
A data analysis project that explores customer behaviour, purchase patterns, and store performance for a retail chain using Python and pandas.

📁 Project Structure
retail-customer-analysis/
│
├── Retail.ipynb                        # Main analysis notebook
├── README.md
│
└── Case Study 1 - Retail Case Study/
    ├── Customer.csv                    # Customer demographics
    ├── Transactions.csv                # Transaction records
    └── prod_cat_info.csv               # Product category hierarchy

📊 Dataset Overview
FileDescriptionKey ColumnsCustomer.csvCustomer demographicscustomer_Id, DOB, Gender, city_codeTransactions.csvPurchase/return recordstransaction_id, customer_Id, Store_type, total_amt, tran_dateprod_cat_info.csvProduct hierarchyprod_cat_code, prod_cat, prod_sub_cat_code, prod_subcat

Customers: 5,647 records
Product Categories: Clothing, Footwear, Electronics, Books, and more
Store Types: e-Shop, Flagship Store, MBR, TeleShop


🔍 Analysis Performed
1. Data Merging

Merged Customer, Transactions, and Product Hierarchy into a single Customer_Final dataframe using appropriate joins (keeping all customers with transactions).

2. Summary Report

Column names and data types
Top/Bottom 10 observations
Five-number summary for continuous variables
Frequency tables for all categorical variables

3. Visualizations

Histograms for all continuous variables
Frequency bar charts for all categorical variables

4. Transaction Insights

Time period covered by transaction data
Count of transactions with negative total amounts (returns)

5. Business Questions Answered
#QuestionAnswer5Popular product categories by genderElectronics & Footwear (Male) / Clothing & Books (Female)6City code with max customersCity Code 37Store type with max sales by value & quantitye-Shop — ₹19,824,816 / 9,311 transactions8Electronics + Clothing revenue from Flagship Stores₹3,409,559.279Electronics revenue from Male customers₹5,703,109.4310Customers with >10 unique positive transactionsIdentified with total spend ₹920,785.4511aElectronics + Books spend (age 25–35)₹11,297,943.2211bSpend by age 25–35 customers (Jan–Mar 2014)₹679,345.16

🛠️ Tech Stack

Python 3.12
pandas — data manipulation and merging
numpy — numerical operations
matplotlib — visualizations
seaborn — statistical plots
datetime — date parsing and age calculation
