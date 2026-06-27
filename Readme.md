# Missing Data Detection, Diagnosis & Imputation

## Project Overview
This project demonstrates how to handle missing data in a customer purchase dataset using a structured workflow:

1. Detect missing values
2. Diagnose missing patterns
3. Impute missing values
4. Avoid data leakage
5. Save cleaned dataset and reports

## Dataset Columns
- Age
- Income
- Purchases

## Missing Data Summary
- Age had 30% missing values
- Income had 30% missing values
- Purchases had 20% missing values

## Cleaning Strategy
| Column | Strategy | Reason |
|---|---|---|
| Age | Median Imputation | Safe for numeric data |
| Income | Median Imputation | Income may contain outliers |
| Purchases | Drop Missing Rows | Purchases is the target column |

## Key Learning
Never impute before train-test split because it can cause data leakage.

## Files Included
- raw_customer_data.csv
- clean_customer_data.csv
- missing_value_report.csv
- income_missing_diagnosis.csv
- notebook.ipynb

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
