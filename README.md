# Finance-and-Supply-Chain-Analysis
Conducted an in-depth SQL-based analysis of Finance and supply chain data for ATLIQ Hardware.
ATLIQ Hardware SQL Analytics Project
Project Overview

This project analyzes sales and supply chain performance for ATLIQ Hardware, focusing on finance analytics and supply chain analytics. Key areas include calculating gross prices, applying invoice discounts, deriving net sales, and evaluating forecast accuracy. The project leverages SQL views, procedures, and functions to simplify complex business queries and support strategic decision-making.
Tech Stack

    Database: MySQL
    SQL Techniques: Views, Stored Procedures, Functions, Common Table Expressions (CTEs)

Project Structure
1. Finance Analytics

This section provides a detailed financial analysis by calculating metrics like gross prices, pre- and post-invoice discounts, and net sales.

    Views:
        sales_pre_invoice_discount: Calculates pre-invoice discounts based on sales data.
        post_inv_discount: Derives the net invoice sales by applying pre-invoice discounts and calculating post-invoice discount percentages.
        net_sales: Provides final net sales figures after both pre- and post-invoice discounts, aiding revenue analysis.
    Use Case: The net_sales view aggregates net sales by product, customer, and date, making it easier to query revenue-related insights.

2. Top Customer and Market Analysis

SQL queries identify the top-performing customers and markets based on net sales for the fiscal year 2021:

    Top 5 Customers by Net Sales: Retrieves the highest-grossing customers.
    Top 5 Markets by Net Sales: Highlights the most profitable markets.

3. Supply Chain Analytics

This section assesses forecasting accuracy by analyzing actual sales versus forecast data, identifying improvement areas in demand forecasting.

    Tables:
        fact_actuals_est: Combines actual and forecasted sales data for analysis.
    Forecast Error Table: Calculates metrics such as net error, absolute error, and percentage errors (net and absolute) to assess forecasting accuracy.
    Customer Forecast Accuracy Comparison:
        Compares forecast accuracy between 2020 and 2021, highlighting customers with declining accuracy.

Key SQL Components

    Function: get_fiscal_year – Calculates the fiscal year based on a given date.
    Stored Procedure: get_badge – Assigns sales performance badges based on total sales quantity for specific markets and fiscal years.
    Stored Procedure: Top Products by Sales – Retrieves the top n products by quantity sold for each division.

Insights and Outcomes

    Finance Analytics: Simplifies the financial analysis process by abstracting complex discount calculations and providing quick access to revenue metrics.
    Supply Chain Analytics: Highlights customers with decreased forecast accuracy, providing valuable insights into demand forecasting and inventory management needs.

How to Use

    Clone the Repository:

    bash

    git clone https://github.com/YourUsername/ATLIQ-Hardware-SQL-Analytics.git

    Database Setup: Load the provided database schema and sample data into MySQL.
    Execute Queries: Run the SQL scripts for views, stored procedures, and queries in the respective order mentioned in the project structure.

Project Acknowledgment

This project was completed as part of the SQL Beginner to Advanced for Data Professionals certification from Codebasics.
