# CreditCardFraudDetection
This project implements a Naive Bayes model for detecting credit card fraud. The goal is to build a robust system that can identify potentially fraudulent transactions and enhance the security of credit card transactions.

## Project Overview
Credit card fraud is a significant concern in the financial industry, and having effective fraud detection mechanisms is crucial to protect both consumers and financial institutions. This project focuses on creating a predictive model using the Naive Bayes algorithm to identify patterns associated with fraudulent credit card transactions.

## Data
The dataset used for this project is sourced from Kaggle: [Credit Card Fraud Detection.](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) This dataset contains transactions made by credit cards in September 2013 by European cardholders. It includes a mix of fraudulent and non-fraudulent transactions, making it suitable for training a machine learning model.

The features in the dataset include time, amount, and various anonymized features (V1, V2, ..., V28) obtained through a dimensionality reduction technique (likely PCA) due to privacy concerns. The target variable is "Class," where 1 indicates a fraudulent transaction and 0 indicates a non-fraudulent transaction.

## Model
The Naive Bayes algorithm is employed for its simplicity and effectiveness in handling high-dimensional data. Despite its "naive" assumption of independence between features, Naive Bayes often performs well in real-world scenarios, especially with limited data and computational resources.

## Downloading the Dataset
To use this notebook or replicate the project, follow these steps to download the dataset:

1. Go to your Kaggle account and navigate to the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

2. Click on the "Copy API command" button (three dots at the top right) to get the command for downloading the dataset.

3. Open a Jupyter Notebook in your Anaconda environment.

4. Paste and run the copied command in a notebook cell to download the dataset directly. Make sure to have the `kaggle.json` file in the correct location. If you don't have it, follow the instructions in the [Kaggle documentation](https://github.com/Kaggle/kaggle-api#api-credentials) to obtain it.

   ```python
   !kaggle datasets download -d mlg-ulb/creditcardfraud
