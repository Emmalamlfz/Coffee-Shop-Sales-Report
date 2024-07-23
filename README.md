# Coffee Shop Sales Data Analysis Report

## Table of Contents

1. [Demo](#Demo)
2. [Project Background](#project-background)
3. [Data Description](#data-description)
4. [KPI's Requirements](#KPI's-Requirements)
5. [Chart's Requirements](#Chart's-Requirements)
6. [Conclusions and Recommendations](#conclusions-and-recommendations)

## Demo
- **Power BI Dashboard**:[Dashboard Link](https://github.com/Emmalamlfz/Coffee-Shop-Sales-Repor)

![image](https://github.com/user-attachments/assets/0ac908f5-153c-437f-a0ad-41d123a8b144)


## Project Background

This project aims to analyze the sales data of a coffee shop to understand sales trends, customer preferences, and peak sales periods. This analysis will provide data-driven insights to help formulate more effective marketing strategies and operational decisions.

## Data Description

The sales data used in this analysis includes the following fields:
- **transaction_id**: Unique identifier for the transaction
- **transaction_date**: Date of the transaction
- **transaction_time**: Time of the transaction
- **transaction_qty**: Quantity of items in the transaction
- **store_id**: Identifier for the store
- **store_location**: Location of the store
- **product_id**: Unique identifier for the product
- **unit_price**: Price per unit of the product
- **product_category**: Category to which the product belongs
- **product_type**: Type of the product
- **product_detail**: Detailed description of the product

The data covers the period from January 2023 to June 2023.

## KPI's Requirements
1. **Total Sales Analysis**:
   - Calculate the total sales for each respective month
   - Determine the month-on-month increase or decrease in sales
   - Calculate the difference in sales between the selected months and the previous month
     
2. **Total Orders Analysis**:
   - Calculate the total  number of orders for each respective month
   - Determine the month-on-month increase or decrease in the number of orders
   - Calculate the difference in the number of orders between the selected months and the previous month
     
3. **Total Quantity Sold Analysis**:
   - Calculate the total quantity sold for each respective month
   - Determine the month-on-month increase or decrease in total quantity sold
   - Calculate the difference in total quantity sold between the selected months and the previous month


## Chart's Requirements

1. **Calendar Heat Map**:
   - Implement a calendar heat map that dynamically adjusts based on the selected month from a slicer
   - Each day on the calendar will be color-coded to represent sales volume, with darker shades indicating higher sales
   - Implement tooltips to display detailed metrics(Sales,Orders,Quantity)when hovering over a special day
     
2. **Sales Analysis by Weekdays and Weekends**:
   - Segment sales data into weekdays and weekends to analyze performance variations.
   - Provide insights into whether sales patterns differ significantly between weekdays and weekends.
     
3. **Sales Analysis by Store Location**:
   - Visualize sales data by different store locatlons
   - Include month-over-month (MoM) difference metrics based on the selected month in the slicer.
   - Highlight MoM sales increase or decrease for each store location to identify trends.
     
4. **Daily Sales Analysis with Average Line**:
   - Display daily sales for the selected month with a line chart.
   - Incorporate an average line on the chart to represent the average daily sales.
   - Highlight bars exceeding or falling below the average sales to identify exceptional sales days.
     
5. **Sales Analysis by Product Category**:
   - Analyze sales performance across different product categories.
   - Provide insights into which product categories contribute the most to overall sales.
     
6. **Top 10 Products by Sales**:
   - identify and display the top 10 products based on sales volume.
   - Allow users to quickly visualize the best-performing products in terms of sales.
     
7. **Sales Analysis by Days and Hours**:
   - Utilize a heat map visualize sales patterns by days and hours.
   - Implement tooltios to display detailed metrics (Sales,Orders,Quantity) when hovering over a specific day-hour


## Conclusions and Recommendations
Based on the sales data analysis, the following conclusions and recommendations are made:

1. Sales Trend: Sales increase significantly in certain months. It is recommended to increase promotional activities during these months.
2. Peak Periods: Daily sales peak in the morning and afternoon. It is recommended to increase staffing and inventory during these periods.
3. Best-Selling Products: Latte and Americano are the best-selling products. Consider offering related promotions.
4. Customer Preferences: Customers purchase more frequently in the morning and afternoon. Special promotions can be launched during these times.

This analysis provides data-driven insights to support more effective marketing strategies and operational optimizations.













