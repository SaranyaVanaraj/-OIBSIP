# OIBSIP — Data Analytics Internship

## Level 1 — Task 2: Customer Segmentation Analysis

## 1. Project Overview

Customer Segmentation Analysis is a data analytics project that groups customers according to their purchasing behaviour and spending patterns. The project uses Exploratory Data Analysis (EDA), feature engineering, data standardisation, and the K-Means clustering algorithm to identify distinct customer segments.

The purpose of this project is to understand customer behaviour and generate insights that can help businesses develop targeted marketing strategies, improve customer engagement, and make data-driven decisions.

## 2. Objectives

The main objectives of this project are:

- To understand the structure and characteristics of the customer dataset.
- To clean the dataset and handle missing or inconsistent values.
- To perform descriptive statistical analysis.
- To analyse customer purchasing frequency and spending behaviour.
- To create relevant features for customer segmentation.
- To apply feature standardisation before clustering.
- To determine a suitable number of clusters using the Elbow Method.
- To apply K-Means clustering to group similar customers.
- To visualise and profile the identified customer segments.
- To recommend suitable marketing strategies for different customer groups.

## 3. Dataset Description

The project uses the **Customer Personality Analysis** dataset available on Kaggle.

Dataset link: https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis

The dataset contains customer demographic information, purchasing behaviour, spending across product categories, and responses to marketing campaigns.

Important columns include:

- **ID:** Unique identifier for each customer.
- **Year_Birth:** Customer's birth year.
- **Education:** Customer's education level.
- **Marital_Status:** Customer's marital status.
- **Income:** Customer's reported income.
- **Kidhome:** Number of young children in the household.
- **Teenhome:** Number of teenagers in the household.
- **Dt_Customer:** Date the customer enrolled with the company.
- **Recency:** Number of days since the customer's last purchase.
- **MntWines:** Spending on wine products.
- **MntFruits:** Spending on fruit products.
- **MntMeatProducts:** Spending on meat products.
- **MntFishProducts:** Spending on fish products.
- **MntSweetProducts:** Spending on sweet products.
- **MntGoldProds:** Spending on gold products.
- **NumWebPurchases:** Number of purchases made through the website.
- **NumCatalogPurchases:** Number of catalogue purchases.
- **NumStorePurchases:** Number of in-store purchases.
- **NumDealsPurchases:** Number of purchases made using deals.
- **NumWebVisitsMonth:** Number of website visits in a month.
- **Response:** Customer response to the most recent campaign.

## 4. Tools and Technologies Used

| Tool | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data loading, cleaning, and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Seaborn | Statistical visualisation |
| Scikit-learn | Feature standardisation and K-Means clustering |
| Jupyter Notebook | Interactive analysis and documentation |
| GitHub | Project storage and version control |

## 5. Methodology

### 5.1 Data Loading

The dataset was loaded into a Pandas DataFrame. The initial records, dataset dimensions, column names, and data types were examined to understand its structure.

### 5.2 Data Inspection

The dataset was inspected for missing values, duplicate records, data types, and inconsistencies. Descriptive statistics were used to understand the distribution of numerical variables.

### 5.3 Data Cleaning

Duplicate records and unsuitable or incomplete values were checked and handled as required. Relevant columns were converted to appropriate data types, and invalid records were excluded from the analysis where necessary.

### 5.4 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand customer income, spending patterns, purchasing behaviour, and product-category preferences.

Histograms and bar charts were used to explore the distributions of important variables and compare spending across product categories.

### 5.5 Feature Engineering

Three behavioural features were selected for customer segmentation:

- **Recency:** Measures how recently a customer made a purchase. Lower values indicate more recent purchases.
- **Frequency:** Calculated by combining the available website, catalogue, and store purchase counts.
- **Monetary:** Calculated as the total historical spending across the six product categories available in the dataset.

These features provide a simplified view of customer purchasing behaviour.

### 5.6 Data Transformation and Standardisation

Frequency and Monetary values were log-transformed where appropriate to reduce skewness. The selected features were then standardised using Scikit-learn's `StandardScaler`.

Standardisation ensures that features with different numerical scales do not disproportionately influence the clustering algorithm.

### 5.7 Elbow Method

The Elbow Method was used to evaluate different numbers of clusters. The Within-Cluster Sum of Squares (WCSS), also called inertia in K-Means, was calculated for different values of K.

The resulting plot was examined to select a suitable number of clusters.

### 5.8 K-Means Clustering

The K-Means clustering algorithm was applied to the standardised features. Customers were assigned to clusters based on similarities in their purchasing behaviour.

### 5.9 Cluster Visualisation

