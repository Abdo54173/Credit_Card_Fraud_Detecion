# Credit Card Fraud Detection

## Description
This project aims to detect fraudulent credit card transactions using machine learning techniques.  
It handles **imbalanced data**, cleans outliers, visualizes the data, and applies different classification models to identify fraud.

---

## Dataset
- The dataset contains transactions made by credit cards in September 2013 by European cardholders.
- Features:
  - V1 to V28: Principal components obtained via PCA
  - Time: Seconds elapsed between this transaction and the first transaction in the dataset
  - Amount: Transaction amount
  - Class: Target variable (0 = normal, 1 = fraud)
- Highly imbalanced: Majority of transactions are normal (Class 0).

---

## Data Preprocessing
- **Duplicate removal**: Remove any duplicate records.
- **Feature selection**: Keep features with correlation > 0.13 with the target variable.
- **Downsampling**: Reduce the number of majority class (Class 0) transactions to balance the dataset.
- **Outlier removal**: Use IQR method to clean extreme values in Class 0.
- **Scaling**: Standardize features using `StandardScaler`.

---

## Models Implemented
1. **Logistic Regression**
2. **Decision Tree Classifier**

---

## Visualization
- Count plots to check class distribution.
- Scatter plots and pairplots to explore relationships between variables.
- Correlation bar charts to identify features most related to fraud.

---

## How to Run
1. Clone the repository:
```bash
git clone https://github.com/username/Credit_Card_Fraud_Detection.git
