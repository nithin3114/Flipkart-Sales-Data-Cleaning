# Flipkart Sales Data Cleaning Project

## Overview
This project involves cleaning and preparing a large Flipkart sales dataset for analysis.  
The original dataset was over **4.5 GB** and contained **46 million rows**, so a smaller subset of **500,000 rows** was used for processing in Python (Jupyter Notebook through PyCharm).

## Objective
To clean and standardize the dataset by handling missing values, duplicates, inconsistent formats, and unnecessary columns — ensuring a reliable dataset for data analysis.

## Steps Performed
- Read the dataset using **pandas** and extracted the first 500,000 rows.
- **Removed duplicate rows** using `.drop_duplicates()`.
- **Handled missing data** by removing rows where `total_weighted_landing_price` was null (less than 5% of data affected).
- **Standardized city names**: merged `HR-NCR` into `Delhi` and converted all city names to uppercase.
- **Converted date format** to `dd-mm-yyyy` and renamed the date column.
- **Cleaned column headers** by making them uppercase and removing spaces.
- **Dropped unnecessary columns** such as `UNNAMED: 0.2`, `UNNAMED: 0.1`, and `UNNAMED: 0`.
- **Verified data types** for correctness (dates as datetime, numbers as integers/floats).
- Saved the cleaned dataset as `Sales_sample_cleaned.csv`.

## Files in This Repository
- `Task1-Sales_Data.ipynb`: Jupyter notebook with all processing steps.
- `Sales_sample.csv`: Sample of raw data (500,000 rows from the main dataset).
- `Sales_sample_cleaned.csv`: Final cleaned dataset.
- `summary.md`: Short summary of data cleaning changes.


## Tools Used
- Python (Jupyter Notebook)
- Pandas
- PyCharm
- CSV Dataset

## Results
The dataset is now consistent, duplicate-free, formatted properly, and ready for analysis or machine learning workflows.

## Author
NITHIN N  
Email: nithin.n.1482003@gmail.com  
GitHub: [@nithin3114](https://github.com/nithin3114)
