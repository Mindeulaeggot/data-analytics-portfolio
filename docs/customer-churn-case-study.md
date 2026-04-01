# Case Study: Customer Churn Prediction

## Problem

Customer churn is a common business problem because losing existing customers reduces recurring revenue and often costs more to recover than to prevent. The goal of this project was to classify which customers were likely to churn using demographic, usage, support, and payment-related features.

## Dataset

- `64,374` customer records
- `12` total columns
- binary target: `Churn`

## Workflow

1. Loaded and inspected the customer data.
2. Removed ID-only fields.
3. Encoded categorical variables with dummy variables.
4. Split the data into training and test sets.
5. Standardized features for logistic regression.
6. Trained and compared logistic regression and decision tree models.
7. Evaluated results using accuracy, precision, recall, F1, and ROC-AUC.

## Results

| Model | Test Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | `0.8271` | `0.8136` | `0.8237` | `0.8186` | `0.9030` |
| Decision Tree | `0.9539` | `0.9308` | `0.9751` | `0.9524` | `0.9937` |

## Key Insight

The strongest decision-tree features were:

- `Payment Delay`
- `Support Calls`
- `Gender_Male`
- `Tenure`
- `Usage Frequency`

In this dataset, churn appears to be most related to payment friction, service burden, and ongoing customer engagement.

## Business Value

This project could support a retention workflow by helping a business identify high-risk customers earlier and prioritize intervention campaigns. It also shows that I understand model comparison, not just training a single algorithm and reporting one score.

## Next Upgrade

- add probability-based customer risk segmentation
- test additional ensemble models
- create a short dashboard or presentation summary for non-technical readers
