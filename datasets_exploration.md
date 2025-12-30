## Dataset 1: Loan Default Dataset (Kaggle)

Source:
https://www.kaggle.com/datasets/nikhil1e9/loan-default

Description:
This dataset contains loan applicant information along with a default indicator. It is a single-file dataset with approximately 250,000 records and 18 features. The dataset has a simple and clean tabular structure, making it suitable for baseline loan default prediction analysis.

Why it is interesting:
Due to its simplicity and well-structured format, this dataset is useful for quickly understanding the fundamentals of loan default prediction without complex data integration.

Prediction Potential:
Binary classification to predict loan default status (default vs. non-default).

## Dataset 2: Home Credit Default Risk (Kaggle)

Source:
https://www.kaggle.com/competitions/home-credit-default-risk/data

Description:
The Home Credit Default Risk dataset provides a predefined training and test split. The training dataset includes a binary target variable (TARGET) indicating loan default, while the test dataset does not include the target and is intended for model evaluation in the original Kaggle competition.

This dataset consists of multiple related CSV files that capture both applicant-level information and historical credit behavior.

Key Files Explored:

application_train.csv
This is the main dataset used for prediction. It contains one row per loan application and includes the target variable (TARGET, where 1 = default and 0 = no default). The dataset includes applicant demographics, income, employment details, and other financial attributes. It contains approximately 307,500 records and has a significant number of missing values, reflecting real-world data complexity.

bureau.csv
This file contains information about clients’ previous credits provided by other financial institutions that were reported to a credit bureau. It includes credit history details such as loan status and credit amounts. There are multiple rows per customer, and the join key with the main dataset is SK_ID_CURR. Credit history is highly predictive of loan default and adds strong real-world relevance.

previous_application.csv
This file contains information about previous loan applications made by the borrower at Home Credit, including whether the applications were approved or rejected. It provides insight into borrower behavior and prior lending decisions, which are relevant for default risk assessment.

HomeCredit_columns_description.csv
This file provides detailed descriptions of columns across all dataset files and is used as documentation to better understand the dataset features.

Additional Supporting Files (Not Used Initially):

bureau_balance.csv – Monthly credit balance history (very large and granular)

installments_payments.csv – Detailed installment payment history

POS_CASH_balance.csv – Monthly POS and cash loan balances

credit_card_balance.csv – Monthly credit card balance snapshots

These files provide detailed time-series information but require complex aggregation and are not included in the initial project scope.

Final Dataset Selection for Prediction:
The primary dataset used for prediction is application_train.csv.
To keep the project scope manageable while still incorporating meaningful historical credit information, bureau.csv is selected as a secondary dataset for potential feature enrichment in later stages.
   

# Dataset 3 Description
Source: https://relational.fel.cvut.cz/dataset/Financial


