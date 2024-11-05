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
6. [Screenshots](#screenshots)

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
- **Code**: 
  ```sql
select Product, SUM(Quantity) as Total_Sales_Category from Sales Data
group by Product;
  ```

![SQL S 1](https://github.com/user-attachments/assets/be62340c-b379-4253-a160-ceeda9ce7dc9)

![SQL S 2](https://github.com/user-attachments/assets/98627f75-f55c-42f4-9146-9858060a972e)






