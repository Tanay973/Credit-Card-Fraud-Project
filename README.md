# Credit-Card-Fraud-Project
This project aims to predict fraudulent credit card transactions using machine learning techniques. We analyze a dataset collected from European cardholders over a two-day period.  

## Problem Statement  
Fraudulent transactions cause **billions of dollars in losses** each year. Banks and financial institutions need **real-time fraud detection models** to minimize risks. This project builds a **classification model** to identify fraudulent transactions effectively.  

## Dataset  
- **Total Transactions:** 284,807  
- **Fraud Cases:** 492 (only 0.172% of total data)  
- **Data Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- **Features:** Time, Amount, V1 to V28 (Principal Component Analysis applied)  
- **Target Variable:** `Class` (0 = Non-Fraud, 1 = Fraud)  

## Project Workflow  
1. **Data Cleaning & Preprocessing**  
   - Handle missing values (if any)  
   - Feature scaling for `Amount`  
2. **Exploratory Data Analysis (EDA)**  
   - Analyze class imbalance  
   - Visualizations for fraud trends  
3. **Handling Imbalanced Data**  
   - SMOTE / ADASYN for balancing  
4. **Model Training & Selection**  
   - Logistic Regression, Random Forest, XGBoost  
   - Hyperparameter tuning using GridSearchCV  
5. **Model Evaluation**  
   - Metrics: Precision, Recall, F1-score, AUC-ROC  

## Key Learnings & Challenges  
- **Class Imbalance:** Since fraudulent cases are very rare, we applied advanced resampling techniques.  
- **Feature Engineering:** PCA-transformed features made interpretation difficult, so additional domain knowledge was required.  

## Results  
Our best-performing model achieved:  
✅ **Accuracy:** 78%  
✅ **AUC-ROC Score:** 85%  

## How to Run  
1. Clone this repository  
