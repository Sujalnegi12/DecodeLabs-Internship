# Project 2: Exploratory Data Analysis (EDA)

## Overview
This project focuses on the discovery phase of the data analytics workflow — Exploratory 
Data Analysis (EDA). Building on the cleaned dataset from Project 1, this analysis goes 
beyond simple reporting to uncover hidden patterns, trends, and outliers within the 
e-commerce orders data, transforming raw numbers into actionable business insights.

## Objective
Analyze the cleaned e-commerce orders dataset (1,200 records) to understand distribution 
patterns, identify anomalies, track revenue trends over time, and quantify relationships 
between key variables — all through statistical and visual analysis in Python.

## Methodology
The analysis followed a structured, six-part approach:

1. **Descriptive Statistics** — Computed mean, median, and count for Quantity, UnitPrice, 
   and TotalPrice to establish a statistical baseline of order behavior.
2. **Distribution & Outlier Detection** — Visualized the *Distribution of Total Price* using 
   a histogram overlaid with a KDE density curve, paired with a boxplot to expose outliers 
   at a glance. Followed up with the **IQR method** to mathematically isolate and quantify 
   exactly which orders qualify as statistical outliers.
3. **Monthly Revenue & Order Trend** — Aggregated 2.5 years of data (Jan 2023 – Jun 2025) 
   into a dual-axis chart tracking revenue (bars) against order volume (line) to surface 
   seasonal patterns and peak-performing months.
4. **Category-wise Breakdown** — Built four dedicated visualizations covering *Total Revenue 
   by Product*, *Revenue & Orders by Payment Method*, *Order Status Breakdown*, and *Total 
   Revenue by Referral Source* to pinpoint where performance is concentrated.
5. **Correlation Analysis** — Quantified the Quantity–TotalPrice relationship using Pearson's 
   correlation coefficient, visualized through a regression plot with a fitted trend line.
6. **Synthesis** — Consolidated all findings into a data-backed narrative connecting raw 
   statistics to real business implications.

## Tools & Libraries Used
- **Python** — Pandas (data manipulation), Seaborn & Matplotlib (statistical visualization)
- **Jupyter Notebook** — Interactive development and reporting environment

## Files in This Folder
- [`Project2_EDA_SujalSinghNegi.ipynb`](./Project2_EDA_SujalSinghNegi.ipynb) — Complete analysis notebook with code, visualizations, and commentary
- [`Project2_EDA_SujalSinghNegi.pdf`](./Project2_EDA_SujalSinghNegi.pdf) — Exported report for quick viewing

## Key Findings

| # | Finding | Business Implication |
|---|---------|----------------------|
| 1 | **Right-skewed distribution** — mean order value (₹1,054) exceeds the median (₹824) | A handful of high-value orders inflate the average; the median is the more trustworthy benchmark for "typical" order size |
| 2 | **8 statistical outliers** isolated via the IQR method — every one a high-quantity (5-unit), high-UnitPrice bulk order | Confirmed as genuine purchases rather than data errors, and deliberately retained rather than stripped out |
| 3 | **Peak revenue month: June 2024** (~₹68,068), with January consistently the softest month in both 2024 and 2025 | No dominant seasonal cycle overall, but a recurring January slump signals room for a targeted promotional push |
| 4 | **Chair is the top revenue-generating product** (₹195,620), while **Phone trails last** (₹151,722) | Inventory planning and marketing spend could tilt toward the strongest-performing product lines |
| 5 | **Credit Card leads as the preferred payment method**, and **Online is the most frequent order status** | A fairly even spread across payment and fulfillment channels — no single point of dependency to de-risk |
| 6 | **Quantity and TotalPrice correlate moderately-to-strongly** (r = 0.62), a mathematically expected relationship | Suggests bulk-purchase incentives (tiered discounts, bundle deals) as a viable lever to lift average order value |

## Conclusion
This exploratory analysis converted a clean but static dataset into a clear, evidence-backed 
narrative — mapping *where* revenue concentrates, *when* it peaks, and *how* order size 
drives value. These insights form the analytical foundation for the SQL-based deep-dive 
conducted in Project 3.
---

**Author:** Sujal Singh Negi  
**Program:** Data Analytics Internship — DecodeLabs
