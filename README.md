# **Walmart Sales Data Analysis – SQL Project**

## **Project Overview**
This project involves analyzing **Walmart's sales data** to gain insights into high-performing branches, top-selling products, and customer purchasing behavior. By examining sales trends across different locations and customer segments, we aim to optimize **sales strategies and business decisions**. The dataset used in this project comes from the **Kaggle Walmart Sales Forecasting Competition** and includes transactional data from three branches.

---

## **Objectives of the Project**
The primary goal of this project is to extract meaningful insights from Walmart’s sales data and evaluate various factors that impact sales performance across different branches and product lines.

---

## **Dataset Overview**
The dataset comprises sales transactions from three Walmart branches located in **Mandalay, Yangon, and Naypyitaw**. It includes **17 columns** and **1,000 rows** detailing customer purchases, product details, payment methods, and revenue data.

### **Dataset Attributes**

| Column Name        | Description                                      | Data Type          |
|--------------------|------------------------------------------------|-------------------|
| invoice_id        | Unique identifier for each transaction           | VARCHAR(30)      |
| branch           | Store branch where the sale occurred             | VARCHAR(5)       |
| city            | City where the branch is located                 | VARCHAR(30)      |
| customer_type   | Type of customer (e.g., Member, Non-Member)      | VARCHAR(30)      |
| gender         | Gender of the customer                           | VARCHAR(10)      |
| product_line   | Category of product purchased                    | VARCHAR(100)     |
| unit_price     | Price of a single unit of the product            | DECIMAL(10,2)    |
| quantity      | Number of units sold                            | INT              |
| VAT          | Value-added tax on the purchase                  | FLOAT(6,4)       |
| total        | Final amount after tax                           | DECIMAL(12,4)    |
| date         | Date of the transaction                         | DATETIME         |
| time         | Time of the transaction                         | TIME             |
| payment      | Payment method used                              | DECIMAL(10,2)    |
| cogs         | Cost of goods sold                              | DECIMAL(10,2)    |
| gross_margin_pct | Gross margin percentage                   | FLOAT(11,9)      |
| gross_income  | Profit generated from sales                    | DECIMAL(12,4)    |
| rating       | Customer rating of the transaction             | FLOAT(2,1)       |

---

## **Key Areas of Analysis**

### **1. Product Performance Analysis**
- Evaluate sales trends for different product lines.
- Identify the **top-performing and underperforming** product categories.
- Analyze which product lines contribute the most to **total revenue**.

### **2. Sales Trend Analysis**
- Assess seasonal trends and variations in **monthly sales revenue**.
- Determine the most **profitable months and branches**.
- Measure the **efficiency of sales strategies** and suggest potential improvements.

### **3. Customer Behavior Analysis**
- Segment customers based on their purchasing behavior.
- Examine the correlation between customer type and **sales revenue**.
- Identify the **most frequent payment methods** and customer preferences.

---

## **Methodology and Approach**

### **1. Data Preparation & Cleaning**
- Created SQL tables and inserted data.
- Checked for **null or missing values** and handled inconsistencies.
- Ensured data integrity by enforcing **NOT NULL** constraints during table creation.

### **2. Feature Engineering**
To enhance the dataset, new columns were generated:
- **time_of_day** – Categorized sales into **Morning, Afternoon, and Evening** for analyzing time-based sales trends.
- **day_name** – Extracted the **day of the week** to determine the busiest days per branch.
- **month_name** – Extracted the **month** to find seasonal sales trends.

### **3. Exploratory Data Analysis (EDA)**
- Conducted in-depth **statistical analysis and data visualization**.
- Used SQL queries to extract key insights about **sales trends, customer behavior, and product performance**.
- Answered various **business-critical questions** related to revenue, sales trends, and customer engagement.

---

## **Key Business Insights**

### **General Information**
✅ How many cities are represented in the dataset?
✅ In which cities are Walmart branches located?

### **Product Insights**
✅ Number of unique **product lines** available.
✅ Most frequently used **payment methods**.
✅ **Top-selling** product line and those needing improvement.
✅ **Highest revenue-generating** product line.
✅ Branches with **above-average product sales**.
✅ VAT (Value-Added Tax) distribution among product lines.
✅ Gender distribution in product purchases.
✅ **Average customer ratings** per product category.

### **Sales Performance Analysis**
✅ Sales distribution by **time of day (Morning, Afternoon, Evening)**.
✅ **Customer segment that contributes most to revenue**.
✅ City with the **highest tax percentage (VAT)**.
✅ Customer types that pay the highest VAT.

### **Customer Behavior Insights**
✅ Number of **unique customer types**.
✅ Gender-based customer distribution.
✅ **Most preferred payment method**.
✅ **Most common customer type**.
✅ Purchasing behavior by **time of day and day of the week**.
✅ Relationship between **customer ratings and sales periods**.

---

## **SQL Queries & Techniques Used**
- **Aggregation Queries** – SUM(), AVG(), COUNT() to analyze sales data.
- **JOINS** – Combined multiple tables for in-depth analysis.
- **Window Functions** – Used RANK(), DENSE_RANK() to find top-performing products.
- **Case Statements** – Categorized sales time and customer segments.
- **CTEs (Common Table Expressions)** – Created reusable queries for complex analysis.

---

## **Tech Stack**
🔹 **SQL (MySQL/PostgreSQL)** – Data retrieval and analysis  
🔹 **Python (Pandas, Matplotlib, Seaborn)** – Visualization and further analysis  
🔹 **Excel** – Exploratory analysis and trend identification  

---

## **Future Enhancements**
🚀 **Predictive Analysis** – Implement machine learning models to forecast sales.  
🚀 **Customer Segmentation Model** – Use clustering techniques to better target customer groups.  
🚀 **Dashboard Development** – Create an **interactive Power BI/Tableau dashboard** for real-time sales tracking.  

This project provides **valuable business insights** into Walmart's sales data, helping optimize **marketing strategies, inventory management, and customer engagement**. 🚀
