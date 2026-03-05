🛍️ Customer Shopping Behavior Analysis








📌 Project Overview

Understanding customer behavior is critical for improving sales strategies, marketing campaigns, and customer retention.

This project analyzes 3,900 customer shopping transactions to uncover insights into:

Customer spending patterns

Product popularity

Discount usage behavior

Subscription trends

Customer segmentation

The project uses a complete data analytics workflow:

Python → Data Cleaning & EDA
SQL → Business Analysis
Power BI → Interactive Dashboard

📊 Dataset Summary
Feature Type	Columns
Customer Demographics	Age, Gender, Location, Subscription Status
Purchase Details	Item Purchased, Category, Purchase Amount, Season
Product Attributes	Size, Color
Shopping Behavior	Discount Applied, Promo Code Used
Customer Activity	Previous Purchases, Frequency of Purchases
Feedback	Review Rating
Logistics	Shipping Type

Dataset Size

Rows: 3,900

Columns: 18

Missing Values: 37 (Review Rating)

🔎 Data Cleaning & EDA (Python)

Performed using Pandas and Python.

Key Steps

✔ Data loading and inspection
✔ Missing value treatment
✔ Feature engineering
✔ Column name standardization
✔ Data validation and consistency checks

Feature Engineering

New columns created:

age_group

purchase_frequency_days

Example:

df['age_group'] = pd.cut(df['age'], bins=[18,25,35,50,70],
                         labels=['Young','Adult','Middle Age','Senior'])
Missing Value Handling

Missing review ratings were filled using:

Median rating per product category

🗄️ SQL Business Analysis

Data was loaded into PostgreSQL to perform analytical queries.

Business Questions Answered

1️⃣ Revenue contribution by Gender

2️⃣ Customers who used discounts but still spent above average

3️⃣ Top 5 highest rated products

4️⃣ Shipping type comparison

Standard vs Express

5️⃣ Subscribers vs Non-Subscribers

Average spending

Total revenue

6️⃣ Discount-dependent products

7️⃣ Customer segmentation

Segment	Definition
New	Few purchases
Returning	Moderate purchase history
Loyal	High purchase frequency

8️⃣ Top 3 products in each category

9️⃣ Relationship between repeat buyers and subscription

🔟 Revenue by age group

📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize insights.

Dashboard Insights

📈 Revenue by Gender
📈 Revenue by Age Group
📈 Category Performance
📈 Customer Segmentation
📈 Subscription Analysis
📈 Shipping Type Comparison

Example visuals:

Bar charts

KPI cards

Category analysis

Customer segmentation charts

(Add dashboard screenshot here in your GitHub repo)

💡 Business Recommendations
🎯 Boost Subscriptions

Offer exclusive deals and benefits for subscribers.

🎯 Improve Customer Loyalty

Implement reward programs for repeat buyers.

🎯 Optimize Discount Strategy

Avoid over-discounting to protect margins.

🎯 Promote Top Products

Focus marketing campaigns on high-rated and popular products.

🎯 Target High Value Segments

Invest in marketing for high spending age groups.

🛠️ Tech Stack
Tool	Purpose
Python	Data cleaning & analysis
Pandas	Data manipulation
PostgreSQL	Business analysis queries
SQL	Data analysis
Power BI	Dashboard & visualization

📁 Project Structure
Customer-Shopping-Behavior-Analysis
│
├── dataset
│   └── shopping_data.csv
│
├── python
│   └── data_cleaning_eda.ipynb
│
├── sql
│   └── business_queries.sql
│
├── powerbi
│   └── shopping_dashboard.pbix
│
├── report
│   └── project_report.pdf
│
└── README.md

📈 Project Outcome

This project demonstrates how data analytics can transform raw customer transaction data into meaningful business insights.

Companies can use these insights to:

Increase revenue

Improve customer targeting

Build stronger loyalty programs

Optimize product marketing
