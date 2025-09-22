# Elavate-task-1-

Sales Data Cleaning
This repository contains a Jupyter notebook (task_1.ipynb) that demonstrates a comprehensive data cleaning process for a sales dataset (sales_data.csv). The project focuses on preparing raw data for analysis by handling missing values, standardizing text, and ensuring data types are correct.

Project Steps
The following data cleaning tasks are performed in the notebook:

Loading Data: The sales_data.csv file is loaded into a pandas DataFrame.

Handling Missing Values: Missing values in numerical columns (PRICEEACH, QUANTITYORDERED, SALES) are filled with the mean of their respective columns. Categorical columns (ADDRESSLINE2, COUNTRY, TERRITORY) are handled by filling with a placeholder or using backward fill.

Removing Duplicates: Duplicate rows are identified and removed to ensure data integrity.

Standardizing Text: Text-based columns like CITY are standardized to a consistent case (e.g., all uppercase). A new column, Full Name, is created by combining the first and last names, and the original name columns are dropped.

Converting Date Formats: The ORDERDATE column is converted to a consistent dd-mm-yyyy format.

Renaming Columns: Column headers are cleaned and standardized to be lowercase with underscores (e.g., ORDERDATE becomes order_date).

Checking and Fixing Data Types: The final step ensures all columns have the correct data types, particularly converting the order_date column to a datetime object for proper analysis.

Requirements
To run the notebook, you will need to have Python and the pandas library installed.

pip install pandas
