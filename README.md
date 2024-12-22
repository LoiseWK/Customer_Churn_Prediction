# Customer Churn Prediction Project
## Overview
This project aims to predict customer churn in a telecommunications dataset using machine learning models. The primary objective is to enable proactive retention strategies by accurately identifying customers who are likely to churn and uncovering key drivers influencing churn. The project includes data preprocessing, exploratory analysis, iterative modeling, and actionable recommendations for business decision-making.
## Business Understunding
In subscription-based businesses, retaining customers is essential for sustained profitability. When customers leave, it doesn’t just affect current revenue,it also drives up the cost of acquiring new ones. By identifying the reasons behind customer churn and accurately predicting it, businesses can:Concentrate efforts on high-risk customers and implement targeted retention strategies, Create personalized experiences that address the specific needs of at-risk customers,Reduce the financial impact of churn while building stronger, long-term relationships with their customers.

This project aims to achieve these objectives by using data-driven insights and predictive models to address churn effectively, ensuring both customer satisfaction and business growth.

### Objectives
1. To identify the most significant factors driving customer churn
2. To accurately predict customers likely to churn using a data-driven model.
3. To identify predictive models can best forecast customer churn.

## Data Understanding
The dataset used for this project is from kaggle and contains customer data from a telecom company, including features such as customer tenure, monthly charges, payment methods, and churn status. Key details include:

- Target Variable: Churn (Yes/No).
- Numerical Features: Tenure, MonthlyCharges, TotalCharges, SeniorCitizen.
- Categorical Features: Contract Type, Internet Service, Payment Method, etc.

## Data Preprocessing
Handled missing values and transformed categorical variables into numerical formats using encoding techniques.
Addressed outliers and normalized numerical variables for consistent scaling.

## Exploratory Data Analysis (EDA)
Analyzed feature distributions and relationships using visualizations.
Highlighted key correlations:
Tenure negatively correlates with churn (-0.35), indicating longer-tenured customers are less likely to churn.
Monthly Charges showed a weak positive correlation (0.19) with churn.

## Modeling
Built multiple models to predict churn:
Baseline Model: Logistic Regression with default parameters for interpretability.
Refined Models: Hyperparameter-tuned Logistic Regression and advanced models like Decision Tree and Random Forest.
Evaluated models using metrics such as accuracy, recall, precision, F1-score, and ROC-AUC.
Addressed class imbalance using techniques like class-weight adjustment and threshold tuning.

## Model Selection
Selected the best-performing model based on recall and ROC-AUC to ensure effective identification of churners.
