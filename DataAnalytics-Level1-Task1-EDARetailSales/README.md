# Exploratory Data Analysis on Retail Sales Data

## Internship Details
- **Organization:** Oasis Infobyte
- **Track:** Data Analytics
- **Level:** Level 1
- **Task:** Task 1 – Exploratory Data Analysis on Retail Sales Data

## Project Overview
Exploratory Data Analysis (EDA) is an important step in data analysis that helps understand a dataset, identify patterns, detect potential data-quality issues, and discover useful insights through statistical summaries and visualizations.

This project analyzes the Sample Superstore retail dataset to explore sales trends, customer segments, product performance, and profitability across different regions and product categories.

## Objectives
- Understand the structure and characteristics of the retail dataset.
- Inspect data types, missing values, and duplicate records.
- Calculate descriptive statistics for numerical variables.
- Analyze monthly and quarterly sales trends.
- Explore customer segments and product performance.
- Compare sales across product categories.
- Examine relationships between numerical variables using a correlation heatmap.
- Analyze profit across different regions.
- Derive business insights and recommendations from the analysis.

## Dataset Description
The project uses the **Sample Superstore** dataset in CSV format.

The dataset contains information about:
- Order ID and order dates
- Shipping dates and shipping modes
- Customer names and customer segments
- City, state, and region
- Product categories and sub-categories
- Sales, quantity, discount, and profit

**Note:** The dataset does not contain customer age or gender, so demographic analysis using those attributes is not included.

## Tools and Technologies
- **Python** – Data analysis
- **Jupyter Notebook** – Interactive analysis and documentation
- **Pandas** – Data loading, inspection, grouping, and statistical summaries
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization and correlation heatmap

## Methodology

### 1. Data Loading and Inspection
Loaded the CSV dataset into a Pandas DataFrame and examined its rows, columns, dimensions, data types, and missing values.

### 2. Descriptive Statistical Analysis
Calculated descriptive statistics to understand the distribution and variability of numerical attributes such as sales, quantity, discount, and profit.

### 3. Time-Based Sales Analysis
Grouped sales by month and quarter to identify changes in sales performance over time.

### 4. Customer Segment Analysis
Examined the distribution of orders across Consumer, Corporate, and Home Office segments.

### 5. Product Performance Analysis
Identified the top 10 products by quantity sold to understand which products had the highest sales volume.

### 6. Category-Wise Sales Analysis
Compared total sales across product categories to identify categories contributing more to overall revenue.

### 7. Correlation Analysis
Created a correlation matrix heatmap for Sales, Quantity, Discount, and Profit to explore linear relationships between numerical variables.

### 8. Regional Profit Analysis
Compared total profit across regions to identify differences in regional business performance.

## Key Findings
The analysis is designed to identify:
- Changes in sales across monthly and quarterly periods.
- Differences in the distribution of customer segments.
- Products with the highest quantities sold.
- Product categories contributing to total sales.
- Relationships between sales, quantity, discount, and profit.
- Differences in profit across regions.

The exact findings should be interpreted from the results and charts generated in the Jupyter Notebook.

## Business Recommendations
- Use historical sales trends to support inventory and sales planning.
- Monitor high-volume products to maintain appropriate stock levels.
- Evaluate product profitability alongside sales volume before prioritizing products.
- Review discounts and their relationship with profit.
- Investigate regional performance differences using sales, product mix, and discount information.
- Use customer-segment information to support targeted marketing strategies.

## Limitations
- The dataset does not contain customer age or gender.
- Correlation indicates association, not necessarily causation.
- Historical sales trends alone cannot guarantee future sales performance.
- Further investigation may be needed to understand the causes of regional or product-level profit differences.

## Conclusion
This project demonstrates how Exploratory Data Analysis can be used to understand retail sales data through data inspection, descriptive statistics, time-based analysis, product and category comparisons, correlation analysis, and regional profitability analysis.

The findings can help identify patterns and areas for further investigation, supporting more informed retail business decisions.


## How to Run the Project
1. Install Python and Jupyter Notebook.
2. Install the required libraries:
   `pip install pandas matplotlib seaborn`
3. Place the dataset in the same directory as the notebook.
4. Open `EDA_Retail_Sales.ipynb` in Jupyter Notebook.
5. Run the notebook cells in order.

