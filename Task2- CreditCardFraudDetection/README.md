# CODSOFT MAY 2024 ML TASK 2 - Credit Card Fraud Detection

## Project Overview

This project aims to build a credit card fraud detection system using machine learning models such as Random Forest, Logistic Regression, and Decision Tree classifiers. The dataset is sourced from Kaggle and contains features such as transaction date, credit card number, merchant, transaction category, amount, and more.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [How to Use](#how-to-use)

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- tqdm

## Dataset

The dataset used in this project is from Kaggle and includes the following features:
- `trans_date_trans_time`: Transaction date and time
- `cc_num`: Credit card number
- `merchant`: Merchant name
- `category`: Transaction category
- `amt`: Transaction amount
- `first`: Cardholder's first name
- `last`: Cardholder's last name
- `gender`: Cardholder's gender
- `street`: Cardholder's street address
- `is_fraud`: Fraud label (target variable)

## Data Preprocessing

The following steps were performed during data preprocessing:
1. Dropping unnecessary columns: First name, last name, and street address were dropped.
2. Label Encoding: Categorical columns such as merchant, category, and gender were converted to numeric values using Label Encoding.
3. Datetime Conversion and Feature Extraction: The transaction date and time were converted to datetime format, and new features like year, month, day, and hour were extracted.
4. Ensuring Numeric Columns: All columns were ensured to be numeric, and any NaNs introduced by coercion were filled.

## Feature Engineering

The following features were engineered:
- `transaction_year`
- `transaction_month`
- `transaction_day`
- `transaction_hour`

These features were extracted from the transaction date and time.

## Model Training and Evaluation

Three models were trained and evaluated:
1. Random Forest Classifier
2. Logistic Regression
3. Decision Tree Classifier

The models were evaluated based on accuracy, precision, recall, and F1-score.

## Results

### Random Forest Classifier
- Accuracy: 99.83%
- Confusion Matrix:
  - True Positives: 553,463
  - True Negatives: 1,304
  - False Positives: 111
  - False Negatives: 841
- Classification Report: High precision and recall for the non-fraudulent class, indicating robust performance.

### Logistic Regression
- Accuracy: 99.60%
- Confusion Matrix:
  - True Positives: 553,470
  - True Negatives: 0
  - False Positives: 104
  - False Negatives: 2,145
- Classification Report: High for the non-fraudulent class but room for improvement in fraud detection.

### Decision Tree Classifier
- Accuracy: 99.39%
- Confusion Matrix:
  - True Positives: 551,188
  - True Negatives: 1,130
  - False Positives: 2,386
  - False Negatives: 1,015
- Classification Report: Balanced approach with moderate performance in fraud detection.

## How to Use

To use this project, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
