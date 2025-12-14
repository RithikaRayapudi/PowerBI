#  Sales Performance & Trend Analysis Dashboard (Power BI)

## Project Overview
This project implements an **enterprise-grade Sales Performance and Trend Analysis dashboard** using **Power BI Desktop and Power BI Service**.  
The dashboard enables interactive analysis of **sales, profit, quantity, trends, and target achievement** to support data-driven business decisions.

---

## Data Sources
- **Sales Data (Excel)**  
  Orders, products, customers, regions, sales amount, profit, and quantity.
- **Sales Targets Data (Excel)**  
  Monthly and category-wise sales targets.
- **Date Dimension**  
  Used for time-based analysis and trend calculations.

> Excel files were maintained as the **single source of truth** and refreshed in Power BI.

---

## Data Preparation (Power Query)
- Removed null values and duplicates  
- Corrected data types  
- Split and standardized columns (region, category, date)  
- Created conditional columns for business classification  

---

## Data Modeling
- Implemented a **Star Schema**:
  - `FactSales`
  - `DimDate`
  - `DimProduct`
  - `DimCustomer`
  - `DimRegion`
- Applied **one-to-many relationships**
- Used **single-direction filtering**
- Marked the Date table as a **Date Table**

---

## DAX Calculations
The following DAX measures were created:
- **Total Sales**
- **Total Profit**
- **Total Quantity**
- **Sales YTD**
- **Sales Last Year (LY)**
- **Year-over-Year (YoY) Growth %**
- **Target Achievement %**

These measures ensured reusable and accurate calculations across all visuals.

---

## Report Pages
### Executive Dashboard
- KPI cards for Sales, Profit, YoY Growth, and Target Achievement  
- Donut chart for sales by category  
- Line chart for monthly sales trends  

### Trend Analysis
- Sales and profit trends over time  
- Time-based comparison visuals  

### Product Performance
- Matrix with category → subcategory → product hierarchy  
- Conditional formatting for sales and profit  
- **Top 10 products** using Top-N filtering  

### Advanced Analytics
- **R Script Visual** used to analyze sales trends  
- Missing values handled in the R script for stable visualization  

---

## Advanced Analytics (R Visual)
An **R script visual** was implemented in Power BI Desktop to plot sales trends over time.  
This demonstrates the use of external analytics for advanced visualization.

---

## Power BI Service Features
- Report published to **Power BI Service**
- **Dashboard** created and key visuals pinned
- **Q&A visuals** enabled for natural language queries
- **KPI alerts** configured for monitoring critical metrics

---

## Outcome
The final solution delivers a **scalable, interactive, and enterprise-ready Power BI dashboard** that provides clear insights, advanced analytics, and real-time monitoring capabilities.

---

## Tools & Technologies
- Power BI Desktop  
- Power BI Service  
- DAX  
- Power Query  
- R (for advanced visuals)  
- Microsoft Excel  

---
