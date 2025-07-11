# Swiggy-Delivery-Executive-Performance-Analytics


This project simulates and analyzes delivery executive performance data for a Swiggy-like platform. It focuses on building a stakeholder-ready Excel-based dashboard to support weekly reward allocation and performance tracking decisions.

##  Problem Statement

Sales managers wanted to identify the top 5 delivery executives weekly in each city based on:
- Total orders delivered
- Average customer rating
- Average delivery time (lower is better)

Additionally, the output had to be presented in Excel in a way that allowed easy filtering and reward decision-making.

##  Tools Used

-  Python (Jupyter Notebook): For synthetic data generation, normalization, scoring logic, and Excel writing.
-  Microsoft Excel: For data cleaning (Power Query), automation, and stakeholder-facing dashboards.
-  Libraries: pandas, numpy, sklearn (MinMaxScaler), datetime

##  Dataset

A synthetic dataset of 1,00,000+ rows was created using Python, containing:
- Unique Order IDs
- Delivery Partner ID (each mapped to a fixed city)
- City, Order Value, Quantity, Timestamps (order/pickup/delivery)
- Customer Ratings

All data points were designed based on real-world Swiggy order behavior.

## Task 1: Top 5 Delivery Executives per City per Week

- Delivery time (mins) calculated from timestamps
- Scoring logic:
  - Total Orders (30%)
  - Avg Rating (30%)
  - Avg Delivery Time (40%) → reverse scaled (lower is better)
- Used Min-Max Normalization
- Final output: An Excel file with a separate sheet for each week, listing Top 5 performers per city

 File: `Top_5_Delivery_Executives_Scored_4weeks.xlsx`

##  Task 2: Interactive Excel Framework (City-wise Filter)

- Final output sheet redesigned using:
  - Power Query (to reshape & clean data)
  - Pivot Tables
  - Filters and Slicers (city-level)
- Made it easy for Sales Managers to select any city and view top performers instantly.

 File: `top5_master_by_city_week_filter.xlsx`

##  Impact

- Enabled Excel-only reward dashboards for business stakeholders
- No need for Python/SQL at the stakeholder level
- Smooth handling of 1 lakh+ rows using Excel optimization techniques

## Output Snapshots

- Excel-based Top 5 Executive Report (Week-wise Sheets)
- City Filter + Pivot Table for instant insights
