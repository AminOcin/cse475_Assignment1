# cse475_Assignment1
Loan Approval Prediction using Ensemble Methods
Overview
This repository contains a comprehensive analysis and predictive modeling project based on a synthetic dataset inspired by real-world credit risk data. The project applies machine learning techniques, including ensemble methods, to predict loan approval statuses and evaluate financial risk factors. The models achieve high accuracy in classifying loan applications as approved or rejected based on multiple financial and personal features.
Dataset Description
The dataset used for this project is a synthetic version derived from the Credit Risk dataset on Kaggle and enriched with additional variables from Financial Risk for Loan Approval data. It contains 45,000 records and 14 variables, with a mix of categorical and numerical features.
Features
Column	Description	Type
person_age	Age of the person	Float
person_gender	Gender of the person	Categorical
person_education	Highest education level	Categorical
person_income	Annual income	Float
person_emp_exp	Years of employment experience	Integer
person_home_ownership	Home ownership status (e.g., rent, own, mortgage)	Categorical
loan_amnt	Loan amount requested	Float
loan_intent	Purpose of the loan	Categorical
loan_int_rate	Loan interest rate	Float
loan_percent_income	Loan amount as a percentage of annual income	Float
cb_person_cred_hist_length	Length of credit history in years	Float
credit_score	Credit score of the person	Integer
previous_loan_defaults_on_file	Indicator of previous loan defaults	Categorical
loan_status (Target)	Loan approval status: 1 = approved, 0 = rejected	Integer


Key Notes:
•	Synthetic Data: SMOTENC was applied to simulate new data points and enrich the dataset.
•	Target Variable: loan_status (1 = Approved, 0 = Rejected).
•	Instances with potential outliers (e.g., age > 100 years) were carefully addressed during preprocessing.
Project Features
Exploratory Data Analysis (EDA)
•	Insights into data distribution and feature correlations.
•	Analysis of numeric feature distributions using histograms.
•	Heatmaps for visualizing correlations.
Machine Learning Models
The notebook includes implementation and evaluation of various ensemble learning models:
•	Bagging:
 Random Forest, Bagging Classifier with Decision Trees.
•	Boosting:
 Gradient Boosting, XGBoost.
•	Stacking:
 Combining multiple base models.
•	Voting: 
Hard and Soft Voting Classifiers.

Metrics and Evaluation
•	Accuracy, precision, recall, F1 score, and cross-validation results are used to evaluate model performance.
•	Visualizations include box plots for cross-validation accuracy and confusion matrices.
Explainability
•	SHAP: Feature importance visualization for interpretability.
•	LIME: Local explanation for specific predictions.
Setup Instructions
1.	Clone the repository:
git clone https://github.com/your-username/credit-risk-loan-approval.git
2.	Install dependencies:
pip install -r requirements.txt
3.	Run the Jupyter Notebook:
jupyter notebook
Requirements
•	Python 3.8+
•	Libraries:
o	pandas
o	numpy
o	scikit-learn
o	matplotlib
o	seaborn
o	xgboost
o	shap
o	lime
Install all dependencies using:
pip install -r requirements.txt
Usage
1.	Dataset Preparation: Load the dataset and preprocess it using the provided notebook.
2.	Model Training: Execute the ensemble models implemented in the notebook.
3.	Model Evaluation: Analyze performance metrics and model explainability using SHAP and LIME.
4.	Deployment: Use the best-performing model for real-world prediction tasks.
Results
•	Best Model: Identified using cross-validation accuracy and F1 score.
•	Ensemble techniques, particularly stacking and boosting, provided robust performance.
•	Explainability techniques offered valuable insights into model decisions.
License
This project is licensed under the MIT License. See the LICENSE file for details.



1
.

