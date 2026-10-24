# ApexPlanet_DATAANALYTICS_task1
# Task 1: Data Immersion & Wrangling

## Project Overview
This project focuses on acquiring, exploring, cleaning, and preparing a sales dataset for further analysis using Python and Pandas. The objective is to identify data-quality issues, handle missing values, validate data, and produce a clean, analysis-ready dataset.

## Objectives
- Understand the structure and business relevance of the dataset.
- Perform initial data profiling and quality assessment.
- Identify and handle missing values.
- Check duplicate records and repeated Order IDs.
- Validate date formats, numerical ranges, and sales calculations.
- Export the cleaned dataset and document the cleaning process.

## Tools and Technologies
- Python
- Pandas
- Google Colab
- Excel
- GitHub

## Dataset Description
The dataset contains 1,000 rows and 12 columns related to sales transactions, customers, products, quantities, prices, and dates.

Key columns include:
- `Order_ID` — Order record identifier
- `Order_Date` — Date of the order
- `Customer_ID` — Customer identifier
- `Customer_Name` — Customer name or label
- `Age`, `Gender`, `City` — Customer information
- `Product`, `Category` — Product information
- `Quantity` — Number of units purchased
- `Unit_Price` — Price per unit
- `Total_Sales` — Recorded sales amount

## Data Quality Assessment
The initial assessment identified:
- 20 missing values in `Age`
- 13 missing values in `City`
- No completely duplicated rows
- One repeated `Order_ID` value, `ORD100050`, appearing nine times
- No missing or invalid dates
- No incorrect sales calculations based on `Quantity × Unit_Price`
- No invalid values detected in the basic age, quantity, and unit-price range checks

## Data Cleaning and Transformation
The following steps were performed:
1. Converted `Order_Date` to datetime format.
2. Replaced missing `Age` values with the median age of 41.
3. Replaced missing `City` values with `Unknown`.
4. Checked for completely duplicated rows.
5. Validated numerical ranges and sales calculations.
6. Investigated the repeated Order ID and retained its records pending further verification.

## Final Dataset
After cleaning, the dataset contains **1,000 rows and 12 columns**, with zero remaining missing values and zero completely duplicated rows.

## Repository Contents
- `README.md` — Project overview and methodology
- `data_dictionary.csv` — Column descriptions, data types, and business relevance
- `cleaning_script.py` — Python script used for cleaning and validation
- `cleaned_sales_dataset.csv` — Cleaned dataset ready for analysis

## Conclusion
This project demonstrates the importance of data profiling, data cleaning, validation, and documentation before conducting further analysis. The resulting dataset is prepared for exploratory data analysis and visualization.

## Author
Pravallika
