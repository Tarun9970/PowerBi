Executive Sales Performance Dashboard

Data set: Transactional sales data covering orders, customers, products, payment types, and order dates.
The dataset includes revenue, quantities sold, payment methods, and basic customer and product attributes.

Project goal: Build an end to end Power BI sales dashboard that tracks performance, trends, and customer behavior.
The goal is to demonstrate solid data modeling, DAX fundamentals, and clear business focused reporting.

Objectives:
Track total sales, orders, and customers over time
Analyze revenue by product, brand, and payment type
Understand customer purchasing patterns
Identify seasonality and sales trends
Compare year over year performance

Analysis pipeline: 
Explore raw sales and order data
Prepare and clean data for analysis
Build a structured data model
Create measures for sales and trends
Design a clear and interactive dashboard
Core analysis and data preparation

Sales data was cleaned and standardized to ensure consistent dates, prices, and quantities.
Revenue was calculated at order level and aggregated for reporting.
Order dates were used directly for time based analysis due to the absence of a separate date table.
Products and payment types were analyzed as key sales drivers.

Key steps (Power Query):
Cleaned column names and data types
Removed errors and blanks from key fields
Created calculated columns for revenue
Built supporting lookup tables where needed
Ensured data was ready for modeling and visuals

Key steps (Power BI Desktop):
Created measures for total sales, order count, and average order value
Built year over year sales measures
Analyzed sales by product, brand, and payment type
Used slicers for time and category filtering
Designed KPI cards and supporting visuals

Data model

This was my first Dashboard! A simple star schema model was used with sales as the main fact table.
Products, customers, and payment types were connected using one to many relationships.
The model was kept intentionally simple to focus on performance analysis.

