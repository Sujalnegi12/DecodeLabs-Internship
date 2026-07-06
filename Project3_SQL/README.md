Project 3 – SQL Data Analysis

Overview

This project focuses on analyzing an e-commerce dataset using SQL in PostgreSQL. The objective was to practice writing SQL queries to retrieve, filter, sort, group, and summarize data in order to generate meaningful business insights.

Dataset

- Table Name: "orders"
- Total Records: 1,200
- Dataset: E-commerce order data (same dataset used in the Data Cleaning project)

The dataset contains information such as order details, customer IDs, products, quantities, prices, payment methods, shipping details, referral sources, coupon codes, and order status.

Tools Used

- PostgreSQL 18
- pgAdmin 4

Database Setup

To prepare the dataset for analysis, I:

- Created a new database in PostgreSQL.
- Created the "orders" table with appropriate data types.
- Imported the CSV file using pgAdmin's Import/Export feature.
- Converted the original text-based order date into a proper "DATE" column using "TO_DATE()" for easier date operations.

SQL Concepts Practiced

During this project, I worked with:

- "SELECT"
- "WHERE"
- "ORDER BY"
- "GROUP BY"
- Aggregate Functions ("COUNT", "SUM", "AVG")
- "HAVING"
- "ROUND()"
- Subqueries

Queries Performed

The SQL script includes queries for:

- Selecting required columns
- Filtering orders by status
- Finding high-value orders
- Filtering data by referral source
- Sorting orders by total price
- Calculating revenue for each product
- Counting orders by status
- Finding average order value by payment method
- Identifying high-revenue products using "HAVING"
- Calculating delivered-order revenue by product
- Finding referral source contribution in percentage
- Analyzing coupon usage and its revenue impact

Key Learnings

This project helped me understand:

- How SQL retrieves and analyzes data from relational databases.
- The difference between "WHERE" and "HAVING".
- How aggregate functions work with "GROUP BY".
- Why SQL follows a logical execution order ("FROM → WHERE → GROUP BY → HAVING → SELECT → ORDER BY").
- How subqueries can be used for percentage calculations.
- The importance of choosing correct data types for efficient analysis.

Project Files

- [Project3_SQL_Analysis_SujalSinghNegi.sql](./Project3_SQL_Analysis_SujalSinghNegi.sql) – Complete SQL script with all queries and comments.
- README.md – Project documentation.

Author
Sujal Singh Negi
