# Heart-Disease-Prediction
To check and display the report of a heart disease

## Project Overview

This project focuses on predicting the presence of heart disease using machine learning techniques. The dataset contains clinical and demographic attributes such as age, sex, chest pain type, cholesterol level, resting blood pressure, maximum heart rate, and other medical indicators.

The project explores two different machine learning pipelines:

1. Feature Selection + PCA + Model Training (No exact dataset but assumed feature values)
2. Feature Selection + Model Training (Without PCA with sample dataset features)

The performance of multiple machine learning models is evaluated and compared.

---

## Dataset Features

* Age
* Sex
* Chest Pain Type (cp)
* Resting Blood Pressure (trestbps)
* Cholesterol (chol)
* Fasting Blood Sugar (fbs)
* Resting ECG (restecg)
* Maximum Heart Rate Achieved (thalach)
* Exercise Induced Angina (exang)
* ST Depression (oldpeak)
* Slope of ST Segment (slope)
* Number of Major Vessels (ca)
* Thalassemia (thal)
* Target (Heart Disease Presence)

---

# Method 1: Feature Selection + PCA

### Workflow

Dataset
↓
Data Preprocessing
↓
Feature Scaling
↓
Feature Selection (SelectKBest)
↓
Principal Component Analysis (PCA)
↓
Model Training
↓
Model Evaluation

### Models Used

* Logistic Regression
* Random Forest
* Support Vector Machine (SVM)

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

### Purpose

This approach reduces feature dimensionality before training. PCA helps transform selected features into principal components that retain most of the dataset variance.

---

# Method 2: Feature Selection Without PCA

### Workflow

Dataset
↓
Data Preprocessing
↓
Feature Scaling
↓
Feature Selection (SelectKBest)
↓
Model Training
↓
Model Evaluation

### Models Used

* Logistic Regression
* Random Forest
* Support Vector Machine (SVM)

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

### Purpose

This approach preserves the original selected features and improves interpretability. For datasets with a small number of features, this method is often preferred because it avoids unnecessary dimensionality reduction.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* Pickle

---

## Project Structure

dataset.ipynb
↓
preprocessing.ipynb
↓
feature_selection.ipynb
↓

Method 1:
pca.ipynb
↓
model_training.ipynb
↓
model_evaluation.ipynb

Method 2:
model_training.ipynb
↓
model_evaluation.ipynb

---

## Conclusion

Two machine learning pipelines were implemented and compared:

* Feature Selection + PCA
* Feature Selection without PCA

The final model can be selected based on evaluation metrics such as Accuracy, Precision, Recall, and F1 Score. This comparison helps determine whether dimensionality reduction through PCA improves performance for the given heart disease dataset.
