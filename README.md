# 🛒 Zepto Inventory & Sales SQL Data Analysis

## 📌 Project Overview
This project performs end-to-end data cleaning, transformation, and exploratory data analysis (EDA) on Zepto e-commerce product data using **MySQL**. The goal is to analyze product inventory, pricing strategies, stock availability, and category-level insights to support data-driven decision-making.

---

## 🛠️ Data Cleaning & Transformations
Key data prep steps performed in MySQL:
1. **Data Import & Type Casting:** Configured table schema (`sku_id`, `category`, `name`, `mrp`, `discountPercent`, `availableQuantity`, `discountSellingPrice`, `weightInGms`, `outOfStock`, `quantity`).
2. **Handling Invalid Data:** Removed erroneous rows where products had `MRP = 0` or missing key attributes.
3. **Currency Normalization:** Converted price columns (`MRP` and `discountSellingPrice`) from paisa to rupees (`Price / 100.0`).
4. **Data Deduplication:** Identified duplicate product names using `GROUP BY name HAVING COUNT(sku_id) > 1`.

---

## 🔍 Key Insights & Queries Analyzed
- **Inventory Health:** Total unique SKUs and total stock items available (`COUNT(*)`, `SUM(availableQuantity)`).
- **Out-of-Stock Analysis:** Count and percentage of products currently marked as out of stock (`outOfStock = 1`).
- **Pricing & Discounts:** Analysis of average discounts and price distributions across product categories.
- **Top Categories:** Categorical breakdown of available inventory and SKU representation.

---

## 🧰 Tech Stack & Tools Used
- **Database Engine:** MySQL 8.0
- **Database GUI:** MySQL Workbench
- **Language:** SQL (DDL, DML, Aggregations, Data Cleaning)
- **Version Control:** Git & GitHub

---

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/subasakthivaishnavi-ctrl/Zepto-SQL-Project.git](https://github.com/subasakthivaishnavi-ctrl/Zepto-SQL-Project.git)
