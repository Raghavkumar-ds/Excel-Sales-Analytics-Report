# 📊 AtliQ Hardwares — Excel Sales Analytics Project
 
> **A complete end-to-end sales analytics solution built entirely in Microsoft Excel**, transforming raw business data into actionable insights using Power Query, Data Modeling, Power Pivot, DAX, and Conditional Formatting.
 
---
 
## 🚀 Project Overview
 
AtliQ Hardwares is a global hardware company selling products across **23+ countries** through **70+ customers** ranging from Amazon and Flipkart to regional brick-and-mortar chains.
 
This project analyzes **three fiscal years (2019–2021)** of sales data to answer critical business questions:
 
- 📈 Which customers drove the most revenue — and who grew the fastest?
- 🌍 Which markets are underperforming against targets?
- 🛒 What are the best-selling products?
- 🆕 How did new product launches perform in 2021?
**Total 2021 Net Sales Analyzed: $598.88 Million across all markets**
 
---
 
## 📁 Reports Included
 
| # | Report | Description |
|---|--------|-------------|
| 1 | 📋 **Customer Performance Report** | Net sales per customer for 2019, 2020, 2021 + YoY growth |
| 2 | 🎯 **Performance vs Target Report** | 2021 actual sales vs targets by market |
| 3 | 🌍 **Top 5 Country Sales Analysis** | Highest revenue-generating countries in 2021 |
| 4 | 🆕 **New Product Sales Report** | Performance of 17 new products launched in 2021 |
| 5 | 🏆 **Top 10 Products Report** | Best performing products by net sales |
 
---
 
## 🔍 Key Insights
 
### 🏆 Top Customers (2021)
| Customer | 2021 Net Sales | Growth vs 2020 |
|----------|---------------|----------------|
| Amazon | $82.09 M | 218.9% |
| AtliQ Exclusive | $61.12 M | 345.8% |
| AtliQ e Store | $52.98 M | 223.8% |
| Sage | $20.70 M | 321.5% |
| Flipkart | $19.29 M | 231.0% |
 
> 💡 **Standout:** Integration Stores clocked a jaw-dropping **887.2% growth** and Nova hit **2664.9%** — both new customers ramping up rapidly.
 
---
 
### 🌍 Top 5 Countries (2021)
| Rank | Country | Net Sales |
|------|---------|-----------|
| 🥇 | India | $241.85 M |
| 🥈 | USA | $131.23 M |
| 🥉 | South Korea | $79.05 M |
| 4 | Canada | $51.99 M |
| 5 | Philippines | $50.92 M |
 
---
 
### 🎯 Performance vs Target (2021)
Every single market **missed its 2021 target**, with a total shortfall of **-$54.94 M (-8.40%)** against a target of $653.82 M.
 
| Biggest Misses | Gap |
|----------------|-----|
| USA | -$10.24 M (-10.44%) |
| India | -$9.55 M (-5.59%) |
| Canada | -$5.07 M (-12.63%) |
| South Korea | -$4.36 M (-8.18%) |
 
> ⚠️ **Poland** had the highest miss percentage at **-15.35%**, while **Portugal** was the closest to target at just **-4.12%**.
 
---
 
### 🆕 New Products - 2021 (Total: $176.16 M)
Top performers among the 17 newly launched products:
- **AQ Qwerty** — $21.98 M
- **AQ Trigger** — $20.74 M
- **AQ Gen Y** — $19.52 M
- **AQ Trigger Ms** — $17.90 M
- **AQ Wi Power Dx3** — $17.25 M
---
 
### 🏅 Top 10 Products (All-Time)
| Product | Net Sales |
|---------|-----------|
| AQ Wi Power Dx1 | $35.57 M |
| AQ Wi Power Dx2 | $31.91 M |
| AQ 5000 Series Ultron 8 5900X Desktop | $28.62 M |
| AQ Lite | $27.06 M |
| AQ Electron 5 3600 Desktop Processor | $26.91 M |
 
