# Power BI Assignment 1 - E-Commerce Sales Analysis

## Overview

This project is based on Power BI Assignment 1, Data Transformation & Data Modeling.

The project analyzes e-commerce sales data using Power BI and demonstrates data transformation, data cleaning, data merging, aggregation, and data modeling.

## Dataset

The project uses three datasets:

- List of Orders
- Order Details
- Sales Target

## Data Transformation

The following transformations were performed:

- Restricted List of Orders to the first 500 rows
- Converted Order Date to Date data type
- Converted Amount and Target to Fixed Decimal Number
- Converted CustomerName to Proper Case
- Created Location using City and State
- Created Profit Margin using Profit / Amount
- Created Profit Status based on Profit values

### Profit Status

| Profit Condition | Status |
|---|---|
| Profit < 0 | Loss |
| Profit = 0 | Break-Even |
| Profit > 0 | Profit |

## Data Merging

List of Orders and Order Details were merged using:

`Order ID`

The merged table was named:

`Orders Data`

## Data Cleaning

- Missing values were checked
- Duplicate data was checked
- Appropriate handling strategies were considered

## Sorting and Filtering

- Orders were sorted by Order Date in descending order
- State filtering was performed for regional analysis

## Data Aggregation

The following aggregations were performed:

- Count of Order ID
- Average Profit by Category
- Total Amount by Sub-Category
- Total Target by Month

## Data Modeling

The following relationships were created:

### Order ID Relationship

`List of Orders[Order ID]`

↓

`Order Details[Order ID]`

### Category Relationship

`Order Details[Category]`

↓

`Sales target[Category]`

Both relationships were configured as active.

## Tools Used

- Power BI Desktop
- Power Query
- DAX/Power BI Data Modeling

## Project File

The main Power BI report is:

`PowerBI_Assignment_1_ECommerce_Sales.pbix`
