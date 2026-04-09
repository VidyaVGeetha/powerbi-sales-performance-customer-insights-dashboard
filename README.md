# 📊 Sales Performance & Customer Insights Dashboard (Power BI)

## 📌 Project Overview

This project focuses on analyzing sales performance and customer behavior using Power BI.
The dataset consists of customer and order data, which were transformed into a structured data model to generate meaningful business insights.

---

## 🎯 Business Objective

* Analyze sales trends over time
* Identify high-performing locations
* Understand customer segmentation
* Evaluate order behavior and payment preferences

---

## 🧠 Approach (Data Analyst Workflow)

1. Data Understanding
2. Data Cleaning & Validation
3. Data Modeling
4. DAX Calculations
5. Performance Optimization
6. Dashboard Development

---

## 🔍 Data Cleaning & Validation

### Customers Table

* Ensured **Customer ID uniqueness**
* Converted **Date of Birth to Date format**
* Validated:

  * No invalid or missing values
  * Names contain only text
  * Phone numbers stored as text
  * Consistent membership tiers

### Orders Table

* Ensured **Order ID uniqueness**
* Converted:

  * Order Date → Date type
  * Numeric fields → Whole/Decimal numbers
* Validated:

  * No negative values in financial fields
  * Order Quantity > 0
  * Customer IDs match Customers table
  * Payment methods are consistent

---

## 🔗 Data Modeling

* Created relationship:

  **Customers (1) → Orders (*)**

* Key:

  * Customers[Customer ID] → Orders[Customer ID]

* Cardinality: **One-to-Many**

* Cross filter direction: **Single**

### 📅 Date Table (Best Practice)

* Created a dedicated Date table

* Established relationship:

  **Date[Date] → Orders[Order Date]**

* Used Date table for all time intelligence calculations

---

## ⚙️ DAX Measures

### Core Metrics

* Total Sales
* Total Orders
* Total Customers
* Average Order Value (AOV)

### Time Intelligence

* Sales YTD
* Previous Month Sales
* Month-over-Month Growth (%)

### Key Concept

* Used **Date Table instead of Order Date** for accurate and scalable time-based analysis

---

## 📊 Dashboard Features

### KPI Cards

* Total Sales
* Total Orders
* Total Customers
* Average Order Value

### Visualizations

* 📈 Sales Trend Over Time (with YTD)
* 🌍 Sales by Location
* 💳 Orders by Payment Method

### Filters (Slicers)

* Date range
* Location
* Membership Tier

---

## 📈 Key Insights

### 🌍 Location Analysis

* Mexico City and New York are top-performing locations in terms of sales and order volume
* Berlin shows the highest average order value, indicating high-value transactions
* Some locations show lower performance, highlighting growth opportunities

### 👥 Customer Segmentation

* Platinum customers generate the highest revenue
* Silver customers have the highest number of orders, indicating strong engagement
* Bronze and Gold tiers contribute moderate performance

### 💳 Order Behavior

* Credit Card is the most preferred payment method
* PayPal is also widely used, showing the need for multiple payment options

### 📈 Sales Trend

* Sales show an overall upward trend (YTD growth)
* Monthly sales fluctuate, indicating variability in demand
* Growth stabilizes in later periods

---

## ⚡ Performance Optimization

* Disabled Auto Date/Time
* Optimized data types
* Used measures instead of calculated columns
* Maintained a clean data model

---

## 📸 Dashboard Preview

<img width="616" height="360" alt="Dashboard_ScreenshotNew" src="https://github.com/user-attachments/assets/2deae86f-9652-4663-b386-7b67f3039bb4" />

---

## 🧠 Key Learnings

* Importance of data validation before analysis
* Building efficient data models in Power BI
* Using DAX for business calculations
* Implementing time intelligence using Date table
* Designing clean and interactive dashboards

---

## 🚀 Conclusion

This project demonstrates the complete data analysis workflow using Power BI, from data preparation and modeling to delivering actionable insights through an interactive dashboard.

---
Author

Vidya Vishnuvihar Geetha
