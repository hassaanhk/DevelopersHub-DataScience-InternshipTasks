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

**Task 5:** Customer Segmentation (Unsupervised Learning)

**Objective:** Group mall customers into distinct segments based on spending habits to propose targeted marketing strategies.

**Approach:** Conducted Exploratory Data Analysis (EDA) to understand the distributions of Annual Income and Spending Scores.Applied StandardScaler to normalize features, ensuring the K-Means distance calculation wasn't biased by different units.Used the Elbow Method (WCSS) to mathematically determine the optimal number of clusters ($K=5$).Implemented PCA (Principal Component Analysis) to reduce dimensionality for 2D visualization of customer "islands.

**Results:** Successfully identified 5 distinct customer personas (e.g., "High Earners/Low Spenders" and "Elite Target Group").

**Key Insight:** Annual Income and Spending Score create very clear boundaries for segmentation, allowing for highly personalized loyalty programs.

**Task 6:** Loan Default Risk with Cost Optimization

**Objective:** Predict loan defaults while minimizing the total financial loss to the bank through threshold tuning.

**Approach:** Preprocessed the Home Credit dataset, focusing on external credit scores (EXT_SOURCE) and handling high-percentage missing data.

Defined a Business Cost Function where a False Negative (missed defaulter) was weighted 10x more expensive than a False Positive (rejected good client).

Shifted the decision threshold from the default 0.50 down to 0.08 to prioritize risk detection.

**Results:** Baseline Recall: 0.00 (The model initially missed all defaulters).

**Optimized Recall:** ~0.66 (Successfully caught 66% of high-risk loans after cost-tuning).

**Key Insight:** Maximizing "Accuracy" is not always the goal in finance; lowering the classification threshold significantly reduced the bank's total potential loss.
