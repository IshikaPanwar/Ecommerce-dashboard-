<img width="1164" height="640" alt="image" src="https://github.com/user-attachments/assets/a1b62183-e643-419d-bfcc-5debbc93c8e9" />

# 🛒 Ecommerce Sales Dashboard


## 📖 Project Overview

This Power BI project involves the analysis of an Ecommerce sales dataset to identify key trends, top-performing regions, and customer preferences. The interactive dashboard provides a comprehensive view of sales performance, profit margins, and quantity sold across various dimensions such as state, category, and payment mode.

The report allows stakeholders to make data-driven decisions regarding inventory management, marketing strategies, and regional expansion.

---

## 📸 Dashboard Preview


*(Note: This dashboard is interactive. Download the `.pbix` file to explore.)*

---

## 🔍 Key Insights & Findings

Based on the data visualized in the report:

* **Sales Performance:**
    * **Total Amount:** 438K
    * **Total Profit:** 37K
    * **Total Quantity:** 5,615 units
* **Regional Analysis:** **Uttar Pradesh** is the leading state in terms of sales amount, followed by Maharashtra and West Bengal.
* **Product Preferences:**
    * **Clothing** dominates the quantity sold, accounting for **63%** of the total volume.
    * **Printers** and **Bookcases** are the most profitable sub-categories.
* **Customer Behavior:**
    * **Cash on Delivery (COD)** is the most preferred payment mode (44%), followed by UPI (21%).
    * Top Customers like **Yogesh** significantly contribute to the revenue stream.
* **Seasonality:**
    * The business sees peak profits in **January** and **November**.
    * Significant profit dips (losses) were observed in May, July, and December, suggesting areas for cost investigation.

---

## 🛠️ Data Processing & Modeling

### 1. Data Cleaning (Power Query)
* Handled missing values and standardized text formats.
* Created conditional columns for data categorization.
* Formatted date tables for time-intelligence analysis.

### 2. Data Modeling
* Established relationships between the Sales Fact Table and dimension tables (Customers, Products, Geography).
* Used a Star Schema approach for optimized performance.

### 3. DAX Measures
Key measures created for this report include:
* `Sum of Amount` = SUM(Sales[Amount])
* `Sum of Profit` = SUM(Sales[Profit])
* `Sum of Quantity` = SUM(Sales[Quantity])
* `Profit Margin %` = DIVIDE([Sum of Profit], [Sum of Amount], 0)

