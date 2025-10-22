## Data Cleaning Summary for Flipkart Sales Dataset

- Original dataset was over 4.5 GB with 46 million rows. Sampled first 500,000 rows for manageable processing.
- Removed duplicate rows using `.drop_duplicates()`.
- Identified and dropped rows with missing values in `total_weighted_landing_price` (less than 5% missing).
- Standardized city names: merged `HR-NCR` under `Delhi` and converted city names to uppercase without spaces.
- Converted `date_` column to a consistent `dd-mm-yyyy` format and renamed it to `DATE`.
- Cleaned and standardized all column headers to uppercase and removed spaces.
- Removed unnecessary columns: `UNNAMED: 0.2`, `UNNAMED: 0.1`, and `UNNAMED: 0`.
- Checked and confirmed appropriate data types (dates as datetime, numeric columns as float/int).
- Saved final cleaned dataset as `Sales_sample_cleaned.csv`.
