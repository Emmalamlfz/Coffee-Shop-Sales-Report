# Coffee Shop Sales Data Analysis Report
![image](https://github.com/user-attachments/assets/0807e23c-a6d6-419d-b9e1-8f3695cd3c06)


## Table of Contents

1. [Demo](#Demo)
2. [Project Background](#project-background)
3. [Data Description](#data-description)
4. [KPI's Requirements](#KPI's-Requirements)
5. [Chart's Requirements](#Chart's-Requirements)
6. [Conclusions and Recommendations](#conclusions-and-recommendations)

## Demo
- **Dynamic Power BI Dashboard**: [Dashboard Link](https://github.com/Emmalamlfz/Coffee-Shop-Sales-Report/blob/main/Coffee%20shop%20sales.pbix)

*Static screenshot is as follows:*
![image](https://github.com/user-attachments/assets/0ac908f5-153c-437f-a0ad-41d123a8b144)


## Project Background

This project aims to analyze the sales data of a coffee shop to understand sales trends, customer preferences, and peak sales periods. This analysis will provide data-driven insights to help formulate more effective marketing strategies and operational decisions.

## Data Description
- **Data Set**: [Data Set Link](https://github.com/Emmalamlfz/Coffee-Shop-Sales-Report/blob/main/Coffee%20Shop%20Sales.xlsx)

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

## Data Analysis
Here are some interesting features in PowerBI to work with:
1. **Tooltip**: Tooltips provide additional information when users hover over data points, offering more context or insights. You can create detailed tooltips that display additional visuals or text.

2. **Conditional Formatting**: Apply conditional formatting to your visuals to dynamically change their appearance based on data values. This helps in highlighting trends, performance metrics, or outliers effectively.

3. **Data Model**: A well-structured data model improves performance and allows for more complex analyses.
   
   - *Date Dimension Table*
     - *Completely self-created, not part of the original dataset: The date dimension table is completely self-created and is not part of the original dataset. This approach provides greater flexibility and consistency, making time-related analysis more convenient and accurate.*
     - *Flexibility and Consistency: Having a date dimension table allows for easy analysis across various time dimensions, such as by day, week, month, quarter, and year.*
       
   - *Relationship Establishment*
     - *Relationship between Transactions Table and Date Table: The relationship between the Transactions table and the Date Table is established through the transaction_date and Date fields. This relationship type is many-to-one (multiple transaction records corresponding to one date), which is a common pattern between fact and dimension tables.*
     - *Many-to-One Relationship: The many-to-one relationship ensures accurate filtering and aggregation of data across the time dimension, guaranteeing the correctness of time-related analyses.*
     
![image](https://github.com/user-attachments/assets/cc3d4f15-f9a1-4f6a-acc9-bd9c4c358929)

5. **Measure**: Measures are powerful calculations used in Power BI to perform dynamic data aggregation and analysis. They are written using DAX and provide the ability to create flexible and reusable calculations.

   - **Aggregation**: Measures can perform various aggregation operations like SUM, AVERAGE, COUNT, MIN, and MAX. For example, you can create a measure to calculate the total sales amount.
   - **Dynamic Calculation**: Measures adjust their calculations based on the context of the report, such as filters and slicers. This means they dynamically update to reflect the data being viewed.
   - **Complex Calculations**: Measures allow for complex calculations and logic. You can create measures for year-over-year growth, percentage changes, and more.
   - **Key Performance Indicators (KPIs)**: Measures can be used to create KPIs, helping you track and evaluate business performance. For instance, you can create a measure to calculate the percentage of targets achieved.
   - **Conditional Formatting**: Measures can serve as the basis for conditional formatting, allowing you to color-code data based on specific conditions. For example, you can highlight sales amounts that exceed a certain threshold.

*An example for calculating Total Sales:*
```dax
Total Sales = SUM(Sales[Amount])
```

*Another DAX example for calculating year-over-year growth:*
```dax
YoY Growth = 
    IF(
        ISBLANK([Total Sales]),
        BLANK(),
        ([Total Sales] - [Total Sales Last Year]) / [Total Sales Last Year]
    )
```

## Conclusions and Recommendations
Based on the sales data analysis, the following conclusions and recommendations are made:

1. Sales Trend: Sales increase significantly in certain months. It is recommended to increase promotional activities during these months.
2. Peak Periods: Daily sales peak in the morning and afternoon. It is recommended to increase staffing and inventory during these periods.
3. Best-Selling Products: Latte and Americano are the best-selling products. Consider offering related promotions.
4. Customer Preferences: Customers purchase more frequently in the morning and afternoon. Special promotions can be launched during these times.













