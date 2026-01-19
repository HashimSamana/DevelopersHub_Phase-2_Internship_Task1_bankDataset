# Task 1: Term Deposit Subscription Prediction

## Objective
Predict whether a bank customer will subscribe to a term deposit based on marketing campaign data. This task involves classification modeling and explainable AI (XAI) techniques to understand customer behavior.

## Dataset
**Bank Marketing Dataset** from UCI Machine Learning Repository.  
Contains attributes like age, job, marital status, education, balance, and campaign-related information.

## Approach
1. **Data Loading and Cleaning**
   - Handled semicolon-separated CSV and removed extra quotes from columns and string values.
   - Encoded categorical features using LabelEncoder.
   - Converted target variable (`y`) to binary (yes=1, no=0).

2. **Exploratory Data Analysis (EDA)**
   - Analyzed distributions of features.
   - Checked correlations and imbalance in the target variable.

3. **Model Building**
   - Trained **Logistic Regression** and **Random Forest** classifiers.
   - Split data into training and testing sets.

4. **Model Evaluation**
   - Evaluated using Confusion Matrix, F1-score, and ROC-AUC.
   - Compared model performances.

5. **Explainable AI**
   - Used **SHAP** to interpret model predictions for 5 sample customers.
   - Identified which features influenced subscription decisions most.

## Results
- Random Forest achieved higher accuracy and F1-score compared to Logistic Regression.
- SHAP analysis revealed `duration`, `campaign`, and `poutcome` as top features influencing customer decisions.

## Tools & Libraries
- Python, pandas, numpy, scikit-learn, matplotlib, seaborn, SHAP

## Insights
- Customers contacted more recently and with shorter campaign durations were more likely to subscribe.
- XAI provided actionable insights for marketing strategy optimization.
