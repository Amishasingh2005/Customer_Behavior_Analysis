Customer Shopping Behavior Analysis

End-to-end data analysis project on 3,900 customer transactions, covering data cleaning in Python, business-question analysis in MySQL, and an interactive dashboard built in Power BI.

📌 Project Overview

This project analyzes customer shopping behavior using transactional data to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior — with the goal of guiding strategic business decisions.

🗂️ Dataset Summary
Rows: 3,900
Columns: 18
Key features:
Customer demographics — Age, Gender, Location, Subscription Status
Purchase details — Item Purchased, Category, Purchase Amount, Season, Size, Color
Shopping behavior — Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type
Missing data: 37 values in the Review Rating column
🛠️ Tools & Tech Stack
Python (pandas) — data cleaning & feature engineering
MySQL — structured business-question analysis
Power BI — interactive dashboard & visualization
🔎 Workflow
1. Data Cleaning & Preparation (Python)
Loaded the dataset with pandas and explored it using df.info() / .describe()
Imputed missing Review Rating values using the median rating per product category
Standardized column names to snake_case
Engineered new features: age_group (binned ages) and purchase_frequency_days
Checked discount_applied vs. promo_code_used for redundancy and dropped promo_code_used
Loaded the cleaned DataFrame into MySQL for SQL-based analysis
2. Business Analysis (MySQL)

Answered 10 key business questions, including:

Revenue by gender
High-spending customers who still used discounts
Top 5 products by average rating
Standard vs. Express shipping — average purchase amount
Subscribers vs. non-subscribers — spend & revenue
Most discount-dependent products
Customer segmentation (New / Returning / Loyal)
Top 3 products per category
Repeat buyers vs. subscription likelihood
Revenue contribution by age group
3. Dashboard (Power BI)

Built an interactive dashboard with filters for Subscription Status, Gender, Category, and Shipping Type, featuring:

Number of customers, average purchase amount, average review rating
% of customers by subscription status
Revenue & sales by category
Revenue & sales by age group
📈 Key Findings
3.9K customers, $59.8 average purchase amount, 3.75 average review rating
Only 27% of customers are subscribers, yet subscribers show comparable average spend to non-subscribers
Clothing leads both revenue and sales by category
Young Adults contribute the highest revenue among age groups
Most customers fall into the Loyal segment (3,116 of 3,900)
💡 Business Recommendations
Boost Subscriptions — promote exclusive benefits for subscribers
Customer Loyalty Programs — reward repeat buyers to move them into the "Loyal" segment
Review Discount Policy — balance sales boosts with margin control
Product Positioning — highlight top-rated and best-selling products in campaigns
Targeted Marketing — focus efforts on high-revenue age groups and express-shipping users
📁 Files
Customer_Shopping_Behavior_Analysis.pdf — full written report
dashboard.png — Power BI dashboard screenshot
README.md — this file
✍️ Author

Prepared as an independent data analysis project covering the full pipeline: data cleaning (Python) → business analysis (MySQL) → visualization (Power BI).
