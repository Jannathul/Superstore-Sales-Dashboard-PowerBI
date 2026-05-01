# 📊 Sales & Profitability Intelligence Dashboard

### Power BI | Business Intelligence | Data Analytics

---

## 🚀 Executive Summary

This project presents an interactive **Power BI dashboard** designed to analyze sales performance and profitability across customer segments, product categories, and regions.

The solution focuses on identifying **revenue drivers, profit leakage, and performance gaps**, enabling stakeholders to make informed business decisions related to pricing, discount strategies, and regional optimization.

---

## 🎯 Business Problem

Organizations often struggle to:

* Identify high-revenue but low-profit segments
* Understand the impact of discounting on margins
* Analyze performance inconsistencies across regions and categories

This dashboard addresses these challenges by providing a **centralized analytical view of business performance**.

---

## 🏗️ Solution Architecture

```text
Raw Dataset (CSV / Excel)
        ↓
Data Cleaning & Transformation (Power Query)
        ↓
Data Model (Denormalized Table + Date Table)
        ↓
DAX Measures (Business Metrics & Time Intelligence)
        ↓
Interactive Dashboard (Power BI)
        ↓
Insights & Decision Support
```

---

## ⚙️ Data Preparation

* Cleaned and standardized dataset using Power Query
* Handled missing values and ensured consistency in categorical fields
* Standardized date formats and created a dedicated **Date table**
* Prepared data for efficient filtering, aggregation, and time-based analysis

---

## 🧱 Data Model Design

The dataset is implemented using a **denormalized (flat) model**, where both transactional and descriptive attributes exist within a single table.

* Single table containing Sales, Profit, Customer, Region, Category, etc.
* Separate **Date table** created for time intelligence calculations

> 🔎 Design Decision
> A denormalized model was chosen for simplicity and faster development due to dataset size.
> For large-scale production systems, a **star schema model** would be implemented to improve scalability and performance.

---

## 📊 Analytical Layer (DAX)

Key business metrics:

* **Total Sales** = SUM(Sales[Sales])
* **Total Profit** = SUM(Sales[Profit])
* **Profit Margin (%)** = DIVIDE([Total Profit], [Total Sales])
* **Year-over-Year (YoY) Growth (%)**
* **Month-over-Month (MoM) Growth (%)**

Time intelligence functions used:

* `SAMEPERIODLASTYEAR`
* `PREVIOUSMONTH`

---

## 📈 Dashboard Capabilities

* **Executive KPI Overview** – High-level performance metrics (Sales, Profit, Orders, Margin)
* **Customer Segment Analysis** – Revenue and profitability across segments
* **Regional Performance Analysis** – Comparative performance across regions
* **Category & Sub-category Insights** – Product-level contribution and trends
* **Profitability Deep Dive** – Impact of discounting on profit margins
* **Controlled Visual Interactions** – Ensures consistent and meaningful filtering behavior

---

## 💡 Key Insights

* Consumer segment contributes the highest share of revenue
* High discount levels negatively impact overall profitability
* Certain regions generate strong sales but weak margins
* Category-level analysis reveals patterns of profit leakage

---

## 🎯 Business Impact

This solution enables stakeholders to:

* Identify and prioritize **high-value customer segments**
* Optimize **pricing and discount strategies**
* Improve **regional sales performance**
* Detect and reduce **profit leakage**

---

## 🔄 Scalability & Future Enhancements

To extend this solution for enterprise-scale use:

* Transition to **Star Schema Data Model**
* Implement **ETL pipelines for automated data ingestion**
* Enable **Incremental Data Refresh**
* Integrate with **Cloud Data Warehouse (e.g., Snowflake)**
* Add **predictive analytics and forecasting models**

---

## 🛠️ Tools & Technologies

* **Power BI** (Data Modeling, DAX, Visualization)
* **Power Query** (Data Transformation)

---

## 🌐 Live Dashboard

👉 [View Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMDQ1MGEzNGEtMzQ3Ni00ZjYyLWI0MDQtYzM1YTVlN2M4M2FjIiwidCI6ImZlMTc4MjFiLTdhMTAtNDdmZi1hZDZhLWNlOWM5Y2Y4OWU3NCIsImMiOjF9)

---

## 📄 Report

👉 [Download PDF](https://github.com/Jannathul/Superstore-Sales-Dashboard-PowerBI/raw/main/SuperStore%20Sales.pdf)

---

## ⭐ Final Note

This project demonstrates:

* Strong **analytical thinking**
* Effective **data modeling decisions**
* Clear focus on **business impact and insights**

---
