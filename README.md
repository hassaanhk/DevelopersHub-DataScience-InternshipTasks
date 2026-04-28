# DevelopersHub-DataScience-InternshipTasks.
Data Science internship tasks involving EDA, Credit Risk Prediction and Customer Churn Prediction.

**Task 1:** Iris Dataset Visualization

**Objective:** To perform Exploratory Data Analysis (EDA) on the Iris dataset.

**Approach:** - Loaded data using Pandas and Seaborn.
- Visualized relationships using Scatter, Histogram, and Box plots.
  
**Insights:** - Petal length and width show a strong linear correlation.
- The "Setosa" species is easily distinguishable from others based on petal size.

**Task 2:** Credit Risk Prediction

**Objective:** Predict loan default probability using Machine Learning.

**Approach:** - Handled missing values using Median and Mode imputation.
- Encoded categorical features for mathematical processing.
- Compared Logistic Regression and Decision Tree models.
  
**Results:** - **Logistic Regression:** ~78.86% Accuracy (Best performing).
- **Decision Tree:** ~74.80% Accuracy.
- **Key Insight:** Credit History is the most significant predictor of loan approval.

**Task 3:** Customer Churn Prediction

**Objective:** To develop a complete machine learning pipeline—from raw data preprocessing and categorical encoding to model training and feature importance analysis.

**Approach:**
Preprocessing: Used Label Encoding for Gender and One-Hot Encoding for Geography to make text data machine-readable.

Scaling: Applied StandardScaler to ensure features like "Age" and "Salary" are treated with equal weight.

Modeling: Deployed a Random Forest Classifier (100 trees) to capture complex, non-linear patterns.

**Insights:**
Performance: Achieved approximately 86% accuracy in predicting customer behavior.

Top Predictor: Age was the most significant factor, followed by Estimated Salary and Credit Score.

Conclusion: The bank should prioritize retention programs for older customers with high balances, as geography and credit card ownership showed minimal impact on the decision to leave.

**Task 4:** Bank Term Deposit Prediction
**Objective:** Predict whether a customer will subscribe to a term deposit based on marketing campaign data.
**Approach:** Performed One-Hot Encoding on categorical features (job, marital status, etc.) to convert text into a machine-readable format.

Balanced the dataset using stratification to handle the class imbalance between "yes" and "no" responses.

Utilized Random Forest to capture complex, non-linear relationships in the customer data.

Implemented SHAP (Explainable AI) to interpret individual model predictions and ensure transparency.
**Results:** Random Forest: ~84.40% Accuracy.

ROC-AUC Score: 0.91 (Excellent discriminatory power).
Key Insight: The duration of the last contact and previous successful marketing outcomes (poutcome) are the strongest indicators of a customer subscribing.


