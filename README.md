# Zepto-SQL-Project

📌 Project Overview

The goal is to simulate how actual data analysts in the e-commerce or retail industries work behind the scenes to use SQL to:

✅ Set up a messy, real-world e-commerce inventory database

✅ Perform Exploratory Data Analysis (EDA) to explore product categories, availability, and pricing inconsistencies

✅ Implement Data Cleaning to handle null values, remove invalid entries, and convert pricing from paise to rupees

✅ Write business-driven SQL queries to derive insights around pricing, inventory, stock availability, revenue and more

📁 Dataset Overview
The dataset was sourced from Kaggle and was originally scraped from Zepto’s official product listings. It mimics what you’d typically encounter in a real-world e-commerce inventory system.

Each row represents a unique SKU (Stock Keeping Unit) for a product. Duplicate product names exist because the same product may appear multiple times in different package sizes, weights, discounts, or categories to improve visibility – exactly how real catalog data looks.

🧾 Columns:

sku_id: Unique identifier for each product entry (Synthetic Primary Key)

name: Product name as it appears on the app

category: Product category like Fruits, Snacks, Beverages, etc.

mrp: Maximum Retail Price (originally in paise, converted to ₹)

discountPercent: Discount applied on MRP

discountedSellingPrice: Final price after discount (also converted to ₹)

availableQuantity: Units available in inventory

🧠 Zepto Product Data Analysis – Project Summary
This project involves analyzing product-level data to derive actionable business insights for a retail company.

🗄️ Database & Table Setup
Designed and created a PostgreSQL table with relevant fields (category, price, discount %, stock, etc.)

Imported data from a CSV using \copy command and pgAdmin

🔍 Data Exploration
Assessed dataset structure, null values, unique categories

Analyzed stock status and duplicate product entries

🧹 Data Cleaning
Removed entries with invalid pricing (MRP or discounted price = 0)

Standardized price units from paise to rupees

📊 Business Insights
Top 10 best-value products by discount %

Identified costly products with low discounts

Revenue potential by category

Price-per-gram analysis for value detection

Weight-based product categorization (Low/Medium/Bulk)

weightInGms: Product weight in grams

outOfStock: Boolean flag indicating stock availability

quantity: Number of units per package (mixed with grams for loose produce)
