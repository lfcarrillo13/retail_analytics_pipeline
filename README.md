# retail_analytics_pipeline
This repository demonstrates a complete analytics workflow: raw retail data → Python/SQL cleaning &amp; analysis → cleaned dataset exported to Power BI → interactive two-page dashboard (KPIs, trends, customer insights).
# Retail Sales Analytics Pipeline – Python, SQL & Power BI

## 📌 Overview
This repository demonstrates a complete **end-to-end analytics workflow** built from raw retail sales data.  
Starting with CSV transactions, I used **SQL** to model and query data, **Python** for cleaning, feature engineering and exploratory analysis, and then delivered insights through an **interactive Power BI dashboard**.  

## 🛠️ Tech Stack & Skills Demonstrated
- **Python (pandas, matplotlib)** – data loading, cleaning, transformation, exploratory analysis, feature engineering  
- **PostgreSQL / SQL** – database design, data quality checks, aggregations, window functions for KPIs  
- **Power BI** – connecting the cleaned dataset to build interactive dashboards with KPIs, trends, and filters  
- **Data Quality & Documentation** – null handling, type casting, schema consistency  

## 📂 Project Structure
retail-analytics-pipeline/
│
├── data/
│ ├── retail_sales.csv # Original dataset
│ 
├── notebooks/
│ └── jupyter retail sales.ipynb # Python data cleaning & analysis notebook
│
├── sql/
│ └── SQL QUERY P1.sql # SQL scripts for table creation & business queries
│
├── powerbi/
│ ├── Retail Sales PowerBI Sheet.pbix # Interactive Power BI dashboard (2 pages)
│ └── screenshots/ # Optional: PNG screenshots of dashboard pages
│
└── README.md # This file


## 🔑 Workflow Highlights

### 1. Data Ingestion & Cleaning
- Imported raw CSV retail transactions into pandas.
- Standardized column names, parsed dates/times, coerced numeric fields.
- Dropped invalid rows to ensure data quality before analysis.

### 2. SQL Modeling & Business Queries
- Created a `retail_sales` table with appropriate data types and constraints:contentReference[oaicite:0]{index=0}.
- Checked for null values and removed invalid records.
- Developed 10+ business-focused SQL queries:
  - Total sales by category, average age of Beauty customers.
  - High-value transactions and top 5 customers by total spend.
  - Monthly best-selling periods and shift-based order counts.

### 3. Python Analysis & Feature Engineering
- Derived a `Shift` column (Morning / Afternoon / Evening) from sale time to analyze patterns by time of day.
- Calculated profit as `total_sale - cogs`.
- Computed KPIs: total transactions, unique customers, and average sale per transaction.
- Built clear charts with matplotlib to visualize category sales, shift distribution, time-series trends, and top customers.

### 4. Power BI Dashboard
- Exported a cleaned dataset from Python to Power BI.
- Built a **two-page interactive dashboard**:
  - **Page 1:** KPIs, category performance, and top customers.
  - **Page 2:** Daily/monthly sales trends with slicers for category and shift.
- Added interactivity (filters, slicers) to make insights business-friendly.

## 📈 Sample Insights
- Clothing category generated the highest total sales.
- Afternoon shifts saw the greatest number of transactions.
- Top 5 customers contributed a disproportionate share of total sales.
- Clear seasonal peaks visible in monthly trend analysis.


