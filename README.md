# Reatil-API-ETL-Project
ETL project that extracts product and order data from a public Retail API, transforms it using Python, and loads it into a SQL Server database for analysis.

This project is a complete ETL (Extract, Transform, Load) pipeline built using Python and SQL Server. It extracts product and order data and transforms the data into clean and structured CSV files, and loads it into a SQL Server database for analysis.

Data Extraction and Cleaning: Fetched product and order data from an external API, then cleaned and normalized the data using data manipulation techniques. This included flattening nested JSON structures such as product ratings and order items, followed by saving the cleaned datasets to CSV format.

Data Loading into SQL Server: Connected to a local SQL Server, created structured tables (products, orders, and order_items) with appropriate schema definitions, and loaded the cleaned data into these tables. Steps included error handling, converting data types, and unpacking nested values to align with the database structure.

Skills -
- Work with public REST APIs and nested JSON data
- Perform data transformation and normalization with pandas
- Handle API-to-database workflows with proper ETL logic
- Use pyodbc to interact with SQL Server in Python
- Structure a project for real-world data workflows

