# Retail Sales Project

This project analyzes about retail sales data using Databricks for data processing and Power BI for visualization. The original data can be found [here](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset)

## Dataset Description

- Transaction ID: A unique identifier for each transaction
- Date: The date when the transaction occurred
- Customer ID: A unique identifier for each customer
- Gender: The gender of the customer
- Age: The age of the customer
- Product Category: The category of the purchased product
- Quantity: The number of units purchased
- Price per Unit: The price of one unit of the product
- Total Amount: The total monetary value of the transaction

## Architecture

The project utilizes the Databricks Medallion Architecture using Delta Lake to implement a multi-layer data pipeline

Raw Data (CSV file) → Bronze (Raw Tables) → Silver (Cleaned & Standardized Data) → Gold (Business-Ready Data) → Power BI (Dashboards)

## Technologies Used

Databricks, Power BI, Python, PySpark, SQL

## Databricks

In "Load Data" the file is loaded, the columns are renamed and the Bronze table is created. In "Cleaning", the types of columns are changed where needed, there's a check for null values and the Silver table is created. In "Gold", multiple tables are made for visualization in PowerBI

## PowerBI

Pages:
1. Revenue and Units Sold per Product Category
2. Customer Insight
3. Revenue by Product Category, Age Group, and Gender 
