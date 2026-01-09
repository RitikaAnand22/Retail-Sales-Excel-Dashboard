# Retail Sales Performance Dashboard (Excel)

## 📌 Project Overview
This project demonstrates an end-to-end data analysis workflow using Microsoft Excel. 
The objective was to analyze retail sales performance and provide actionable insights 
using Pivot Tables, XLOOKUP, and interactive dashboards, DAX measures.

---

## 🧩 Business Problem
- Which regions are not meeting sales expectations?
- Which customer segments drive the highest and lowest revenue?
- What categories contribute most to achieving the target?
- Why does one region outperform others?
- Should marketing or inventory be increased in low-performing regions?
- Are logistics or customer demand affecting certain regions?
- Are Corporate and Home Office customers under-targeted?
- Is the Average Order Value (AOV) lower for certain segments?
- Can tailored offers improve segment performance?

** ** Solutions :
- Total sales of $2.26M are below the $3M target, indicating a performance gap

- Identified underperforming regions impacting overall revenue

- Analyzed customer segments to understand sales contribution differences

- Evaluated product categories to highlight growth and low-performing areas

- Assessed shipping modes and order patterns for efficiency improvements

Performed sales forecasting using a line chart to predict future trends and support data-driven planning
---

## 🗂 Dataset
- Source: Kaggle (Superstore Sales Dataset)
- Format: CSV
- Records: ~10,000 rows

## 🌍 Analysis Measures
   **- Total Sales**
     TotalSales = SUM(Sales[Sales])

   **- MoM Growth%**
     MoM Growth % =DIVIDE( [Total Sales]
    - CALCULATE([Total Sales], DATEADD('Date'[Date], -1, MONTH)),
    CALCULATE([Total Sales], DATEADD('Date'[Date], -1, MONTH))
)

**- AVERAGE ORDER VALUE (AOV)**
    AOV = DIVIDE([Total Sales], [Total Orders])

**- Total Customer**
     Total Customers = DISTINCTCOUNT(Sales[Customer ID])

**- Total Order**
     Total Orders = DISTINCTCOUNT(Sales[Order ID])


## 🔧 Tools & Skills Used
- Microsoft Excel
- Data Cleaning & Preparation
- Pivot Tables & Pivot Charts
- XLOOKUP & Calculated Fields
- Slicers & Timelines
- DAX measures 
- KPI Dashboard Design

---

## 🎯 Target Assumptions
The original dataset did not include sales targets. 
A separate target table was created based on category-level historical averages 
with an assumed growth rate of 8–15% to simulate real business planning scenarios.

---

## 📊 Dashboard Preview
![Dashboard Overview] : https://drive.google.com/file/d/1u-H4dB3jM4SayZ1DXENxJhIyze6c_rkh/view?usp=sharing

---

## 🔍 Key Insights
- The technology category contributes the highest revenue but has higher variability.
- Office Supplies shows stable growth and consistently meets targets.
- Certain regions underperform against targets and require focused action.

---

## 📁 Repository Structure
