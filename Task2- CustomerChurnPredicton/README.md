# CODSOFT MAY 2024 ML TASK 3 - Customer Churn Prediction

## Project Overview

This project aims to predict customer churn for a subscription-based service or business using a Random Forest classifier. The dataset is sourced from Kaggle and includes features such as credit score, geography, gender, age, tenure, balance, and number of products used by the customer.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- imbalanced-learn

## Dataset

The dataset used in this project is sourced from Kaggle and includes the following features:
- `RowNumber`: Row number of the dataset
- `CustomerId`: Customer ID
- `Surname`: Surname of the customer
- `CreditScore`: Credit score of the customer
- `Geography`: Location of the customer
- `Gender`: Gender of the customer (male or female)
- `Age`: Age of the customer
- `Tenure`: Number of years the customer has been with the bank
- `Balance`: Average balance of the customer
- `NumOfProducts`: Number of bank product facilities the customer is using
- `Exited`: Churn label (target variable)

## Data Preprocessing

The following steps were performed during data preprocessing:
1. Dropping unnecessary columns: Row number, customer ID, and surname were dropped.
2. Label Encoding: Categorical columns such as geography and gender were converted to numeric values using Label Encoding.
3. Handling Missing Values: Any missing values were handled appropriately, such as imputation or dropping rows/columns.
4. Feature Scaling: Features were scaled using StandardScaler to ensure uniformity in the range of values.

## Model Training and Evaluation

A Random Forest Classifier was trained and evaluated:
- Random Forest Classifier
  - Accuracy: 86.55%
  - Precision: 79.25%
  - Recall: 42.75%
  - F1-score: 55.54%

### Check out Video Demonstration of this Project on my LinkedIn:

> [(https://www.linkedin.com/posts/mhmmeddanish_machinelearning-naturallanguageprocessing-activity-7201396718871928832-eYoN?utm_source=share&utm_medium=member_desktop)](https://www.linkedin.com/feed/update/urn:li:activity:7202431136365514752/)

### Author

Mohammed Danish Mohiuddin
> Contact me @ [LinkedIn](https://linkedin.com/in/mhmmeddanish/) | [Instagram](https://instagram.com/mhmmeddanishh) | [Email](mailto:dmohiuddin2@gmail.com)
