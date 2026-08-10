Overview:

Using MySQL, I prepared a dataset focused on company layoffs. In order for the data to be ready for analysis, I performed the following steps: 

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

3.) layoffs_cleaned_data.csv - Final dataset (cleaned)
