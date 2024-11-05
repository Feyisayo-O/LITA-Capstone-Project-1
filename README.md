# Sales Performance Analysis for a Retail Store

## Table of Contents
1. [Project Overview](#project-overview)
2. [Tools Used](#tools-used)
3. [Dataset Description](#dataset-description)
4. [Steps Undertaken](#steps-undertaken)
   - [Data Preparation](#data-preparation)
   - [Excel Analysis](#excel-analysis)
   - [SQL Analysis](#sql-analysis)
   - [Power BI Dashboard](#power-bi-dashboard)
5. [Key Insights](#key-insights)
6. [Acknowledgements](#acknowledgements)

## Project Overview
This project involves analyzing the sales performance of a retail store to uncover key insights, including top-selling products, regional performance, and monthly sales trends. The goal is to produce an interactive Power BI dashboard that highlights these findings.

## Tools Used
- **Excel**: For initial data exploration and analysis.
- **SQL Server**: For querying and extracting insights from the dataset.
- **Power BI**: This was used to create an interactive dashboard.

## Dataset Description
- **Source**: Excel file
- **Description**: The sheet contains sales data with column headers namely Order ID, Customer ID, Product, Region, Order date, Quantity, and Unit Price. There are 50000 rows of data.

## Steps Undertaken

### Data Preparation
- **Loaded Data**: Imported the dataset into Excel and SQL Server.
- **Data Cleaning**: Checked for missing values and performed necessary data cleaning.


### Excel Analysis
- **Initial Exploration**: Performed an initial exploration of the sales data.
![Excel Data S](https://github.com/user-attachments/assets/6fe096b3-a99e-464a-90f2-f6a1d2cc115a)
- **Calculations**: 
  - Total revenue.
- **Code/Formula**: 
  ```excel
  =Quantity*UnitPrice
- **Pivot Tables**: Created pivot tables to summarize total sales and revenue by product, region, and month.
![Excel Analysis](https://github.com/user-attachments/assets/0687ccd0-6ce9-4862-a605-7fe4a437a736)

### SQL Analysis
- **Setup**: Loaded the dataset into SQL Server.
- **Queries Executed**: 
  - Total sales for each product category.
  - Number of sales transactions in each region.
  - Highest-selling product by total sales value.
  - Total revenue per product.
  - Monthly sales totals for the current year.
  - Top 5 customers by total purchase amount.
  - Percentage of total sales contributed by each region.
- **Code example**: Total sales for each product category.
 ```sql
select Product, SUM(Quantity) as Total_Sales_Category from Sales Data
group by Product
 ```
![SalesSql1](https://github.com/user-attachments/assets/c9237b8f-58c6-44e8-9e19-1f08bf16b224)
![SalesSql2](https://github.com/user-attachments/assets/559cd6a9-b4d1-4fa5-8aaf-4b35646d2c84)

### Power BI Dashboard
- **Dashboard Creation**: Developed an interactive dashboard visualizing key sales insights.
- **Features**: Included sales overview, top-performing products, and regional breakdowns.
![Power BI Sales](https://github.com/user-attachments/assets/18561428-c669-40ce-8d87-0bad38fd9c11)

## Key Insights
  - The top-selling product is Hat, contributing 23.19% to total sales and was purchased mostly in the East region.
  - The South region generated the highest revenue at $4,675,000 with 122,500 sales transactions.
  - The monthly sales had no particular trend as it fluctuated. The most sales recorded were in February and July. The least sales recorded were in May and December.
  - A total of $10,587,500 was generated in revenue with 345,000 sales recorded.

Below are the dashboards for the years 2023 and 2024 respectively.
![Power BI Sales 1](https://github.com/user-attachments/assets/8e58b47d-6fb5-4f10-85d3-f4eed5c55bc2)
![Power BI Sales 2](https://github.com/user-attachments/assets/e7e6050f-8fb8-4240-9945-d69a9344b23d)

## Acknowledgements
  - Special thanks to the instructors at The Incubator Hub for guidance throughout the learning period.









