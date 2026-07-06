# 📊 Project 3 – SQL Data Analysis

## 🚀 Overview

This project focuses on analyzing an **e-commerce dataset** using **SQL in PostgreSQL**.
The main objective was to practice writing SQL queries to **retrieve, filter, sort, group, and summarize data** in order to generate meaningful business insights.

---

## 📁 Dataset

* **Table Name:** `orders`
* **Total Records:** 1,200
* **Type:** E-commerce order data

The dataset includes:

* Order details
* Customer IDs
* Product information
* Quantity & pricing
* Payment methods
* Shipping details
* Referral sources
* Coupon codes
* Order status

---

## 🛠️ Tools Used

* 🐘 PostgreSQL 18
* 📊 pgAdmin 4

---

## ⚙️ Database Setup

To prepare the dataset for analysis:

* Created a new database in PostgreSQL
* Designed the `orders` table with appropriate data types
* Imported the CSV file using pgAdmin
* Converted text-based order date into proper `DATE` format using `TO_DATE()`

---

## 🧠 SQL Concepts Practiced

* `SELECT`
* `WHERE`
* `ORDER BY`
* `GROUP BY`
* Aggregate Functions (`COUNT`, `SUM`, `AVG`)
* `HAVING`
* `ROUND()`
* Subqueries

---

## 🔍 Queries Performed

* Selecting specific columns
* Filtering orders by status
* Identifying high-value orders
* Filtering based on referral sources
* Sorting orders by total price
* Calculating revenue per product
* Counting orders by status
* Finding average order value by payment method
* Identifying high-revenue products using `HAVING`
* Calculating delivered-order revenue
* Referral contribution analysis (%)
* Coupon usage & revenue impact

---

## 📈 Key Learnings

* Understanding how SQL extracts insights from relational data
* Difference between `WHERE` and `HAVING`
* Working with aggregate functions and grouping
* SQL execution order:

  ```
  FROM → WHERE → GROUP BY → HAVING → SELECT → ORDER BY
  ```
* Using subqueries for advanced calculations
* Importance of correct data types for performance

---

## 📂 Project Files

* 📄 [SQL Script](./Project3_SQL_Analysis_SujalSinghNegi.sql)

---

## 👨‍💻 Author

**Sujal Singh Negi**


---
