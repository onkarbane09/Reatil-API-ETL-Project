# Reatil-API-ETL-Project
ETL project that extracts product and order data from a public Retail API, transforms it using Python, and loads it into a SQL Server database for analysis.

This project is a complete ETL (Extract, Transform, Load) pipeline built using Python and SQL Server. It extracts product and order data from the Fake Store API (https://fakestoreapi.com/), transforms the data into clean and structured CSV files, and loads it into a SQL Server database for analysis.

The project is organized into two main Python scripts located in the `etl/` folder:

1. `extract_from_api.py`: This script uses the `requests` and `pandas` libraries to fetch data from the API endpoints for products and orders. It flattens nested JSON structures (like the product `rating` and order `items`), and then saves the cleaned data into CSV files inside the `data/` folder.

2. `load_to_sqlserver.py`: This script connects to a local SQL Server instance using `pyodbc`, creates three tables (`products`, `orders`, and `order_items`) if they don’t already exist, and loads the CSV data into those tables. It includes error handling and data cleaning steps (e.g., unpacking nested values, type conversions) before loading the data.

By completing this project, I learned how to:
- Work with public REST APIs and nested JSON data
- Perform data transformation and normalization with pandas
- Handle API-to-database workflows with proper ETL logic
- Use pyodbc to interact with SQL Server in Python
- Structure a project for real-world data workflows

This is a beginner-friendly data engineering project and can serve as a strong portfolio piece showing practical skills in API integration, data cleaning, and relational database handling.
