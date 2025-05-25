# Final-Project-BAN-6440
# Credit Card Fraud Detection Using Machine Learning

This project applies supervised machine learning models to detect fraudulent credit card transactions using the Kaggle Credit Card Fraud Dataset(https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). The dataset is highly imbalanced and includes anonymized features extracted using PCA.

---

## Objective

To build a robust fraud detection model that identifies fraudulent transactions with high recall, minimizing false negatives, and ensuring customer trust and financial protection.

---

## Dataset Overview

- **Source:** Kaggle (Anonymized credit card transactions)
- **Size:** 284,807 transactions
- **Fraudulent transactions:** 492 
- **Features:** 28 anonymized PCA features + Amount and Time

---

##  Data Preprocessing

- Dropped Time feature (not useful for prediction)
- Scaled Amount using StandardScaler
- Addressed class imbalance using class_weight='balanced' and stratified sampling

---

## Exploratory Data Analysis

- Visualized class imbalance
- Analyzed feature correlations using heatmaps
- Summarized transaction amounts for fraud vs. legitimate cases

---

##  Models Used

| Model                | Accuracy | Recall | Precision |
|---------------------|----------|--------|-----------|
| **Random Forest**    | 95%      | **100%** | 100%       |
| **Logistic Regression** | **97%** | 97%    | 100%       |
| **Decision Tree**     | 91%      | 98%    | 100%       |

> **Best model**: Random Forest due to its perfect recall, meaning it detects all fraudulent transactions.

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall (primary focus)
- F1 Score
- Confusion Matrix
- AUC-ROC Curve

---

##  Business Impact

- Reduced financial losses by identifying fraudulent transactions in real-time
- Increased customer trust and operational efficiency
- Estimated ROI: Prevent potential loss of ~$500,000/year

---

##Future Improvements
- Implement advanced models like XGBoost,Isolation Forest, or AutoEncoders
- Deploy model in a real-time detection system
- Set up feedback loops to retrain the model with new data
- Investigate deep learning for complex fraud patterns

---

## How to Run

1. Clone this repository
2. Install required libraries:
   
   


