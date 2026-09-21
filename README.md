Overview:

In the Exploratory Data Analysis project, I explore and build upon the data I cleaned in my [Cleaning Layoff Data](https://github.com/Dannys-Portfolio/Cleaning_Layoff_Data.git) project.

Using MySQL, I prepared the company layoffs dataset for analysis. I performed the following steps: 

- Removed duplicate records using ROW_NUMBER() and PARTITION BY
- Standardized company names using TRIM()
- Standardized industry names
- Standardized country names
- Converted date values into the DATE format
- Identified and handled NULL and blank values
- Used a self-join to populate missing industry values
- Removed records with insufficient data
- Removed the temporary row_num column

Then, I explored the dataset further:

- Identified the date range covered by the dataset
- Analyzed total layoffs by company, industry, country, year, and funding stage
- Examined companies where 100% of reported employees were laid off
- Calculated monthly layoffs
- Created a rolling total of layoffs over time
- Identified the top five companies by layoffs for each year using DENSE_RANK()
- Compared the number of companies and average percentage laid off across funding stages
- This project demonstrates the use of the following:
  - SELECT
  - WHERE
  - GROUP BY
  - ORDER BY
  - Aggregate functions, such as, SUM(), MAX(), MIN(), COUNT(), and AVG()
  - YEAR() and SUBSTRING() for date-based analysis
  - Common Table Expressions (WITH)
  - Window functions
  - SUM() OVER() for rolling totals
  - DENSE_RANK() with PARTITION BY for yearly rankings
  - Conditional filtering of NULL values
  
Key Areas Explored:

Layoffs Over Time:

  I performed monthly and yearly aggregations to identify changes in the volume of reported layoffs over the period covered by the dataset.

Companies:

  I ranked companies based on their total reported layoffs. Additionally, a yearly ranking was also created to reveal the five companies with the highest reported layoffs for each year.

Industries and Countries:

  I aggregated by industry and country to identify where the largest numbers of reported layoffs occurred.

Funding Stage:

  I compared funding stage, number of companies, and average percentage laid off to find patterns in layoffs across different stages of company development.

Files:

1.) layoffs_raw_data.csv - Original layoffs dataset (uncleaned)

2.) layoffs_data_cleaning.sql - SQL script containing the complete data cleaning process

3.) layoffs_cleaned_data.csv - Final dataset (cleaned)

4.) Exploratory_Data_Analysis_Script.sql — SQL queries and explanations of their use cases for this exploratory data analysis

