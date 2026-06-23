

## Training and Guidance

This project was developed as part of practical learning and hands-on implementation under the guidance and support of:

**Coding Block School of Technology**

**Instructor:** Aryeesh Sir

The project involved understanding customer churn prediction concepts, data preprocessing techniques, exploratory data analysis, handling imbalanced datasets using SMOTE, and implementing multiple machine learning models for prediction and comparison.



# Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn prediction is the process of identifying customers who are likely to discontinue a company's services. Customer retention is important because acquiring a new customer generally costs more than retaining existing customers.

This project analyzes customer behavior and predicts customer churn using Machine Learning techniques on a telecom customer dataset.

The project includes:

- Exploratory Data Analysis (EDA)
- Data preprocessing
- Handling class imbalance using SMOTE
- Multiple Machine Learning models
- Model comparison and evaluation

---

## Problem Statement

Telecom companies often lose customers due to competition, pricing issues, customer dissatisfaction, or service-related problems.

The objective of this project is to build a machine learning model that predicts whether a customer is likely to churn based on customer behavior and service-related features.

---

## Dataset Information

Dataset: Telco Customer Churn Dataset

### Dataset Statistics

- Total Records: 7043
- Total Features: 33
- Target Variable: `Churn Value`

### Target Classes

- `0` → Customer stays
- `1` → Customer churns

### Features Include

- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure Months
- Phone Service
- Internet Service
- Online Security
- Online Backup
- Tech Support
- Contract
- Payment Method
- Monthly Charges
- Total Charges

---

## Exploratory Data Analysis (EDA)

The following analyses were performed:

- Distribution of Tenure Months
- Distribution of Monthly Charges
- Contract Type vs Churn
- Internet Service vs Churn
- Payment Method vs Churn
- Tech Support vs Churn
- Correlation Heatmap
- Histograms and Boxplots

### Key Findings

- Customers with month-to-month contracts have higher churn rates.
- Customers with lower tenure are more likely to churn.
- Customers with higher monthly charges tend to churn more frequently.
- Customers without technical support show higher churn probability.

---

## Data Preprocessing

Steps performed during preprocessing:

1. Converted `Total Charges` from object datatype to numeric datatype.
2. Handled missing values using median imputation.
3. Removed unnecessary columns:
   - CustomerID
   - Count
   - Country
   - State
   - Zip Code
   - Latitude
   - Longitude
   - Churn Label
   - Churn Score
   - CLTV
   - Churn Reason

4. Applied One-Hot Encoding using:

```python
pd.get_dummies(drop_first=True)
````

5. Split data into training and testing datasets.

---

## Handling Imbalanced Dataset

The dataset showed class imbalance:

* Non-Churn Customers: 73.46%
* Churn Customers: 26.54%

SMOTE (Synthetic Minority Oversampling Technique) was applied to balance classes.

---

## Machine Learning Models Used

The following models were implemented:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. K-Nearest Neighbors (KNN)
5. Support Vector Machine (SVM)
6. Gradient Boosting
7. XGBoost

---

## Model Evaluation Metrics

Models were evaluated using:

* Accuracy Score
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Results

Random Forest showed the best overall performance.

### Random Forest Performance

* Accuracy: ~78.6%
* Precision: ~0.63
* Recall: ~0.61
* F1-score: ~0.62

---

## Feature Importance

Important factors affecting customer churn:

* Total Charges
* Tenure Months
* Monthly Charges
* Contract Type
* Internet Service Type
* Payment Method
* Tech Support
* Paperless Billing
* Dependents
* Senior Citizen

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn (SMOTE)
* XGBoost

### Environment

* Google Colab

---

## Project Workflow

Dataset Collection
↓
Data Cleaning
↓
Exploratory Data Analysis
↓
Feature Engineering
↓
Data Encoding
↓
Train-Test Split
↓
SMOTE for Class Balancing
↓
Model Training
↓
Model Evaluation
↓
Prediction and Insights

---

## Conclusion

This project successfully analyzed customer behavior and predicted customer churn using machine learning techniques.

The results indicate that factors such as customer tenure, monthly charges, contract type, and technical support strongly influence customer churn behavior.

These predictive insights can help telecom companies identify customers likely to leave and improve customer retention strategies.

---

## Future Enhancements

* Hyperparameter tuning
* Deep Learning implementation
* Real-time prediction dashboard
* Deployment using Flask or Streamlit
* Customer retention recommendation system

```
```
