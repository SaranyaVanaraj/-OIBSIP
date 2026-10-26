# Credit Card Fraud Detection

## Oasis Infobyte – Data Analytics Internship
**Level 1 | Task 3**

## Project Overview
This project focuses on detecting fraudulent credit card transactions using exploratory data analysis and machine learning techniques. The analysis explores transaction patterns, addresses class imbalance, and compares classification models to identify potentially fraudulent transactions.

## Objectives
- Analyze credit card transaction data using Python.
- Perform Exploratory Data Analysis (EDA) to identify patterns and trends.
- Examine class imbalance between legitimate and fraudulent transactions.
- Visualize transaction amounts and fraud patterns over time.
- Build and compare machine learning classification models.
- Evaluate model performance using appropriate metrics.
- Identify important features influencing fraud detection.

## Dataset
The project uses the Credit Card Fraud Detection dataset, which contains anonymized credit card transactions made by European cardholders.

- **Total transactions:** 284,807
- **Legitimate transactions:** 284,315
- **Fraudulent transactions:** 492
- **Features:** Time, Amount, anonymized numerical features (`V1`–`V28`), and Class
- **Target variable:** `Class` (0 = Legitimate, 1 = Fraudulent)

The dataset is highly imbalanced, as fraudulent transactions account for only a small proportion of the total transactions.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow
1. Import the required Python libraries.
2. Load and inspect the credit card transaction dataset.
3. Perform data cleaning and preprocessing.
4. Analyze the distribution of legitimate and fraudulent transactions.
5. Visualize transaction amounts and fraudulent transactions across time intervals.
6. Split the dataset into training and testing sets.
7. Standardize the relevant numerical features.
8. Train Logistic Regression and Random Forest classification models.
9. Evaluate the models using precision, recall, F1-score, ROC-AUC, and confusion matrices.
10. Analyze feature importance using the Random Forest model.
11. Summarize the key findings and conclusions.

## Machine Learning Models

### Logistic Regression
Used as a classification model to predict whether a transaction is legitimate or fraudulent.

### Random Forest
An ensemble learning model that combines multiple decision trees to classify transactions and estimate feature importance.

Class weighting was used to help address the imbalance between legitimate and fraudulent transactions.

## Evaluation Metrics
- **Precision:** Measures the proportion of predicted fraud cases that are actually fraudulent.
- **Recall:** Measures the proportion of actual fraudulent transactions correctly detected.
- **F1-score:** Balances precision and recall.
- **ROC-AUC:** Measures the model's ability to distinguish between legitimate and fraudulent transactions.
- **Confusion Matrix:** Shows correct predictions and classification errors.

## Key Findings
- The dataset contains a significant imbalance between legitimate and fraudulent transactions.
- Transaction amounts and time intervals were explored to understand potential fraud patterns.
- Logistic Regression and Random Forest were compared using multiple evaluation metrics.
- Confusion matrices were used to examine fraud detection errors.
- Random Forest feature importance was analyzed to identify influential features.

## Conclusion
This project demonstrates how exploratory data analysis and machine learning can be applied to credit card fraud detection. It provides practical experience in data preprocessing, data visualization, classification model development, performance evaluation, and feature importance analysis using Python.

The project highlights the importance of evaluating models with metrics such as precision, recall, and F1-score when working with highly imbalanced datasets.

## Repository Contents
- `Fraud_Detection_Analysis.ipynb` – Jupyter Notebook containing the complete analysis, visualizations, model training, and evaluation.
- `creditcard.csv` – Dataset containing credit card transaction details used for the analysis.