Scatter plots were created to visualise the customer groups using different feature combinations, including:

- Frequency versus Monetary.
- Recency versus Monetary.

These visualisations help illustrate differences in purchasing activity, spending, and recency among customer groups.

### 5.10 Cluster Profiling

The mean feature values and customer counts for each cluster were calculated. These summaries were used to interpret the characteristics of each segment and identify potential customer types.

## 6. Analysis and Visualisations

The project includes the following analytical outputs:

- Dataset inspection and descriptive statistics.
- Missing-value and duplicate checks.
- Customer income distribution.
- Spending comparison across product categories.
- Elbow Method plot for cluster selection.
- Frequency versus Monetary scatter plot.
- Recency versus Monetary scatter plot.
- Cluster profile summary.
- Bar chart showing the number of customers in each cluster.

Each visualisation supports the interpretation of customer behaviour and the identification of meaningful segments.

## 7. Customer Segmentation and Marketing Strategies

The clusters can be interpreted using their average Recency, Frequency, and Monetary values.

Potential customer types and corresponding strategies include:

- **High-value customers:** Customers with high spending and frequent purchases may respond well to loyalty programmes, exclusive offers, and early access to new products.
- **Recent and active customers:** Customers who purchased recently may be encouraged to make repeat purchases through personalised recommendations and relevant promotions.
- **Low-frequency customers:** Customers with relatively few purchases may benefit from product recommendations, introductory offers, and engagement campaigns.
- **At-risk or inactive customers:** Customers with higher Recency values may need re-engagement campaigns, personalised discounts, or reminders.
- **Lower-spending customers:** Customers with lower Monetary values may respond to affordable product bundles, suitable offers, and cross-selling opportunities.

*Note: These are potential interpretations. Actual segment names and recommendations should be based on the calculated cluster profiles.*

## 8. Key Insights

The analysis helps identify:

- Differences in customer spending behaviour.
- Variations in purchasing frequency.
- Differences in the time elapsed since customers' last purchases.
- Groups of customers with similar purchasing patterns.
- Potential opportunities for targeted promotions and customer retention.
- Customer segments that may benefit from personalised marketing strategies.

Specific numerical findings should be added after reviewing the actual cluster profiles and visualisation outputs.

## 9. Business Applications

Customer segmentation can help businesses:

- Design targeted marketing campaigns.
- Improve customer retention.
- Identify high-spending and frequent customers.
- Develop suitable promotional offers.
- Re-engage inactive customers.
- Personalise product recommendations.
- Allocate marketing resources more effectively.
- Support data-driven customer relationship management.

## 10. Project Structure

```text
OIBSIP/
└── DataAnalytics-L1-Task2-CustomerSegmentation/
    ├── README.md
    ├── Customer_Segmentation_Analysis.ipynb
    └── marketing_campaign.csv
```

The notebook and dataset filenames should match the files actually present in the repository. Include the dataset only if permitted by the submission guidelines.

## 11. How to Run the Project

1. Clone or download the repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. Place the dataset in the location referenced by the notebook.
5. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open `Customer_Segmentation_Analysis.ipynb`.
7. Run the notebook cells sequentially to reproduce the analysis, charts, and clustering results.

## 12. Limitations

- The dataset contains aggregated customer-level information rather than individual transaction records.
- Frequency is estimated using the available purchase-channel counts.
- Monetary value represents recorded historical spending across the available product categories.
- True Customer Lifetime Value (CLV) cannot be calculated reliably from the available features alone.
- K-Means results depend on feature selection, preprocessing, and the chosen number of clusters.
- The resulting segments describe patterns in the available dataset and may not represent every customer population.

## 13. Conclusion

This project demonstrates how customer purchasing data can be analysed using Python and machine learning techniques. Through data cleaning, exploratory analysis, feature engineering, standardisation, and K-Means clustering, customers are grouped according to similarities in their purchasing behaviour.

The resulting clusters can help businesses understand customer differences and develop more targeted marketing and retention strategies. The project also provides practical experience in data analysis, visualisation, and unsupervised machine learning.

## 14. Skills Gained

- Data cleaning and preprocessing.
- Exploratory Data Analysis.
- Descriptive statistical analysis.
- Feature engineering using Recency, Frequency, and Monetary values.
- Data standardisation.
- K-Means clustering.
- Elbow Method.
- Cluster visualisation and profiling.
- Marketing insight generation.
- Python-based data analysis.
- GitHub repository management.

## 15. Internship Details

**Organisation:** Oasis Infobyte

**Domain:** Data Analytics

**Level:** Level 1

**Task:** Task 2 — Customer Segmentation Analysis

**Repository:** OIBSIP
