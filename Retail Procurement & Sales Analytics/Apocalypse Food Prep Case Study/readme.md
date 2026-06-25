# Power BI Retail Procurement & Sales Analytics
## (Apocalypse Food Prep Case Study)

A Power BI project that transforms messy Excel-style data into an interactive analytics model for procurement, sales, profitability, and customer behavior analysis.

## Problem Statement

Raw spreadsheet data is often messy, semi-structured, and difficult to analyze directly. In this project, the source data contains purchase records, product data, customer data, and pivot-table style formatting that must be cleaned before meaningful analysis can begin.

The objective is to:
- identify the cheapest store overall,
- determine which store is best for each product,
- analyze customer purchasing behavior,
- calculate product-level profitability,
- and explore time-based patterns in sales.

## What This Project Solves

This project demonstrates how to turn unstructured Excel data into a decision-ready Power BI dashboard.

It answers questions such as:
- Where should I buy each product at the lowest cost?
- Which products are most expensive or most cost-effective by store?
- Which customers place the most orders?
- Which products generate the most profit?
- How do purchases vary by day of week or time period?

## How It Works

### 1. Data Cleaning in Power Query
- Removed null rows and subtotal/grand total rows
- Renamed columns for clarity
- Fixed data types
- Unpivoted date columns to create an analysis-friendly structure

### 2. Data Modeling
- Built relationships between sales, customer, and product tables
- Configured cardinality and cross-filter direction properly
- Ensured the model supports accurate reporting and filtering

### 3. DAX Measures and Calculated Columns
- Count of sales
- Total units sold
- Profit calculations
- Profit per row using iterator logic
- Day-of-week grouping
- Order size classification

### 4. Visual Analytics
- Store comparison charts
- Product-level price comparison
- Customer purchase breakdown
- Profit and sales summaries
- Drill-down enabled views for deeper exploration

## Key Insights
- The overall cheapest store was identified through total spend comparison.
- Different products can be cheapest at different stores.
- Customer and product relationships unlock more accurate reporting.
- SUMX is required when calculation must happen row-by-row.
- Drill-down makes executive dashboards more useful and interactive.

## Files in This Repository
- `data/` → source datasets
- `powerbi/` → Power BI report files (`.pbix`)
- `screenshots/` → dashboard previews
- `README.md` → project overview

## Tools Used
- Power BI Desktop
- Power Query
- DAX
- Excel
- Data modeling / relationships

## Project Structure
```text
├── data
│   ├── apocalypse_food_prep.xlsx
│   ├── apocalypse_sales.xlsx
│   ├── customer_information.xlsx
│   └── purchase_tracker.xlsx
├── powerbi
│   └── apocalypse_food_prep_dashboard.pbix
├── screenshots
│   ├── overview.png
│   ├── store_comparison.png
│   └── customer_breakdown.png
└── README.md
