Overview:

Using MySQL, I completed a data cleaning project that identified duplicates, standardized data, and handled missing values, preparing a layoffs dataset for analysis.

- Data Cleaning Process
- Removed duplicate records using ROW_NUMBER() and PARTITION BY
- Standardized company names using TRIM()
- Standardized industry names
- Standardized country names
- Converted date values into the DATE format
- Identified and handled NULL and blank values
- Used a self-join to populate missing industry values
- Removed records with insufficient data
- Removed the temporary row_num column

Files:

1.) layoffs_raw_data.csv - Original layoffs dataset (uncleaned)
2.) layoffs_data_cleaning.sql - SQL script containing the complete data cleaning process
3.) layoffs_cleaned_data.csv - Final dataset (cleaned
