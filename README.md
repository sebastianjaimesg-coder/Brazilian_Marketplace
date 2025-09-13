# 🛒 Brazilian E-Commerce Marketplace Analytics  

## 📌 Project Overview  
This project analyzes data from the **Olist Brazilian E-Commerce Marketplace** using **SQL + Power BI**.  
The goal is to simulate a real business intelligence workflow:  
- Import raw CSV data into a relational **MySQL database**.  
- Clean, transform, and query the data with **SQL**.  
- Build interactive dashboards in **Power BI** for business insights.  

The dataset contains millions of records about orders, customers, sellers, products, payments, reviews, and delivery logistics.  

---

## 🎯 Objectives  
- Create a **relational database schema** for the marketplace.  
- Perform **SQL queries** to generate KPIs:  
  - Monthly sales trends.  
  - Average order value (ticket size).  
  - Customer retention (new vs returning).  
  - Top product categories.  
  - Delivery performance.  
- Design a **Power BI dashboard** with interactive visualizations.  
- Demonstrate end-to-end BI skills: ETL, SQL, visualization, storytelling.  

---

## 🗂️ Dataset  
Source: [Olist E-Commerce Dataset on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  

Tables included:  
- **customers** → customer IDs, location.  
- **orders** → order details, status, timestamps.  
- **order_items** → products per order, prices, freight.  
- **products** → product metadata (category, dimensions).  
- **sellers** → seller IDs, location.  
- **payments** → payment method, value, installments.  
- **reviews** → customer review scores and comments.  
- **geolocation** → latitude/longitude of zip codes.  

---

## 🛠️ Tools & Technologies  
- **SQL (MySQL)** – data modeling, queries, ETL.  
- **Power BI** – dashboard and visualization.  
- **Python (optional)** – data import automation.  
- **GitHub** – project documentation and code sharing.  

---

## ⚙️ Database Schema  
Relational structure (simplified):  

```text
customers --< orders --< order_items >-- products  
                          |  
                          >-- payments  
                          >-- reviews  
sellers   --< order_items  
```

---

## 📊 Power BI Dashboard  
**Main KPIs:**  
- Total sales & monthly revenue trend.  
- Average order value (ticket).  
- Top 10 product categories by revenue.  
- New vs returning customers.  
- Delivery performance (estimated vs actual).  

 

---

## 📂 Repository Structure  
```text
/SQL
   customers.sql
   orders.sql
   queries_kpis.sql
/PowerBI
   ecommerce_dashboard.pbix
/Docs
   dashboard_screenshots.png
