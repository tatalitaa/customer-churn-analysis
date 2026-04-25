# Customer Churn Analysis

## Overview
This project analyzes customer churn behavior in a telecom company using exploratory data analysis (EDA) and provides actionable business insights to improve customer retention.

Customer churn is a critical problem for subscription-based businesses, as losing customers directly impacts revenue. This analysis aims to understand the key drivers behind churn and translate them into strategic recommendations.



## Objectives
- Identify key factors influencing customer churn
- Perform exploratory data analysis (EDA)
- Understand customer behavior patterns
- Provide data-driven business recommendations



## Dataset
- Telco Customer Churn Dataset
- Contains customer demographics, services, account information, and churn status



## Data Preparation
- Converted `TotalCharges` to numeric format
- Removed missing values
- Dropped irrelevant features (e.g., customerID)
- Performed categorical encoding for analysis


## Exploratory Data Analysis

Key analyses performed:
- Churn distribution
- Tenure vs churn
- Monthly charges vs churn
- Contract type vs churn
- Tech support vs churn
- Internet service vs churn


## Key Insights

- **Contract Type**
  - Month-to-month contracts have the highest churn rate
  - Long-term contracts significantly reduce churn

- **Tenure**
  - Customers with shorter tenure are more likely to churn
  - Early-stage customer experience is critical

- **Monthly Charges**
  - Higher monthly charges correlate with higher churn
  - Pricing perception plays an important role

- **Tech Support**
  - Customers without tech support are more likely to churn
  - Support services improve retention

- **Internet Service**
  - Fiber optic users show higher churn compared to DSL users
  - Potential issue in service quality or expectations



## Business Recommendations

Based on the analysis:

1. **Promote Long-Term Contracts**
   - Offer discounts or incentives for yearly subscriptions

2. **Improve Customer Onboarding**
   - Focus on early-stage engagement to reduce initial churn

3. **Optimize Pricing Strategy**
   - Align pricing with perceived value

4. **Enhance Customer Support**
   - Provide accessible and responsive tech support

5. **Evaluate Service Quality**
   - Investigate high churn in fiber optic customers


## Tools & Technologies
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn (optional modeling)

