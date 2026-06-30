# 🩺 Diabetes Classification with Machine Learning

A machine learning project that predicts whether a patient has diabetes using the **Pima Indians Diabetes Dataset**. The project compares multiple classification algorithms, evaluates their performance using standard metrics, and saves the best-performing model for future predictions.

---

# 📌 Project Overview

Early detection of diabetes can significantly improve patient outcomes. This project develops a binary classification system using five machine learning algorithms and compares their performance to identify the most effective model.

Developed as part of the **Ostad AI Engineering Bootcamp – Module 11 Assignment**.

---

# 📂 Dataset

- **Dataset:** Pima Indians Diabetes Dataset
- **Source:** UCI Machine Learning Repository (via Kaggle)
- **Records:** 768
- **Features:** 8
- **Target:** `Outcome`
  - **0** → Non-Diabetic
  - **1** → Diabetic

**Dataset Link:**

https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

> **Note:** The dataset contains medically invalid zero values in `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI`. These values were treated as missing data and replaced with the median of each respective feature.

---

# ⚙️ Project Workflow

## 1. Data Loading
- Loaded dataset using Pandas
- Explored dataset structure
- Checked shape, information, and summary statistics

## 2. Data Preprocessing
- Replaced invalid zero values with median values
- Separated features and target variable
- Performed train-test split (80:20)
- Applied feature scaling using `StandardScaler`

## 3. Exploratory Data Analysis (EDA)
- Class distribution visualization
- Feature distribution histograms
- Correlation heatmap

## 4. Model Training

The following machine learning models were trained:

- Logistic Regression
- Random Forest
- Decision Tree
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

## 5. Model Evaluation

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

## 6. ROC Curve Comparison

All trained models were compared using a single ROC Curve.

## 7. Best Model Selection

- Selected using the highest **F1-Score**
- Saved using **Joblib** as:

```
diabetes_model.pkl
```

---

# 📊 Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|--------|---------:|----------:|--------:|---------:|---------:|
| Logistic Regression | 0.753247 | 0.649123 | 0.672727 | 0.660714 | 0.814692 |
| Random Forest | 0.720779 | 0.607143 | 0.618182 | 0.612613 | 0.812489 |
| Decision Tree | 0.746753 | 0.625000 | 0.727273 | **0.672269** | 0.742424 |
| K-Nearest Neighbors (KNN) | 0.694805 | 0.583333 | 0.509091 | 0.543689 | 0.764096 |
| Support Vector Machine (SVM) | 0.733766 | 0.645833 | 0.563636 | 0.601942 | 0.804959 |

> **Best Model:** Decision Tree (Highest F1-Score: **0.672269**)

---

# 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

---

# 📁 Project Structure

```
diabetes-classification-ml/
│
├── diabetes_classification_ml.ipynb
├── diabetes_model.pkl
├── README.md
└── requirements.txt
```

---

# 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/diabetes-classification-ml.git
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Download the dataset

Download the dataset from Kaggle:

https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

### 4. Update the dataset path

Place the dataset in your preferred directory and update the path in the notebook.

### 5. Run the notebook

Open the notebook in **Google Colab** or **Jupyter Notebook** and execute all cells.

---

# 📈 Results

The project compares five popular machine learning algorithms for diabetes prediction. The best-performing model is selected based on the **F1-Score**, providing a balanced evaluation of precision and recall.

---

# 📜 License

This project is intended for educational purposes.

---

# 👨‍💻 Author

**Alex Emon Halder**

- CSE Student
- Green University of Bangladesh

GitHub: https://github.com/alexemonhalder

LinkedIn: https://www.linkedin.com/in/alexemonhalder/