---
 
## 🛠️ Tools & Techniques Used
 
### 1. 🔄 Power Query — Data Transformation
Used Power Query as the **first line of data preparation**, including:
- Importing raw CSV/Excel source files
- Cleaning nulls, fixing data types, renaming columns
- Merging and appending multiple tables
- Creating reusable, refresh-ready query pipelines
### 2. 🗄️ Data Model — Relationship Building
Loaded all cleaned tables into the **Excel Data Model** and established relationships to enable cross-table analysis:
- Fact table: Sales transactions
- Dimension tables: Customers, Products, Markets, Date
- Star schema design for optimal query performance
### 3. ⚙️ Power Pivot — Advanced Analysis Engine
Leveraged Power Pivot to:
- Handle **millions of rows** beyond Excel's sheet limit
- Build a structured, scalable analytical layer
- Connect all reports to a single unified data model
### 4. 🧮 DAX Formulas — Custom Calculations
Wrote DAX measures to power all KPIs, including:
```
Net Sales = SUM(fact_sales[net_sales])
 
Net Sales LY = CALCULATE([Net Sales], SAMEPERIODLASTYEAR(dim_date[date]))
 
YoY Growth % = DIVIDE([Net Sales] - [Net Sales LY], [Net Sales LY], 0)
 
Target Gap = [Net Sales] - [Target Sales]
 
Target Gap % = DIVIDE([Target Gap], [Target Sales], 0)
```
 
### 5. 🎨 Conditional Formatting — Visual Storytelling
Applied conditional formatting to make reports scannable and insight-rich:
- **Color scales** (gold → dark) on sales figures to highlight top performers
- **Red fills** on all negative Target Gap % values
- **Data bars** for quick visual comparison across rows
- Icon sets for YoY performance indicators
---
 
## 📂 Project Structure
 
```
atliq-excel-sales-analytics/
│
├── 📄 Customer_Performance_Report.xlsx
├── 📄 New_Product_Sales_Performance_Report.xlsx
├── 📄 Performance_vs_Target_Report.xlsx
├── 📄 Top_5_Country_Sales_Performance_Analysis.xlsx
├── 📄 Top_10_Product_Analysis_Report.xlsx
│
└── 📖 README.md
```
 
---
 
## 🧰 Tech Stack
 
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=for-the-badge&logo=microsoft&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
 
| Tool | Purpose |
|------|---------|
| Power Query | ETL — Extract, Transform, Load |
| Data Model | Relational schema & table relationships |
| Power Pivot | In-memory analytics engine |
| DAX | Calculated measures & KPIs |
| Conditional Formatting | Visual highlighting & heatmaps |
 
---
 
## 📌 How to Use
 
1. **Clone or download** this repository
2. Open any `.xlsx` file in **Microsoft Excel 2016 or later** (Power Pivot support required)
3. If prompted, click **Enable Content** to allow the Data Model to load
4. Explore the reports — all are connected to a shared data model
5. Use the **slicers/filters** at the top of each report to drill down by Region, Market, or Division
---
 
## 💡 Business Value Delivered
 
✅ Identified fastest-growing customers for prioritized account management  
✅ Revealed every market missed 2021 targets — enabling target recalibration  
✅ Highlighted $176M+ contributed by new product launches in a single year  
✅ Pinpointed top 10 products that drive disproportionate revenue  
✅ Built scalable, refreshable reports — one data refresh updates all dashboards  
 
---
 
## 👤 Author
 
**[Your Name]**  
Aspiring Data Analyst | Excel • SQL • Power BI  
 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat&logo=github)](https://github.com/yourusername)
 
---
 
## ⭐ If you found this helpful...
 
Give this repo a ⭐ — it helps others discover it and motivates me to keep building!
 
---
 
*Data source: AtliQ Hardwares internal sales reports | All values in USD*
