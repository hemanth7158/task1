# 🧹 Task 1 - Data Cleaning and Preprocessing

## 📊 Dataset Overview
This project uses the sales_data_sample.csv dataset, which contains sales transaction records from a fictitious company. The dataset includes information such as order dates, product lines, quantities ordered, prices, customer details, and order statuses. It was downloaded from [Kaggle](https://www.kaggle.com/), and is used here to demonstrate practical data cleaning techniques.

## 🎯 Objective
To clean and preprocess the raw dataset by:
- Identifying and handling missing values
- Removing duplicate records
- Standardizing inconsistent text and formatting
- Converting date columns to appropriate datetime formats
- Fixing column names and data types for better usability

These steps ensure that the dataset is reliable, structured, and ready for further analysis or machine learning workflows.

## 🧪 Data Cleaning Steps Performed
1. *Missing Values:*
   - Checked for null values using .isnull().sum()
   - Dropped rows with missing data using .dropna() to maintain data integrity

2. *Duplicate Records:*
   - Identified and removed exact duplicate rows using .drop_duplicates()

3. *Column Name Cleaning:*
   - Standardized column names by converting them to lowercase and replacing spaces with underscores (e.g., Order Date → order_date)

4. *Text Standardization:*
   - Cleaned inconsistent values in columns such as status and productline by applying .str.upper() and .str.title() respectively

5. *Date Format Correction:*
   - Converted the orderdate column from string to datetime format using pd.to_datetime()

6. *Data Type Conversion:*
   - Ensured priceeach is treated as float and quantityordered as int for numerical operations

## 🧰 Tools & Libraries Used
- Python
- Pandas Library (for data manipulation and preprocessing)

## 📁 Output
The cleaned dataset is saved as:
- sales_data_cleaned.csv

This dataset is now ready for exploratory data analysis (EDA), data visualization, or feeding into a machine learning pipeline.

## 🧠 What I Learned
- Practical application of core Pandas functions for data cleaning
- Importance of consistent formatting in real-world datasets
- Debugging file encoding issues (UnicodeDecodeError) and resolving them using encoding='ISO-8859-1'
- Hands-on experience preparing raw data for further use

## 📸 Screenshots
Add relevant screenshots of your code output, terminal, or visualizations here (optional but helpful)

## 🔗 References
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Kaggle Dataset](https://www.kaggle.com/datasets/)

## ✅ Status
Task 1 complete and submitted as part of the Data Analyst Internship assignment.
