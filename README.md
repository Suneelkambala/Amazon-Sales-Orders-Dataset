# Amazon.in Sales Orders Dataset – README
## 📌 Project Description

This project analyzes real-world e-commerce sales data from Amazon.in to derive insights into sales trends, product demand, fulfillment efficiency, and geographic distribution. It demonstrates data cleaning, exploratory data analysis (EDA), visualization, and actionable business insights, suitable for showcasing in a GitHub portfolio.

## 🎯 Project Objectives

Clean and preprocess raw e-commerce sales data for analysis

Analyze order status trends (Shipped, Delivered, Cancelled)

Identify top-selling product categories and sizes

Evaluate fulfilment methods (Amazon vs Merchant) and delivery efficiency

Perform geographic analysis of orders by city and state

Analyze revenue distribution and average order value

Derive business recommendations to optimize inventory, logistics, and revenue

## 📌 Overview

This dataset contains detailed sales order information from an e-commerce platform (Amazon.in). It includes order details, fulfillment status, product attributes, shipping information, and payment-related data. The dataset is useful for sales analysis, order tracking, customer behavior analysis, and logistics insights.

## 📂 Dataset Structure

Each row represents one order.

# 🔍 Exploratory Data Analysis (EDA) – Key Insights


## 1️⃣ Courier Status vs Order Status

Most orders are successfully shipped or delivered.

A small proportion of orders are cancelled or delayed.

## 2️⃣ Size Distribution

Popular sizes include M, L, XL, and 2XL.

Smaller sizes like 6XL are less common.

## 3️⃣ Quantity by Size

Largest order quantities are for popular sizes like M and L.

Demand aligns with size distribution trends.

## 4️⃣ Category Distribution

Top categories include T-shirts, Shirts, and Blazzers.

Premium categories like Blazers have fewer orders but higher average order values.

## 5️⃣ Top 10 States by Orders

States with highest order volumes: Maharashtra, Karnataka, Uttar Pradesh.

Major metro cities such as Mumbai, Bengaluru, and Lucknow contribute significantly to sales.

## 🧹 Data Quality Notes

Missing values exist in fulfilled-by, New, and PendingS

Postal codes are stored as float; convert to string for consistency

Convert Date to datetime for time-series analysis

## 🛠️ Recommended Preprocessing

Convert Date column to datetime format

df['Date'] = pd.to_datetime(df['Date'])

Convert ship-postal-code to string

df['ship-postal-code'] = df['ship-postal-code'].astype(str)

Fill missing values appropriately

df.fillna('Unknown', inplace=True)

## 📌 Tools & Technologies

Python (Pandas, NumPy)

Visualization: Matplotlib, Seaborn

Optional: SQL databases (MySQL / SQL Server)

## 📄 License

For educational and analytical purposes only.

## 👤 Author

Kambala Suneel Kumar
