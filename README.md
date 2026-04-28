# Customer Churn Analysis & Prediction

## Overview
This project analyzes customer churn behavior in a telecom company and builds a machine learning model to identify customers at risk of leaving.

Customer churn is a critical business problem, as retaining existing customers is significantly more cost-effective than acquiring new ones. This project transforms raw data into actionable insights and predictive modeling to support data-driven retention strategies.

---

## Objectives
- Identify key factors influencing customer churn  
- Perform exploratory data analysis (EDA)  
- Build a machine learning model for churn prediction  
- Generate actionable business recommendations 

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
- **Higher monthly charges** are associated with higher churn 
- Customers without **tech support** are more likely to churn  
- **Fiber optic users** show relatively higher churn  

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

## Key Model Insight
While the model achieves a strong ROC AUC score (0.82), indicating good overall separability, it struggles to capture churn cases effectively:

Only 50% of actual churn customers are correctly identified.

This highlights a critical business challenge:
- Many at-risk customers are not detected
- Potential revenue loss due to missed retention opportunities

---

## Feature Importance

Top factors influencing churn:
- Contract type  
- Tenure  
- Monthly charges  
- Tech support  
- Internet service  
These features enable targeted and data-driven retention strategies.

---

## Business Recommendations

- Promote long-term contracts with incentives  
- Improve onboarding experience for new customers  
- Optimize pricing strategy  
- Enhance customer support services  
- Investigate fiber optic service quality  

---

## Model Limitation & Improvement Opportunities
- Low recall for churn detection (0.50)
- Model may miss a significant portion of at-risk customers

### Potential Improvements:
- Adjust classification threshold (optimize recall)
- Apply resampling techniques (e.g., SMOTE)
- Hyperparameter tuning
- Try advanced models (e.g., XGBoost, LightGBM)

---

## Sample Output

### Confusion Matrix
<img width="458" height="402" alt="Confusion Matrix" src="https://github.com/user-attachments/assets/de49e5c5-fedd-48c7-ada4-ff4a72a36b42" />

The model correctly classifies most non-churn customers, but still misses a substantial number of churn cases.

---

### ROC Curve
<img width="459" height="463" alt="ROC" src="https://github.com/user-attachments/assets/5754e341-3c57-46da-a2d6-2d4677c1c864" />

The ROC curve demonstrates good model performance with strong class separability (AUC = 0.82).

---

### Feature Importance
<img width="934" height="479" alt="Feature Importance" src="https://github.com/user-attachments/assets/df7f370e-6f34-4b44-9774-7867af0e9d50" />

Contract type, tenure, and pricing are the most influential factors in predicting churn.

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Seaborn, Matplotlib  
- Scikit-learn  

---

## How to Run

1. git clone <your-repo-link>
2. pip install -r requirements.txt
3. Run the notebook / script
