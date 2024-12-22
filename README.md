# Customer Churn Prediction Project
![alt text](download-1.png)

## Overview
This project aims to predict customer churn in a telecommunications dataset using machine learning models. The primary objective is to enable proactive retention strategies by accurately identifying customers who are likely to churn and uncovering key drivers influencing churn. The project includes data preprocessing, exploratory analysis, iterative modeling, and actionable recommendations for business decision-making.
## Business Understanding
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

## Data Preparation
Handled missing values and converted TotalCharges column from object to integer
Checked the distribution of numerical variables for consistent scaling.

## Exploratory Data Analysis (EDA)
Analyzed feature distributions and relationships using visualizations.
Checked for outliers in the dataset
Highlighted key correlations:
Tenure negatively correlates with churn (-0.35), indicating longer-tenured customers are less likely to churn.
Monthly Charges showed a weak positive correlation (0.19) with churn.

## Data Preprocessing
Dropped unnecessary columns.
split the data into train and test sets.
onehotencoded the categorical variables and scaled the numerical variables

## Modeling
Built multiple models to predict churn, including Logistic Regression, Decision Tree, and Random Forest.
The Baseline Model is Logistic Regression with default parameters for interpretability.
Refined Models using cross validation Hyperparameter-tuned Logistic Regression and advanced models like Decision Tree and Random Forest.
Evaluated models using metrics such as accuracy, recall, precision, F1-score, and ROC-AUC.
did cross-validation to provide detailed insights into the performance of my classification model by showing how predictions are distributed among the true positive, true negative, false positive, and false negative categories. 

## Model Selection
Selected the best-performing model based on accuracy and ROC-AUC to ensure effective identification of churners.

## Limitations
1. Class Imbalance:
The dataset is imbalanced, with fewer churn cases than non-churn cases, which affects model performance.
Future Work: Apply advanced techniques like SMOTE or ensemble methods to better address class imbalance.
2. Limited Features:
The dataset lacks potential features like customer support interactions, feedback, or competitor pricing, which could improve model accuracy.
Future Work: Incorporate additional data sources for richer predictions.
3. Recall vs. Precision Trade-off:
While the model achieves high recall, precision is moderate, leading to some false positives. This may result in unnecessary retention efforts.
Future Work: Optimize the classification threshold to balance recall and precision based on business needs.

## Recommendations and Areas of Improvement
1. Utilize Model Predictions for Targeted Retention Campaigns:

- Retaining existing customers is more cost-effective than acquiring new ones. By focusing on customers flagged as likely churners, businesses can prioritize resources effectively.
- **Action:** Develop personalized retention strategies such as discounts, loyalty programs, or tailored communication for at-risk customers to prevent churn and maximize revenue.
2. Enhance Data Quality and Feature Enrichment:

- The quality and diversity of data directly influence model performance. Missing or irrelevant features may prevent the model from accurately identifying churn patterns.
- **Action:** Incorporate additional data sources such as customer support interactions, complaint records, and external market data to improve the model’s predictive capabilities and actionable insights.
3. Monitor Model Performance and Retrain Regularly:

- Customer behaviors and market dynamics evolve over time, which can lead to model drift. Regular monitoring ensures that predictions remain accurate and relevant.
- **Action:** Set up periodic model evaluations and retraining using updated data to adapt to changing patterns and maintain high performance.
