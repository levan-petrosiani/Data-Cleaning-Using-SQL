# SQL Data Cleaning Project

## Project Overview
This project demonstrates data cleaning techniques using SQL. The data comes from a dataset tracking layoffs, and the goal is to clean and standardize this information to improve its reliability for analysis. Key tasks include removing duplicates, handling null values, and organizing data into a staging table for further transformations.

## Objectives
- **Remove Duplicates**: Identify and eliminate duplicate records to ensure each row is unique.
- **Data Standardization**: Apply transformations to standardize data formats and remove inconsistencies.
- **Handle Null Values**: Address missing values by replacing them with appropriate substitutes or handling them as needed.
- **Column Management**: Drop unnecessary columns to focus on relevant data.

## Dataset Structure
The dataset includes key information about layoffs, such as:
- **company**: Name of the company where layoffs occurred.
- **location**: Location of the company.
- **industry**: Industry type.
- **total_laid_off**: Number of employees laid off.
- **percentage_laid_off**: Percentage of employees laid off.
- **date**: Date of the layoff.
- **stage**: Company stage (e.g., early, growth).
- **country**: Country of the company's location.
- **funds_raised_millions**: Total funds raised by the company.

## Key SQL Techniques
This project employs various SQL techniques to clean and prepare the data, including:
- **Removing Duplicates**: Using `ROW_NUMBER()` to identify and remove duplicate entries based on specific fields.
- **Handling Missing Values**: Filtering or replacing `NULL` values to ensure data completeness.
- **Staging Table Creation**: Organizing data into a `layoffs_staging` table to work on a cleaned and structured version of the original data.

## Steps and Code Overview
1. **Create a Staging Table**: Copied data into a new table (`layoffs_staging`) for easier transformations.
2. **Duplicate Removal**: Used a CTE (Common Table Expression) with `ROW_NUMBER()` to identify and delete duplicate records.
3. **Standardization and Null Value Handling**: Standardized fields and addressed null values or blanks for consistent data quality.
4. **Unnecessary Column Removal**: Dropped columns that were irrelevant to the main analysis.

## Running the SQL Script
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/SQL-Data-Cleaning-Project.git
