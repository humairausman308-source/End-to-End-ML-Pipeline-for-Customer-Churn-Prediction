End-to-End ML Pipeline for Customer Churn Prediction

Project Overview
This project demonstrates the construction of a reusable and production-ready machine learning pipeline for predicting customer churn using the Telco Churn Dataset
. By leveraging Scikit-learn's Pipeline API, the project streamlines preprocessing, model training, hyperparameter tuning, and deployment in a single, cohesive workflow.

Objective
-Build a robust ML pipeline that can handle preprocessing, modeling, and evaluation in one workflow.
-Predict customer churn efficiently and accurately.
-Ensure the pipeline is reusable and ready for production deployment.

Dataset
-Source: Telco Customer Churn Dataset
-Description: Contains information about customers of a telecom company, including demographic info, services   subscribed, and churn status.
-Target Variable: Churn (Yes/No)

Features & Preprocessing
The pipeline handles the following steps automatically:
1.Data Cleaning & Handling Missing Values
2.Feature Scaling – Standardization of numerical features using StandardScaler.
3.Encoding Categorical Features – Using OneHotEncoder.
4.Column Transformer – Applies preprocessing selectively to numerical and categorical columns.

ML Models
The pipeline allows training and evaluation of multiple models:
-Logistic Regression – Baseline linear model for classification.
-Random Forest Classifier – Ensemble method for better accuracy and robustness.

Hyperparameter Tuning
-GridSearchCV is used to optimize model hyperparameters.
-Cross-validation ensures stable and generalized performance.
-Supports tuning parameters such as:
    -C and penalty for Logistic Regression
    -n_estimators, max_depth, and min_samples_split for Random Forest

Pipeline Export
-Once trained, the complete pipeline (preprocessing + model) is exported using joblib.
-This allows reusability in production without retraining or redefining preprocessing steps.


Evaluation Metrics
-Accuracy
-Precision, Recall, F1-score
-Confusion Matrix for detailed analysis of model predictions

Skills Gained
-Constructing end-to-end ML pipelines
-Implementing data preprocessing using ColumnTransformer and Pipeline
-Performing hyperparameter tuning with GridSearchCV
-Exporting and deploying models in a production-ready format
-Writing reusable, maintainable ML code

Next Steps / Production Readiness
-Integrate the pipeline into a web application or API using Flask/FastAPI.
-Schedule regular retraining with new data.
-Monitor model performance with production logs and alerts.