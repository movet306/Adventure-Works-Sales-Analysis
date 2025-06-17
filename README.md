# Adventure Works Sales Analysis

> **End-to-end Sales Analytics using SQL & Power BI**

![image](https://github.com/user-attachments/assets/213cd5ca-2068-4ef2-9859-edbfd06b45e7)


## Executive Summary

In this project, I built an interactive sales dashboard for Adventure Works by **combining the power of SQL Server** (for data engineering and heavy calculations) **with Power BI** (for data modeling, analytics, and data storytelling).  
Rather than just presenting charts, my aim was to answer real business questions, uncover actionable insights, and build an analytical foundation for data-driven decision-making.

---

## My Analytical Process

### 1. Data Sourcing & Preparation (SQL Server)

- **Source:** AdventureWorksDW2019 (sample enterprise data warehouse)
- **Approach:**  
  I used SQL to aggregate, filter, and pre-process millions of sales records, ensuring performance and accuracy at the data source.
- **Typical SQL Tasks:**
    - Monthly/Yearly sales aggregations
    - Product and customer segmentation
    - KPI calculations (AOV, Repeat Rate, Top N)
- **SQL Query Examples:**
  ![image](https://github.com/user-attachments/assets/82e111c3-6679-452e-9adb-b24df9559bba)
![image](https://github.com/user-attachments/assets/81c1b6cb-d638-43e1-9ec2-c135b7267d55)
![image](https://github.com/user-attachments/assets/feeffa88-8b65-4db4-8442-45239bd46f3d)


- **Rationale:**  
  Complex business calculations are handled at the source, ensuring Power BI only receives clean, analysis-ready data. This approach improves report performance and reliability.

---
### 2. Data Modeling in Power BI

- **Star Schema:**  
  I designed a clear data model using fact and dimension tables (Sales, Product, Customer, Date, Geography).
- **Relationship Design:**  
  Proper one-to-many relationships enable seamless cross-filtering and drilldown.
- **Dynamic Measures:**  
  KPIs such as Total Sales, Orders, Average Order Value, Repeat Rate, and Top N logic are calculated in DAX.

   ![image](https://github.com/user-attachments/assets/9d3c15ac-d38d-49f5-83d3-57633271b279)


---

### 3. Dashboard Design & Data Storytelling

- **Key Visuals:**
    - **Executive KPIs:** Total Sales, Total Orders, Total Customers, Average Order Value, Repeat Customers
    - **Product Analysis:** Sales by Product Category (donut chart), Top 10 Best Selling Products (bar chart)
    - **Customer Analysis:** Top 10 Customers by Sales
    - **Seasonal Trend:** Combined column & line chart (monthly sales + orders)
    - **Geographic Analysis:** Sales distribution by city (interactive map)
- **Self-Service Slicers:**  
  Filter by year, day, city, product, category, and day to enable any business user to ask and answer their own questions—instantly.

---

## Key Insights

- **Revenue is highly concentrated** in a small set of products (mainly Bikes) and top customers.
- **Seasonality is clear:** Certain months have predictable sales spikes, highlighting opportunities for targeted campaigns and inventory planning.
- **Repeat business is strong,** showing the value of nurturing loyal customers.
- **Geographically,** most revenue comes from North America & Europe, but expansion opportunities exist in other regions.

- ## Data Source
- https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksDW2019.bak 
