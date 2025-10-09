🌍 World Layoffs Data Cleaning & Exploration (SQL Project)
📋 Overview

This project focuses on cleaning, transforming, and analyzing global layoffs data using SQL. The dataset (world_layoff.layoffs_staging2) contains information about company layoffs, industries, locations, and funding — providing insights into global workforce trends.

The workflow includes data cleaning, standardization, and exploratory data analysis (EDA) to uncover patterns such as which industries, countries, and companies have seen the largest layoffs.

🧹 Data Cleaning Steps

Removed duplicates using a ROW_NUMBER() method.

Trimmed whitespace and standardized text fields (company, country, industry).

Fixed inconsistent entries, e.g., unified all variations of “Crypto” under one category.

Converted date formats (STR_TO_DATE) and changed column type to DATE.

Handled missing values by:

Setting blank fields to NULL.

Updating missing industry values based on matching company/location data.

Deleting rows with no layoff or percentage data.

📊 Exploratory Analysis

Key SQL queries explored:

Top companies and industries by total layoffs.

Layoffs by country to identify geographic trends.

Monthly and rolling totals of layoffs over time.

Yearly breakdowns of layoffs per company.

Top 5 companies with the highest layoffs each year using window functions (DENSE_RANK()).

🧠 Insights

Revealed which industries were hit hardest by layoffs.

Tracked temporal layoff patterns (e.g., pandemic spikes).

Identified companies with recurring layoffs across multiple years.

⚙️ Tools & Technologies

SQL (MySQL flavor)

Window functions (ROW_NUMBER(), DENSE_RANK(), OVER)

CTEs and subqueries

String and date manipulation functions

🚀 How to Use

Import the dataset into your SQL environment.

Run the cleaning queries in order.

Use the analysis queries to explore trends and visualize results.

📈 Future Improvements

Automate transformations using Python + SQLAlchemy.

Build a dashboard in Power BI or Tableau for visual analytics.

Add time-series forecasting of layoffs by sector.
