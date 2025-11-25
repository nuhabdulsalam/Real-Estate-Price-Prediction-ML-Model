# 📘 Real Estate Price Prediction – Machine Learning Project

### 🏡 Project Overview
This project predicts house prices using the Real Estate dataset.
Two regression models were trained and evaluated:
-Linear Regression
-K-Nearest Neighbors (KNN) Regression
After comparing both models, KNN Regression performed better and was further improved using Hyperparameter Tuning (GridSearchCV & RandomizedSearchCV).

### 📂 Dataset
-The dataset used is:
📄 Real estate.csv
-Target Variable
Y house price of unit area
-Features include:
House age
Distance to MRT station
Number of convenience stores
Latitude & Longitude
...and more

### 🧹 Data Preprocessing
Removed target column from features
Train-test split (80/20)
Feature scaling using StandardScaler (for KNN model)
Correlation heatmap created

### 🤖 Models Trained
1️⃣ Linear Regression
Trained on raw (unscaled) features
Performance was good but not the best
2️⃣ KNN Regression
Trained on scaled features
Outperformed Linear Regression on all evaluation metrics

### 📊 Model Comparison
Metric	Linear Regression	KNN Regression (Before Tuning)
R² Score	67.45%	70.46%
RMSE	7.39	7.04
MAE	5.41	5.01

### ✔ KNN Regression selected for hyperparameter tuning

### 🔧 Hyperparameter Tuning
GridSearchCV — Best Parameters Found
{'algorithm': 'auto', 'n_neighbors': 15, 'weights': 'distance'}

### 🏆 Final Tuned Model Performance
Metric	Value
Final R² Score	72.03%
Final RMSE	6.85
Final Model	KNN Regression (GridSearchCV Tuned)
