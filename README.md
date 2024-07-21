# Fraud Detection in Financial Transactions

## Project Overview

This project involves developing a machine learning model to detect fraudulent transactions in a financial dataset. The goal is to build a robust model that can accurately identify fraudulent transactions based on various features provided in the dataset.

## Dataset

The dataset for this project was obtained from Kaggle. You can access it [here](https://www.kaggle.com/datasets/vardhansiramdasu/fraudulent-transactions-prediction).

### Dataset Description

- **step**: Maps a unit of time in the real world. In this case, 1 step is 1 hour of time. Total steps are 744 (30 days simulation).
- **type**: Type of transaction. Possible values are:
  - `CASH-IN`
  - `CASH-OUT`
  - `DEBIT`
  - `PAYMENT`
  - `TRANSFER`
- **amount**: Amount of the transaction in local currency.
- **nameOrig**: Customer who started the transaction.
- **oldbalanceOrg**: Initial balance before the transaction.
- **newbalanceOrig**: New balance after the transaction.
- **nameDest**: Customer who is the recipient of the transaction.
- **oldbalanceDest**: Initial balance of the recipient before the transaction. Note that there is no information for customers that start with 'M' (Merchants).
- **newbalanceDest**: New balance of the recipient after the transaction. Note that there is no information for customers that start with 'M' (Merchants).
- **isFraud**: Indicates whether the transaction is fraudulent (1) or not (0). In this dataset, fraudulent behavior involves agents taking control of customer accounts to empty the funds by transferring to another account and then cashing out.
- **isFlaggedFraud**: Indicates whether the transaction has been flagged as potentially fraudulent based on a rule-based system. Specifically, it flags transactions where more than 200,000 is transferred in a single transaction.

## Steps to Develop the Model

1. **Data Collection**: Obtain historical transaction data from Kaggle.
2. **Data Preprocessing**: 
   - Clean the data and handle missing values.
   - Encode categorical features.
   - Balance the dataset if necessary.
3. **Feature Engineering**:
   - Extract relevant features.
   - Engineer new features that could help in fraud detection.
4. **Exploratory Data Analysis (EDA)**:
   - Visualize patterns and anomalies in the data using graphs and statistics.
5. **Model Selection**:
   - Choose appropriate classification algorithms such as Random Forest, Support Vector Machines (SVM), or Neural Networks.
6. **Model Training**:
   - Train the selected model on the preprocessed dataset.
7. **Model Evaluation**:
   - Evaluate the model's performance using metrics like accuracy, precision, recall, and F1-score.

## Tech Stack

- **Python**: Main programming language.
- **Data Manipulation Libraries**: Pandas, NumPy.
- **Machine Learning Libraries**: Scikit-learn, XGBoost.
- **Deep Learning Libraries**: TensorFlow, Keras.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/vishal-git21/FraudDetection.git

2. Run the notebook or script to start the analysis:
Note : Remember to download the dataset in the same directory or modify the path as required
   

