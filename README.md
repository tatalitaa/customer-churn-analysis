# Customer Churn Analysis & Prediction

## Overview
This project analyzes customer churn behavior in a telecom company and builds a machine learning model to predict customers at risk of leaving.

Customer churn is a critical business problem because retaining existing customers is significantly more cost-effective than acquiring new ones. This project transforms raw data into actionable insights and predictive capabilities to support customer retention strategies.

---

## Objectives
- Identify key factors influencing customer churn  
- Perform exploratory data analysis (EDA)  
- Build a predictive model using machine learning  
- Provide actionable business recommendations  

---

## Dataset
- Telco Customer Churn Dataset (Kaggle)  
- Includes:
  - Customer demographics  
  - Service subscriptions  
  - Billing information  
  - Churn status  

---

## Data Preparation
- Converted `TotalCharges` to numeric format  
- Removed missing values  
- Dropped irrelevant features (`customerID`)  
- Created new feature: `tenure_group`  
- Encoded categorical variables using one-hot encoding  

---

## Key Insights

- Customers with **tenure < 12 months** have the highest churn risk  
- **Month-to-month contracts** significantly increase churn  
- Higher **monthly charges** correlate with higher churn  
- Customers without **tech support** are more likely to churn  
- Fiber optic users show relatively higher churn  

---

## Machine Learning Model

- Model: Random Forest Classifier  
- Data split: 80% training, 20% testing  
- Evaluation metrics:
  - Accuracy  
  - ROC AUC Score  
  - Confusion Matrix  

The model helps identify high-risk customers and key drivers of churn.

---

## Feature Importance

Top factors influencing churn:
- Contract type  
- Tenure  
- Monthly charges  
- Tech support  
- Internet service  

---

## Business Recommendations

- Promote long-term contracts with incentives  
- Improve onboarding experience for new customers  
- Optimize pricing strategy  
- Enhance customer support services  
- Investigate fiber optic service quality  

---
## Sample Output

### Confusion Matrix
![Confusion Matrix](https://github.com/user-attachments/assets/e155da74-bae6-4508-a62f-a63b0994e211)

The model is able to correctly classify a majority of customers, although some churn cases are still misclassified.

---

### ROC Curve
![ROC Curve](https://github.com/user-attachments/assets/3c275430-31ce-4622-8c40-030a4d6b1a95)

The ROC curve shows good model performance with a strong ability to distinguish between churn and non-churn customers.

---

### Feature Importance
![Feature Importance](https://github.com/user-attachments/assets/9ac414e0-e918-48e6-bd0a-ebb9e57161d8)

Contract type, tenure, and monthly charges are the most influential factors in predicting customer churn.

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Seaborn, Matplotlib  
- Scikit-learn  

---

## How to Run

1. Clone repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
