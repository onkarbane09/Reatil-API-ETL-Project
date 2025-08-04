# Reatil-API-ETL-Project
ETL project that extracts product and order data from a public Retail API, transforms it using Python, and loads it into a SQL Server database for analysis.

This project is a complete ETL (Extract, Transform, Load) pipeline built using Python and SQL Server. It extracts product and order data from the Fake Store API (https://fakestoreapi.com/), transforms the data into clean and structured CSV files, and loads it into a SQL Server database for analysis.

The project is organized into two main Python scripts located in the `etl/` folder:

Data Extraction and Cleaning: Fetched product and order data from an external API, then cleaned and normalized the data using data manipulation techniques. This included flattening nested JSON structures such as product ratings and order items, followed by saving the cleaned datasets to CSV format.

Data Loading into SQL Server: Connected to a local SQL Server, created structured tables (products, orders, and order_items) with appropriate schema definitions, and loaded the cleaned data into these tables. Steps included error handling, converting data types, and unpacking nested values to align with the database structure.

By completing this project, I learned how to:
- Work with public REST APIs and nested JSON data
- Perform data transformation and normalization with pandas
- Handle API-to-database workflows with proper ETL logic
- Use pyodbc to interact with SQL Server in Python
- Structure a project for real-world data workflows

This is a beginner-friendly data engineering project and can serve as a strong portfolio piece showing practical skills in API integration, data cleaning, and relational database handling.
