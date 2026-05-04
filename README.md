📊 TeleConnect ML Project

Customer Churn Prediction & Revenue Forecasting

🚀 Project Overview

This project focuses on solving two major business problems in a telecom company:

🔹 Predicting customer churn (whether a customer will leave)
🔹 Forecasting monthly revenue per customer

Using machine learning, the project helps identify high-risk customers and provides insights to improve retention and profitability.

🎯 Problem Statement

Telecom companies often face:

High customer churn
Unstable revenue patterns

This project aims to:

Build a classification model to predict churn (Yes/No)
Build a regression model to predict monthly revenue
Identify key factors influencing customer behavior
Provide actionable business recommendations

📁 Dataset

Dataset: Telco Customer Churn Dataset
Records: 7,043 customers
Features: 21
Target Variables:
Churn → Classification
MonthlyCharges → Regression
Key Features:
Demographics (gender, tenure)
Services (InternetService, TechSupport)
Billing (MonthlyCharges, TotalCharges)
Contract type

⚙️ Project Workflow

🔹 1. Data Preprocessing
Data cleaning (missing values, duplicates)
Encoding (Label Encoding, One-Hot Encoding)
Feature scaling (StandardScaler / MinMaxScaler)
Outlier detection (IQR / Z-score)
Feature engineering:
AvgMonthlySpend
ServiceCount
Handling class imbalance (SMOTE)
Train/Validation/Test split (70/15/15)

🔹 2. Exploratory Data Analysis (EDA)
Distribution analysis (histograms, boxplots)
Categorical analysis (count plots)
Correlation heatmap
Churn pattern analysis

🔹 3. Key Insights
📌 Month-to-month contracts → highest churn
📌 High monthly charges → higher churn
📌 Long tenure → loyal customers
📌 Lack of TechSupport/OnlineSecurity → higher churn
📌 Electronic check users → more churn

🤖 Models Used

🔹 Classification Models
Logistic Regression ✅ (Best)
Decision Tree
Random Forest
SVM
KNN

📊 Classification Results
Model	Accuracy	Precision	Recall	F1 Score
Logistic Regression	0.81	0.67	0.52	0.59
Decision Tree	0.73	0.49	0.52	0.50
Random Forest	0.78	0.61	0.49	0.55
SVM	0.79	0.65	0.50	0.57
KNN	0.76	0.56	0.47	0.51

✅ Best Model: Logistic Regression
Reason: Best balance between accuracy, precision, and recall

🔹 Regression Models
Linear Regression
Lasso Regression
Ridge Regression
Decision Tree Regressor
Random Forest Regressor ✅ (Best)
Gradient Boosting
SVR

📊 Regression Results
Model	MAE	RMSE	R²
Linear Regression	4.52	4.52	Low
Decision Tree	2.13	3.53	0.986
Random Forest	1.58	1.58	0.992
Gradient Boosting	1.83	1.83	High
SVR	3.88	3.88	Low

✅ Best Model: Random Forest Regressor
Reason: Lowest error & highest R²

📈 Model Interpretation
Feature importance analysis
SHAP values for explainability
Key drivers:
Contract type
Monthly charges
Tenure
TechSupport & OnlineSecurity

💡 Business Recommendations
Offer discounts for long-term contracts
Target high-risk customers using predictions
Provide loyalty rewards
Improve customer support services
Promote value-added services
Introduce bundled plans
Optimize pricing strategies

🛠️ Tech Stack
Languages: Python
Libraries:
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
SHAP

📂 Project Structure

Teleconnect_ML_Assignment/
│
├── Data/
│   ├── Raw_Data/
│   │   └── (original dataset files)
│   │
│   └── Processed_Data/
│       └── (cleaned datasets)
│
├── Notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Preprocessing.ipynb
│   ├── 03_Classification.ipynb
│   ├── 04_Regression.ipynb
│   └── 05_Model_Interpretation.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore

📌 Conclusion

This project demonstrates a complete end-to-end ML pipeline:

Data preprocessing → EDA → Feature Engineering → Modeling → Evaluation → Interpretation

Key outcomes:

Logistic Regression is best for churn prediction
Random Forest is best for revenue prediction
Insights help improve customer retention & revenue growth