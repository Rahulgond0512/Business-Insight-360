# Business Insights 360 – Power BI Dashboard Project

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow)
![DAX](https://img.shields.io/badge/Skill-DAX-blue)
![Power Query](https://img.shields.io/badge/Skill-Power%20Query-green)
![Data Modeling](https://img.shields.io/badge/Skill-Data%20Modeling-orange)
![KPI Dashboard](https://img.shields.io/badge/Type-KPI%20Dashboard-purple)

## Project Overview
This is an end-to-end Power BI dashboard project built to analyze business performance across multiple functional areas including Finance, Sales, Marketing, Supply Chain, and Executive reporting.

The objective of this project is to provide actionable business insights using KPI tracking, profitability analysis, customer insights, product performance, and forecast accuracy.

 View the live interactive dashboard here:
 [Live Report Link](https://www.novypro.com/project/business-insights-360-233)
 
---

## Business Problem

Atliq Hardware is one of the fastest-growing companies in the electronic goods market.

However, the company faced a major loss in the Latin America region because some important decisions were made only based on surveys and intuition.

This made the company realize the importance of data-driven decision-making.

Earlier, they were using Excel for analysis, but as the company expanded, Excel was no longer enough.

So, they hired a data analytics team to bring transparency into the data and support better business decisions.
Another major challenge for the company is competition from Dell, which is growing rapidly.

Dell has a strong data analytics team that analyzes customer demographics, buying patterns, and income levels to improve decision-making.
To stay competitive, Atliq Hardware also needs to build a strong analytics-driven approach.

---

## Business Objective

Develop an interactive Power BI dashboard to support data-driven decision-making across key business functions.

The dashboard is designed to provide insights in the following sequence:

- **Finance** – revenue, profit, gross margin, and financial trends
- **Sales** – customer and product sales performance analysis
- **Marketing** – market, region, and customer behavior insights
- **Supply Chain** – forecast accuracy, inventory, and operational performance
- **Executive** – overall business performance and KPI summary
  
---

## Tools & Skills Used
- MySQL
- Power BI
- DAX
- Power Query
- Data Modeling
- KPI Dashboard Design
- Business Storytelling
- Interactive Filters and Slicers



## Dashboard Views
- Home Page
- Finance 
- Sales 
- Marketing 
- Supply Chain 
- Executive 

---

## Key KPIs
- Net Sales $
- Gross Margin %
- Net Profit %
- Forecast Accuracy %
- Net Error
- Absolute Error

---

## Dataset Understanding

Before starting the analysis, it is important to understand what data is available and how it supports business decision-making.

Database Used

- MySQL Database: "gdb041", "gdb056"
- Additional Source Files: Excel files for Target Sales, Market Share, and Operating Expenses

---

Data Structure

The dataset uses both star schema and snown flake schema methods.

- Dimension Tables: Static descriptive information
- Fact Tables: Transactional and numerical business data

---

## Dimension Tables

"dim_customer"

Contains customer-level static details.

- 82 distinct customers across all markets (updated)
- 27 distinct markets
- 2 platforms
  - Brick & Mortar- Offline retail stores 
  - E-commerce- Online platforms 
- 3 channels
  - Retailer (eg. Croma, Vijay Sales, Amazon, Flipkart)
  - Direct (eg. AtliQ Exclusive, AtliQ Estore)
  - Distributor (eg. Neptune)

---

"dim_market"

Contains geography and market hierarchy details.

- 27 markets
- 7 sub-zones
- 4 regions
  - APAC
  - EU
  - LATAM
  - NA / Other

---

"dim_product"

Contains product details such as

- Divisions:
  - P & A
  - N & S
  - PC 
- Segments:
  - Peripherals
  - Accessories
  - Notebook
  - Desktop
  - Networking
  - Storage
- 14 categories
- Multiple variants for the same product

---

"dim_date"

The dataset did not have a date table, so I created it using DAX in Power BI.
The table was created using the start date and end date from "fact_sales_monthly".
I also created a fiscal year column for time-based business analysis.

---

Fact Tables

"fact_forecast_monthly"

Contains customer demand forecast data.

Used for:

- demand planning
- warehouse optimization
- customer satisfaction improvement

The table is denormalized for analytical reporting.

Key metric:

- "forecast_quantity"

---

"fact_sales_monthly"

Contains actual sales transaction data.

Key metric:

- "sold_quantity"

This table is used to compare:

- forecast vs actual sales
- sales trends
- customer performance

---

Additional Financial Tables ("gdb056")

- "freight_cost"
- "gross_price"
- "manufacturing_cost"
- "pre_invoice_deductions"
- "post_invoice_deductions"

These tables were used for financial and profitability analysis.

---

Additional Excel Files Used

Along with MySQL database tables, the following Excel files were integrated into the Power BI data model:

- Target Sales
- Market Share
- Operating Expenses

These files were connected and related using data modeling relationships in Power BI.

This helped in building a complete business performance view across:

- sales
- targets
- expenses
- market growth
- profitability

---

## Data Model

The dashboard is built using a well-structured Power BI data model with fact and dimension tables.

The model supports accurate KPI calculations, time intelligence analysis, and interactive cross-filtering across all dashboard views.

<img src="Data%20model.png" width="900"/>

---

## Dashboard Screenshots

### Home Page
<img src="./Business%20Insight%20360%20Home%20Page.png" width="900"/>

### Finance Dashboard
<img src="./Business%20Insight%20360%20Finance%20Page.png" width="900"/>

### Sales Dashboard
<img src="./Business%20Insight%20360%20Sales%20Page.png" width="900"/>

### Marketing Dashboard
<img src="./Business%20Insight%20360%20Marketing%20Page.png" width="900"/>

### Supply Chain Dashboard
<img src="./Business%20Insight%20360%20Supply%20Chain%20Page.png" width="900"/>

### Executive Dashboard
<img src="./Business%20Insight%20360%20Executive%20Page.png" width="900"/>

---

## Video Walkthrough
🎥 Full Dashboard Demo : [Watch on YouTube](https://youtu.be/rBdJJ9JUV10)

## Project File
The complete Business Insights 360 project file (.pbix) is available in this repository for reference and learning purposes.
It includes :
- Data model
- DAX measures
- Interactive dashboard pages
- KPI calculations
- Business insight visuals
  
---

## Project Outcome
By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
