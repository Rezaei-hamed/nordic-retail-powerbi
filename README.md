# Nordic Retail – Power BI Report

## Project Description

This Power BI report provides a comprehensive analysis of sales performance for a Nordic retail business. It is designed to support both strategic decision-making for executives and operational analysis for regional and store managers.

## Target Users

* **Executive Management** – Uses the *Executive Overview* page to monitor total sales, profitability, and business performance over time.
* **Regional & Operations Managers** – Use the *Operation* and *Store Details* pages to analyze performance by region, store, category, and product.

## Key KPIs

* Total Sales
* Profit
* Margin %
* Orders / Quantity
* Sales YTD
* Year-over-Year (YoY %) growth

These metrics provide a clear view of revenue, volume, and profitability.

## Business Value

The report helps users to:

* Identify top- and low-performing regions or stores
* Analyze profitable and underperforming product categories
* Find top products at store level
* Track sales trends over time
* Support data-driven business decisions

## Data Preparation (Power Query)

Data was imported from multiple CSV files and transformed using Power Query:

* Missing values handled (e.g., discounts set to 0)
* Corrected data types for dates and numeric fields
* Cleaned text fields (Trim & Clean)
* Combined product hierarchy into a single product dimension
* Removed duplicates and validated data quality

## Data Model

A **star schema** was implemented:

* Fact table: Sales
* Dimensions: Date, Product, Customer, Store
* Dedicated Date table for time intelligence (YTD, YoY)
* All calculations created using **DAX** and organized in a measure table

## Report Structure & Features

The report consists of three pages:

1. **Executive Overview** – High-level performance summary
2. **Operation** – Regional and category analysis
3. **Store Details** – Detailed store and product insights

Features include:

* KPI cards
* Trend analysis
* Top 10 visuals
* Detailed tables
* Interactive slicers (Date, Region, Category)
* Tooltips showing Profit and Margin % for deeper insights without cluttering the layout
