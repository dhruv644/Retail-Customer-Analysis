# 🛒 Retail Customer Analysis — Case Study

A data analysis project that explores customer behaviour, purchase patterns, and store performance for a retail chain using Python and pandas.

---

## 📁 Project Structure

```
retail-customer-analysis/
│
├── Retail.ipynb                        # Main analysis notebook
├── README.md
│
└── Case Study 1 - Retail Case Study/
    ├── Customer.csv                    # Customer demographics
    ├── Transactions.csv                # Transaction records
    └── prod_cat_info.csv               # Product category hierarchy
```

---

## 📊 Dataset Overview

| File | Description | Key Columns |
|---|---|---|
| `Customer.csv` | Customer demographics | `customer_Id`, `DOB`, `Gender`, `city_code` |
| `Transactions.csv` | Purchase/return records | `transaction_id`, `customer_Id`, `Store_type`, `total_amt`, `tran_date` |
| `prod_cat_info.csv` | Product hierarchy | `prod_cat_code`, `prod_cat`, `prod_sub_cat_code`, `prod_subcat` |

- **Customers:** 5,647 records
- **Product Categories:** Clothing, Footwear, Electronics, Books, and more
- **Store Types:** e-Shop, Flagship Store, MBR, TeleShop

---

## 🔍 Analysis Performed

### 1. Data Merging
- Merged `Customer`, `Transactions`, and `Product Hierarchy` into a single `Customer_Final` dataframe using appropriate joins (keeping all customers with transactions).

### 2. Summary Report
- Column names and data types
- Top/Bottom 10 observations
- Five-number summary for continuous variables
- Frequency tables for all categorical variables

### 3. Visualizations
- Histograms for all continuous variables
- Frequency bar charts for all categorical variables

### 4. Transaction Insights
- Time period covered by transaction data
- Count of transactions with negative total amounts (returns)

### 5. Business Questions Answered

| # | Question | Answer |
|---|---|---|
| 5 | Popular product categories by gender | Electronics & Footwear (Male) / Clothing & Books (Female) |
| 6 | City code with max customers | City Code 3 |
| 7 | Store type with max sales by value & quantity | **e-Shop** — ₹19,824,816 / 9,311 transactions |
| 8 | Electronics + Clothing revenue from Flagship Stores | **₹3,409,559.27** |
| 9 | Electronics revenue from Male customers | **₹5,703,109.43** |
| 10 | Customers with >10 unique positive transactions | Identified with total spend **₹920,785.45** |
| 11a | Electronics + Books spend (age 25–35) | **₹11,297,943.22** |
| 11b | Spend by age 25–35 customers (Jan–Mar 2014) | **₹679,345.16** |

---

## 🛠️ Tech Stack

- **Python 3.12**
- **pandas** — data manipulation and merging
- **numpy** — numerical operations
- **matplotlib** — visualizations
- **seaborn** — statistical plots
- **datetime** — date parsing and age calculation
