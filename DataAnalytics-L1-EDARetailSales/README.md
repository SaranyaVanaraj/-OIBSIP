# Exploratory Data Analysis on Retail Sales Data

## Internship
Oasis Infobyte – Data Analytics Internship

## Task
Level 1 – Task 1

## Objective
To analyze retail sales data and identify sales trends,
customer segments, product performance, and profit patterns.

## Tools Used
- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn

## Dataset Description

The project uses the Sample Superstore dataset in CSV format.

The dataset contains information about:

Order ID and order dates

Shipping dates and shipping modes

Customer names and customer segments

City, state, and region

Product categories and sub-categories

Sales, quantity, discount, and profit

Note: The dataset does not contain customer age or gender, so demographic analysis using those attributes is not included.

## Methodology

1. Data Loading and Inspection

Loaded the CSV dataset into a Pandas DataFrame and examined its rows, columns, dimensions, data types, and missing values.

2. Descriptive Statistical Analysis

Calculated descriptive statistics to understand the distribution and variability of numerical attributes such as sales, quantity, discount, and profit.

3. Time-Based Sales Analysis

Grouped sales by month and quarter to identify changes in sales performance over time.

4. Customer Segment Analysis

Examined the distribution of orders across Consumer, Corporate, and Home Office segments.

5. Product Performance Analysis

Identified the top 10 products by quantity sold to understand which products had the highest sales volume.

6. Category-Wise Sales Analysis

Compared total sales across product categories to identify categories contributing more to overall revenue.

7. Correlation Analysis

Created a correlation matrix heatmap for Sales, Quantity, Discount, and Profit to explore linear relationships between numerical variables.

8. Regional Profit Analysis

Compared total profit across regions to identify differences in regional business performance.

## Key Findings

The analysis is designed to identify:

Changes in sales across monthly and quarterly periods.

Differences in the distribution of customer segments.

Products with the highest quantities sold.

Product categories contributing to total sales.

Relationships between sales, quantity, discount, and profit.

Differences in profit across regions.

The exact findings should be interpreted from the results and charts generated in the Jupyter Notebook.

## Repository Contents

EDA_Retail_Sales.ipynb – Jupyter Notebook containing the analysis, code, visualizations, and observations.

retail_sales.csv – Retail dataset used for the analysis.

## How to Run the Project

Install Python and Jupyter Notebook.

Install the required libraries:
pip install pandas matplotlib seaborn

Place the dataset in the same directory as the notebook.

Open EDA_Retail_Sales.ipynb in Jupyter Notebook.

Run the notebook cells in order.
