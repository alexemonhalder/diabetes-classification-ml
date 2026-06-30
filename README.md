```
# 🩺 Diabetes Classification with Machine Learning

Diabetes is one of the most prevalent chronic diseases worldwide, and early detection can make a significant difference in patient outcomes. This project builds and compares multiple machine learning classification models on the Pima Indians Diabetes Dataset to predict whether a patient is diabetic or not — based on diagnostic health measurements.

---

## 📌 Project Overview

The goal of this project is to develop a reliable binary classification system using five different machine learning algorithms, evaluate their performance across multiple metrics, and identify the best-performing model for diabetes prediction.

This project was built as part of the **Ostad AI Engineering Bootcamp — Module 11 Assignment**.

---

## 📚 Dataset

- **Name:** Pima Indians Diabetes Dataset
- **Source:** UCI Machine Learning Repository via Kaggle
- **Link:** https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database
- **Records:** 768 patients
- **Features:** 8 diagnostic measurements (Glucose, BMI, Age, Insulin, etc.)
- **Target:** `Outcome` — 1 (Diabetic) / 0 (Non-Diabetic)

> Note: The dataset contains biologically invalid zero values in columns like Glucose, BloodPressure, BMI, Insulin, and SkinThickness. These were treated as missing values and replaced with the column median during preprocessing.

---

## 🔧 Project Workflow

### 1. Data Loading & Exploration
- Loaded dataset using Pandas
- Inspected shape, data types, and missing values
- Generated summary statistics using describe()

### 2. Data Preprocessing
- Identified and replaced invalid zero values with column medians
- Separated features (X) and target variable (y)
- Applied 80/20 train-test split
- Standardized features using StandardScaler

### 3. Exploratory Data Analysis (EDA)
- Class distribution plot
- Feature distribution histograms
- Correlation heatmap

### 4. Model Training
Five classification models were trained:
- Logistic Regression
- Random Forest
- Decision Tree
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

### 5. Model Evaluation
Each model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

### 6. ROC Curve Comparison
All five models were plotted on a single ROC curve for visual comparison.

### 7. Best Model Selection & Saving
- Best model selected based on F1-Score
- Saved as diabetes_model.pkl using joblib



## 🛠️ Tech Stack

- Language: Python 3
- Environment: Google Colab
- Libraries:
  - pandas, numpy — Data manipulation
  - matplotlib, seaborn — Visualization
  - scikit-learn — Model training & evaluation
  - joblib — Model saving

---

## 🚀 How to Run

1. Clone this repository:

   git clone https://github.com/your-username/diabetes-classification-ml.git

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Download the dataset from Kaggle and upload it to your Google Drive at:

   /content/drive/MyDrive/OSTAD/Datasets/diabetes.csv

4. Run all cells from top to bottom.

---

## 📁 Project Structure

diabetes-classification-ml/
│
├── diabetes_classification_ml.ipynb   # Main notebook
└── README.md                          # Project documentation

---

## 👤 Author

Alex Emon Halder
CSE Student | Green University of Bangladesh
```