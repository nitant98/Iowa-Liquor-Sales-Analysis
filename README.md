# Iowa Liquor Sales Analysis

## Overview
This project focuses on analyzing Iowa’s liquor sales data by creating a data warehouse (DW) for optimized reporting and business intelligence (BI). The project involves three main phases: data profiling and ETL, dimensional modeling, and business analytics to answer critical questions about sales trends, gross profit, and sales distribution across different locations and time periods.

## Project Objectives
1. **Data Profiling and ETL**:
   - Cleansed and loaded raw data into staging tables.
   - Used **Alteryx** and **Talend** to perform ETL on DBMS for staging tables.

2. **Dimensional Modeling**:
   - Designed a dimensional data model to support analytical reporting.
   - Developed a schema to facilitate queries on various sales metrics by dimensions like location, product, and time.

3. **Business Analytics and Visualization**:
   - Answered predefined business questions through SQL queries.
   - Visualized results with dashboards in **Tableau** and **Power BI**.

## Data Sources
1. **Liquor Sales Data**: Monthly and yearly sales data from 2012 to 2022.
2. **Product Data**: Details on products sold, including item categories and vendors.
3. **Store Data**: Store locations and demographic information.
4. **Population Data**: City and county population statistics by year.

## Project Phases

### Part 1: Data Profiling and Staging
   - **Data Profiling**: Profiled datasets (`Iowa_Liquor_Sales`, `Iowa_Liquor_Products`, `Iowa_Liquor_Stores`) using **Alteryx**.
   - **Data Loading (ETL)**: 
     - Load data into staging tables across two separate DBMS (one for Alteryx, one for Talend).
     - Key staging tables:
       - `stg_iowa_liquor_sales`
       - `stg_iowa_liquor_products`
       - `stg_iowa_liquor_stores`
       - `stg_iowa_city_population_by_year`
       - `stg_iowa_county_population_by_year`
   - **Data Cleansing**: Defined cleansing steps, handled inconsistencies, and saved cleansed data in separate tables.

### Part 2: Dimensional Modeling and Integration Schema
   - **Key Business Questions**:
      1. **Sales Analysis**:
         - Total sales ($) by year, city, store, category, and vendor.
         - Sales volume in gallons and bottles.
         - Gross profit by sales cost and retail price.
         - Sales per capita across different regions.
      
      2. **Temporal Analysis**:
         - Monthly and yearly sales trends.
         - Year-over-year comparison of sales volume and profit.
      
      3. **Geographical Analysis**:
         - Top 10 cities, counties, and stores by sales volume.
         - Sales distribution across urban and rural areas.
         - 
   - **Dimensional Model Creation**: Based on the business requirements created a schema using **ER/Studio**.
   - **SQL DDL Scripting**: Generated DDL scripts for dimensional tables in the database.
   - **Load Integration Schema**: Loaded data from staging into the dimensional model for analytical queries.
     
![Dimensional Model](https://github.com/user-attachments/assets/f4b7dd90-4f89-4191-8615-d31e23a486f8)

### Part 3: Business Intelligence and Reporting           
   - **SQL Queries**: Generated reports for:
     - Sales ($, volume, per capita) by year, city, county, store, category, and vendor.
     - Gross profit by sales cost and retail price.
   - **Dashboard Development**:
     - **Power BI** and **Tableau** dashboards to visualize top-performing stores, cities, categories, and trends.

## Tools and Technologies
- **ETL Tools**: **Alteryx** and **Talend** for data transformation.
- **Database Management**: **Azure SQL**, **SQL Server**
- **Data Modeling**: **ER/Studio** for dimensional modeling.
- **Business Intelligence**: **Tableau** and **Power BI** for dashboards and data visualization.


