# Zepto SQL Data Analysis Project

## Project Overview
This project focuses on analyzing Zepto grocery data using SQL.  
The dataset was collected from Kaggle and cleaned using MySQL Workbench.  
After cleaning the data, multiple business-related questions were solved using SQL queries to extract meaningful insights.

---

## Dataset Source
- Kaggle Zepto Grocery Dataset

---

## Tools & Technologies Used
- MySQL
- MySQL Workbench
- SQL
- Kaggle Dataset
- Data Cleaning
- Data Analysis

---

## Data Cleaning Process
The dataset contained inconsistent values and required cleaning before analysis.

Tasks performed:
- Removed duplicate records
- Handled NULL values
- Converted TRUE/FALSE values into 1/0
- Corrected column datatypes
- Standardized column names
- Checked missing values

---

## Business Questions Solved

Some important SQL queries used in this project:

1. Top expensive products
2. Average MRP by category
3. Products with highest discounts
4. Out of stock product analysis
5. Category-wise product count
6. Discount percentage analysis
7. Quantity and availability analysis

---

## Example SQL Query

```sql
SELECT category, AVG(mrp) AS average_price
FROM zepto
GROUP BY category
ORDER BY average_price DESC;
