Customer Shopping Behavior Analysis
1. Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.

2. Dataset Summary

Rows: 3,900

Columns: 18

Key Features:

Customer demographics: Age, Gender, Location, Subscription Status

Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Shopping behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

Missing Data: 37 values in the Review Rating column

3. Exploratory Data Analysis (Python)

Performed data preparation and cleaning using Python (pandas):

Data Loading: Imported the dataset using pandas.

Initial Exploration: Used df.info() for structure and df.describe() for summary statistics.

Missing Data Handling: Imputed missing values in Review Rating using the median rating per product category.

Column Standardization: Renamed columns to snake_case for readability.

Feature Engineering:

Created age_group by binning customer ages.

Created purchase_frequency_days from purchase timestamps.

Data Consistency Check: Verified redundancy between discount_applied and promo_code_used; dropped promo_code_used.

Database Integration: Loaded the cleaned DataFrame into PostgreSQL for SQL analysis.

4. Data Analysis (SQL)

Structured SQL queries were used to answer business questions:

Revenue by Gender – Total revenue by male vs. female customers

High-Spending Discount Users – Customers who used discounts but spent above average

Top 5 Products by Rating – Products with highest average review ratings

Shipping Type Comparison – Avg. purchase amount for Standard vs. Express shipping

Subscribers vs. Non-Subscribers – Average spend and total revenue by subscription status

Discount-Dependent Products – Top 5 products with highest % of discounted purchases

Customer Segmentation – Classified as New, Returning, Loyal

Top 3 Products per Category – Most purchased products within each category

Repeat Buyers & Subscriptions – Whether customers with >5 purchases are more likely to subscribe

Revenue by Age Group – Total revenue contribution by each age group

5. Dashboard (Power BI)

Created an interactive dashboard in Power BI to present insights visually.

The dashboard includes key metrics like revenue, customer segmentation, top products, and purchase patterns.

Designed to support data-driven business decisions and make insights accessible for stakeholders.

6. Business Recommendations

Based on the analysis, the following recommendations were made:

Boost Subscriptions: Promote exclusive benefits for subscribers.

Customer Loyalty Programs: Reward repeat buyers to move them into the “Loyal” segment.

Review Discount Policy: Balance sales boosts with margin control.

Product Positioning: Highlight top-rated and best-selling products in campaigns.

Targeted Marketing: Focus efforts on high-revenue age groups and express-shipping users.

7. Technologies Used

Python: pandas, NumPy

SQL: PostgreSQL

Data Visualization: Power BI

Version Control: Git & GitHub
