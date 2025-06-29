# Apple_Store_Project (2024)


## 📊 Apple Retail Sales Analysis Using Advanced SQL  
**A Portfolio Project Featuring Over 1 Million Rows of Global Sales Data**

This project demonstrates advanced SQL querying techniques applied to a large-scale dataset from Apple retail operations. With over 1 million rows of data spanning global store locations, product categories, sales transactions, and warranty claims, the project simulates real-world business scenarios that data analysts frequently encounter.

The objective is to extract actionable insights, optimize query performance, and apply analytical thinking to solve complex business questions using structured data.

---
![Image](https://github.com/user-attachments/assets/af1b302b-1691-4305-8151-166c0dd0f57c)

## 🧱 Database Overview

The analysis is based on a relational database with five core tables:

1. **stores** – Apple retail locations, including store name, city, and country  
2. **category** – Product categories such as iPhones, iPads, and accessories  
3. **products** – Product-level details including launch date and price  
4. **sales** – Transaction-level data capturing product sales across stores  
5. **warranty** – Warranty claim records linked to sales, with claim status  

This schema supports a wide range of analytical use cases, from performance benchmarking to customer behavior analysis.

---

## 🔍 Project Objectives

The project is structured into three tiers of complexity to showcase a progression of SQL skills:

### Tier 1: Foundational Analysis (10 Queries)
- Store distribution by country  
- Total units sold per store  
- Monthly sales volume (e.g., December 2023)  
- Stores with zero warranty claims  
- Percentage of claims marked as "Warranty Void"  
- Top-performing store by units sold (last 12 months)  
- Unique products sold in the past year  
- Average product price by category  
- Warranty claims filed in a specific year (e.g., 2020)  
- Best-selling day per store based on quantity sold  

### Tier 2: Intermediate Business Insights (5 Queries)
- Least-selling product per country per year  
- Warranty claims filed within 180 days of purchase  
- Claims associated with recently launched products (last 2 years)  
- High-volume sales months in the USA (over 5,000 units)  
- Most-claimed product category in the past two years  

### Tier 3: Advanced Analytical Challenges (5 Queries)
- Country-wise probability of a warranty claim per purchase  
- Year-over-year growth analysis by store  
- Correlation between product price and warranty claims (segmented by price range)  
- Store with the highest proportion of “Paid Repaired” claims  
- Monthly running total of sales per store over four years, with trend comparison  

### Bonus Analysis
- Product lifecycle sales trends segmented into:  
  - 0–6 months post-launch  
  - 6–12 months  
  - 12–18 months  
  - Beyond 18 months  

---
![Image](https://github.com/user-attachments/assets/e0e3d20b-9e15-4d03-884a-c6fd8f7324cc)

## 🗂️ Database Schema Overview

The project is built on a relational database consisting of five core tables. Each table captures a distinct aspect of Apple’s retail operations, enabling comprehensive analysis across sales, products, store performance, and warranty claims.

### 1. **`stores`** – Apple Retail Locations  
Contains metadata about each Apple store worldwide.  
- `store_id` – Primary key; uniquely identifies each store  
- `store_name` – Name of the retail store  
- `city` – City where the store is located  
- `country` – Country of operation  

### 2. **`category`** – Product Categories  
Defines the classification of Apple products.  
- `category_id` – Primary key; uniquely identifies each category  
- `category_name` – Name of the product category (e.g., iPhone, Mac, Accessories)  

### 3. **`products`** – Product Details  
Captures product-level information and pricing.  
- `product_id` – Primary key; uniquely identifies each product  
- `product_name` – Name of the product  
- `category_id` – Foreign key; links to the `category` table  
- `launch_date` – Official release date of the product  
- `price` – Retail price of the product  

### 4. **`sales`** – Sales Transactions  
Records each product sale across all stores.  
- `sale_id` – Primary key; uniquely identifies each transaction  
- `sale_date` – Date of the sale  
- `store_id` – Foreign key; links to the `stores` table  
- `product_id` – Foreign key; links to the `products` table  
- `quantity` – Number of units sold in the transaction  

### 5. **`warranty`** – Warranty Claims  
Tracks warranty activity and repair outcomes.  
- `claim_id` – Primary key; uniquely identifies each warranty claim  
- `claim_date` – Date the warranty claim was filed  
- `sale_id` – Foreign key; links to the `sales` table  
- `repair_status` – Status of the claim (e.g., “Paid Repaired”, “Warranty Void”)  

This schema supports a wide range of analytical use cases, including sales performance tracking, product lifecycle analysis, warranty reliability, and store-level benchmarking.

---

## 🧠 Key Skills Demonstrated

- **Advanced SQL Joins & Aggregations** – Efficiently combining and summarizing data across multiple tables  
- **Window Functions** – Implementing ranking, running totals, and time-based comparisons  
- **Temporal Analysis** – Segmenting and analyzing data across custom time frames  
- **Data Optimization** – Writing performant queries for large datasets  
- **Correlation & Trend Analysis** – Identifying relationships between variables and tracking performance over time  
- **Business-Oriented Thinking** – Translating raw data into strategic insights  

---

## 📦 Dataset Summary

- **Volume**: 1M+ rows of transactional and operational data  
- **Time Span**: Multi-year coverage for longitudinal analysis  
- **Geographic Scope**: Apple retail stores across multiple countries  

---

## 🎯 Project Outcome

This project exemplifies advanced SQL capabilities applied to a real-world, enterprise-scale dataset. It demonstrates the ability to:

- Efficiently manage and analyze large, normalized relational databases  
- Translate complex business requirements into data-driven solutions  
- Deliver clear, optimized SQL queries that surface actionable insights  
- Construct a portfolio-quality case study aligned with industry standards and expectations  


