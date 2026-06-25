

## Training and Guidance

This project was developed as part of practical learning and hands-on implementation under the guidance and support of:

**Coding Block School of Technology**

**Instructor:** Aryeesh Sir

The project involved understanding customer churn prediction concepts, data preprocessing techniques, exploratory data analysis, handling imbalanced datasets using SMOTE, and implementing multiple machine learning models for prediction and comparison.




# Customer Segmentation and Churn Prediction using Machine Learning

## Project Overview

Customer churn prediction is the process of identifying customers who are likely to discontinue a company's services. Customer retention is critical because acquiring new customers generally costs more than retaining existing customers.

This project focuses on analyzing telecom customer behavior, segmenting customers based on their characteristics, and predicting customer churn using multiple Machine Learning techniques.

The project includes:

- Exploratory Data Analysis (EDA)
- Data Cleaning and Preprocessing
- Customer Segmentation using K-Means Clustering
- Handling Imbalanced Data using SMOTE
- Multiple Machine Learning Models
- Hyperparameter Tuning
- Model Evaluation and Comparison

---

## Problem Statement

Telecom companies often face customer loss because of competition, pricing issues, poor service quality, or customer dissatisfaction.

The objective of this project is to:

- Analyze customer behavior patterns
- Segment customers into different groups
- Predict customers likely to churn
- Identify important factors affecting churn
- Provide insights for improving customer retention

---

## Dataset Information

**Dataset:** Telco Customer Churn Dataset

### Dataset Statistics

- Total Records: 7043
- Total Features: 33
- Target Variable: `Churn Value`

### Target Variable

- `0` → Customer stays
- `1` → Customer churns

### Features Include

- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure Months
- Phone Service
- Multiple Lines
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming Services
- Contract Type
- Payment Method
- Monthly Charges
- Total Charges

---

## Training and Guidance

This project was developed as part of practical learning and implementation under:

**School of Technology**

**Instructor:** Aryeesh Sir

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
- Histograms
- Boxplots

### Key Findings

- Customers with month-to-month contracts have higher churn rates.
- Customers with lower tenure are more likely to churn.
- Higher monthly charges increase churn probability.
- Customers without technical support have greater churn risk.

---

## Data Preprocessing

The following preprocessing steps were performed:

### Data Cleaning

- Converted `Total Charges` from object datatype to numeric datatype
- Handled missing values using median imputation

### Removed Unnecessary Features

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

### Feature Engineering

Applied One-Hot Encoding:

```python
pd.get_dummies(drop_first=True)
````

### Data Split

Dataset was divided into:

* Training Data: 80%
* Testing Data: 20%

---

## Handling Imbalanced Data

The dataset showed class imbalance:

* Non-Churn Customers: 73.46%
* Churn Customers: 26.54%

To address this issue:

**SMOTE (Synthetic Minority Oversampling Technique)** was applied.

Benefits:

* Balanced minority class samples
* Improved model performance
* Reduced prediction bias

---

## Machine Learning Models Implemented

The following models were trained and compared:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. K-Nearest Neighbors (KNN)
5. Support Vector Machine (SVM)
6. Gradient Boosting
7. XGBoost
8. Balanced Random Forest

---

## Hyperparameter Tuning

Hyperparameter tuning was performed using:

**GridSearchCV**

Parameters tuned:

* Number of estimators
* Maximum tree depth

Purpose:

* Improve model accuracy
* Optimize model performance

---

## Customer Segmentation

Customer segmentation was implemented using:

**K-Means Clustering**

Steps performed:

1. Selected important customer attributes:

   * Tenure Months
   * Monthly Charges
   * Total Charges

2. Applied Standard Scaling

3. Used Elbow Method to determine optimal clusters

4. Created customer segments

Benefits:

* Understand customer groups
* Identify high-value customers
* Improve retention strategies

---

## Model Evaluation Metrics

Models were evaluated using:

* Accuracy Score
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC Curve
* AUC Score

---

## Feature Importance

Major features influencing churn:

* Total Charges
* Tenure Months
* Monthly Charges
* Contract Type
* Internet Service
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

### Development Environment

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
Feature Scaling
↓
Model Training
↓
Hyperparameter Tuning
↓
Model Comparison
↓
ROC Curve Evaluation
↓
Customer Segmentation using K-Means
↓
Prediction and Business Insights

---

## Conclusion

This project successfully analyzed telecom customer behavior, segmented customers into groups, and predicted customer churn using Machine Learning techniques.

The analysis indicated that factors such as:

* Customer tenure
* Monthly charges
* Contract type
* Technical support availability
* Internet services

strongly affect customer churn behavior.

Machine Learning can help telecom companies identify customers likely to leave and support effective retention strategies.

---

## Future Enhancements

* Deep Learning Implementation
* Real-Time Prediction Dashboard
* Deployment using Flask or Streamlit
* Recommendation System for Customer Retention
* Live Customer Monitoring System

```
```
