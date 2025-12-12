# Zepto_SQL_Project

# 📦 Zepto Product & Inventory Analysis using SQL

A complete SQL project analyzing Zepto’s product dataset to uncover insights related to pricing, discount patterns, inventory availability, and category-level performance.
This project includes data exploration, data cleaning, and business-focused SQL analysis.

# 📁 Project Overview

This project focuses on analyzing Zepto’s product database using SQL to understand product pricing, discounts, inventory status, and category performance.
The SQL script performs:

Data exploration

Data cleaning

Business insights extraction

Revenue and inventory calculations

Value-based product segmentation

🛠️ Tech Stack

Database: PostgreSQL

Query Types: Aggregations, GROUP BY, DISTINCT, CASE, Filtering

# 📂 Dataset Structure

The dataset contains the following fields:

Column	Description
sku_id	Unique SKU identifier
category	Product category
name	Product name
mrp	Maximum Retail Price
discountPercent	Discount offered (%)
availableQuantity	Units available in stock
discountedSellingPrice	Selling price after discount
weightInGms	Product weight in grams
outOfStock	Boolean indicating stock availability
quantity	Pack quantity

# 🧹 Data Cleaning Performed

Removed invalid entries with MRP = 0

Converted price fields from paise to rupees

Detected missing values across key attributes

Identified duplicate product names to avoid skewed insights

# 🔍 Data Exploration

Key checks included:

Total number of records

List of unique categories

Out-of-stock vs in-stock distribution

Duplicate product names

Null value detection

# 📊 Data Analysis & SQL Queries
Q1: Top 10 Best-Value Products (Highest Discounts)

Identified products offering the highest discount percent, ranked descending.

Q2: High-MRP Out-of-Stock Products

Filtered premium products (MRP > ₹300) that are unavailable.

Q3: Estimated Revenue by Category

Calculated potential revenue =
discountedSellingPrice × availableQuantity

Q4: High-Price, Low-Discount Products

Products where:

MRP > ₹500

Discount < 10%

Q5: Top 5 Categories with Highest Average Discount

Computed category-wise mean discount percentage.

Q6: Price Per Gram Analysis

Calculated value metric =
discountedSellingPrice / weightInGms
for 100g+ products.

Q7: Weight-Based Product Segmentation

Used CASE to categorize products into:

Low (<1000g)

Medium (<5000g)

Bulk (≥5000g)

Q8: Total Inventory Weight by Category

Computed overall weight for each product category.

📄 SQL Script

# Your project includes:

✔ Table creation
✔ Data exploration queries
✔ Data cleaning
✔ Business analysis queries

# Full script is included in the repository as:

📄 zepto_sql_analysis.sql

📈 Key Insights

Some high-MRP products are out of stock, indicating potential demand–supply mismatch.

Discounts vary significantly across categories, influencing customer buying behavior.

Price-per-gram analysis reveals best-value SKUs for bulk purchases.

Category-level inventory weight helps optimize warehousing and stock rotation.

# 🚀 How to Run

Open PostgreSQL or any compatible SQL environment.

Run the CREATE TABLE script.

Insert dataset records.

Execute each query section for exploration, cleaning, and insights.
