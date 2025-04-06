
# 🛒 Retail Sales SQL Analysis

This project explores a **retail sales dataset** using **SQL queries** to extract meaningful business insights. The goal is to analyze customer behavior, sales trends, and category performance using structured queries.

---

## 📁 Project Structure

- **SQL File**: [`sql_project_1.sql`](sql_project_1.sql)  
  Contains the table creation statement and SQL queries for analysis.

---

## 🧱 Database Schema

A single table named `retail_sales` is used with the following structure:

```sql
CREATE TABLE retail_sales (
    transaction_id INT PRIMARY KEY,	
    sale_date DATE,	 
    sale_time TIME,	
    customer_id INT,
    gender VARCHAR(15),
    age INT,
    category VARCHAR(15),	
    quantity INT,
    price_per_unit FLOAT,	
    cogs FLOAT,
    total_sale FLOAT
);
```

Each row represents a transaction, containing customer demographics, product category, pricing, quantity sold, and time of sale.

---

## 🔍 Analytical Questions & SQL Solutions

This project answers 10 targeted business questions using SQL:

1. **Daily Sales Retrieval**  
   → Retrieve all columns for sales made on `2022-11-05`.

2. **High-Volume Clothing Sales in Nov 2022**  
   → Find transactions where the category is **'Clothing'** and quantity sold is **more than 10** in **November 2022**.

3. **Category-Wise Sales Summary**  
   → Calculate **total sales (`total_sale`)** for each category.

4. **Average Age of Beauty Shoppers**  
   → Find the **average age** of customers who purchased from the **'Beauty'** category.

5. **High Value Transactions**  
   → List all transactions where `total_sale` is **greater than 1000**.

6. **Gender & Category-Wise Transaction Count**  
   → Count the number of transactions made by **each gender** in **each category**.

7. **Monthly Sales Trends & Best Month Per Year**  
   → Calculate the **average sale per month** and identify the **best-selling month each year**.

8. **Top Customers by Total Spend**  
   → Identify the **top 5 customers** based on **highest total sales**.

9. **Unique Customers per Category**  
   → Count the **number of unique customers** who purchased from **each category**.

10. **Sales by Shift**  
    → Classify transactions into **Morning (≤ 12:00)**, **Afternoon (12:01–17:00)**, and **Evening (> 17:00)**, then count number of orders per shift.

---

## 📊 Insights You Can Derive

- Popular product categories and top-selling months
- Customer behavior by age and gender
- High-value customers for targeted campaigns
- Time-of-day patterns for staffing or marketing

---

## 🚀 How to Run

1. Import or create the `retail_sales` table in your SQL environment (MySQL/PostgreSQL/etc.)
2. Copy the queries from [`sql_project_1.sql`](sql_project_1.sql) and execute them sequentially
3. Explore and expand the analysis based on your business goals

---

## 🧠 Tools Used

- SQL (Standard queries, aggregation, joins, date/time functions)
- Any RDBMS (e.g., MySQL, PostgreSQL, SQLite)

---

## 📎 License

This project is open-source and free to use under the [MIT License](LICENSE).
