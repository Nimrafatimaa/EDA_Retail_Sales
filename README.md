# Exploratory Data Analysis (EDA) – Retail Sales Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on a real-world online retail transaction dataset using Python.

The objective is to explore, clean, analyze, and visualize retail sales data to identify meaningful business patterns, customer purchasing behavior, product performance, and revenue trends.

The analysis also investigates missing values, duplicate records, invalid transactions, and statistical outliers.

## Project Objectives

- Understand the structure and characteristics of retail sales data.
- Identify and handle missing values and duplicate records.
- Clean and prepare data for analysis.
- Detect unusual transactions and outliers using the IQR method.
- Calculate important business performance indicators (KPIs).
- Analyze monthly revenue and sales trends.
- Identify top-performing products.
- Analyze country-wise sales performance.
- Explore customer purchasing patterns.
- Generate visualizations and actionable business insights.

## Dataset Information

**Dataset:** Online Retail

**Source:** UCI Machine Learning Repository

**Dataset Link:** https://archive.ics.uci.edu/dataset/352/online-retail

**Time Period:** December 2010 – December 2011

**Original Records:** 541,909 transaction lines

**Original Features:** 8 columns

### Dataset Columns

| Column | Description |
|---|---|
| InvoiceNo | Invoice or transaction number |
| StockCode | Unique product code |
| Description | Product description |
| Quantity | Number of items purchased |
| InvoiceDate | Transaction date and time |
| UnitPrice | Price per item |
| CustomerID | Customer identification number |
| Country | Customer's country |

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Openpyxl
- Visual Studio Code

## Project Structure

```text
Exploratory-Data-Analysis/
│
├── data/
│   └── Online Retail.xlsx
│
├── outputs/
│   ├── charts/
│   ├── cleaned_sales_data.csv
│   ├── monthly_sales_summary.csv
│   ├── country_sales_summary.csv
│   └── customer_summary.csv
│
├── eda_sales_analysis.py
├── requirements.txt
└── README.md
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project directory

```bash
cd Exploratory-Data-Analysis
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Download the dataset

Download the Online Retail dataset from the UCI Machine Learning Repository.

Place the downloaded Excel file inside the `data` folder and name it:

`Online Retail.xlsx`
 
## Analysis Performed

### 1. Data Loading and Exploration

- Imported the retail dataset using Pandas.
- Examined the first and last records.
- Checked dataset dimensions, columns, and data types.
- Generated descriptive statistical summaries.

### 2. Data Quality Assessment

- Identified missing values.
- Calculated missing value percentages.
- Detected duplicate records.
- Investigated invalid transactions and data inconsistencies.

### 3. Data Cleaning

- Removed exact duplicate records.
- Converted transaction dates into datetime format.
- Converted numeric fields into appropriate data types.
- Cleaned text columns.
- Separated positive sales from cancellations and returns.
- Retained unidentified customers for valid overall sales calculations.

### 4. Outlier Detection

Applied the Interquartile Range (IQR) method to identify unusual values in:

- Quantity
- Unit Price
- Revenue

Visualized outliers using boxplots.

Outliers were flagged for investigation rather than automatically removed.

### 5. Feature Engineering

Created additional analytical features:

- Revenue
- Year
- Month
- Month Name
- Day
- Day of Week
- Hour

Revenue was calculated using:

**Revenue = Quantity × Unit Price**

### 6. Business KPI Analysis

Calculated:

- Total Revenue
- Total Orders
- Unique Customers
- Unique Products
- Total Quantity Sold
- Average Order Value

### 7. Sales Trend Analysis

Analyzed monthly revenue to identify changes in sales performance and potential seasonal patterns.

### 8. Product Performance Analysis

Identified top-performing products based on revenue and quantity sold.

### 9. Geographic Sales Analysis

Analyzed country-wise revenue and compared international markets.

### 10. Customer Analysis

Examined customer revenue, order frequency, and purchasing quantities to identify high-value customers.

### 11. Data Visualization

Created charts using Matplotlib to communicate analytical findings.

## Business Questions Addressed

1. What is the total revenue generated?
2. Which month generated the highest revenue?
3. Which products generated the most revenue?
4. Which products sold the highest quantity?
5. Which countries generated the most revenue?
6. How many unique customers made purchases?
7. What is the average order value?
8. What percentage of customer IDs are missing?
9. Are there unusual transactions or outliers?
10. What business opportunities can be identified from the analysis?

## Key Business Insights

The final insights and recommendations are based on the actual results generated by running the analysis.

Areas of investigation include:

- Monthly sales performance and seasonality.
- Top revenue-generating products.
- Product demand and inventory planning.
- International market performance.
- High-value customer identification.
- Returns and cancellation patterns.
- Data quality improvements.

## Project Outcomes

This project demonstrates practical skills in:

- Data exploration and cleaning.
- Data manipulation using Pandas.
- Numerical analysis using NumPy.
- Statistical analysis and outlier detection.
- Feature engineering.
- Business KPI calculations.
- Data visualization using Matplotlib.
- Extracting business insights from real-world data.

## Future Improvements

- Build an interactive sales dashboard using Power BI.
- Perform more advanced customer segmentation.
- Conduct RFM analysis.
- Analyze customer retention.
- Use SQL for additional business queries.
- Apply machine learning for sales forecasting.

## Author

**Nimra Fatima**

Data Analytics | Python | SQL | Power BI | Machine Learning

## Dataset Attribution

Chen, D. (2015). Online Retail [Dataset]. UCI Machine Learning Repository.

https://doi.org/10.24432/C5BW33

Dataset License: Creative Commons Attribution 4.0 International (CC BY 4.0).# EDA_Retail_Sales
