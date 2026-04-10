## 🩺 Diabetes Prediction using Machine Learning

### 📌 Overview

This project presents an end-to-end machine learning pipeline for predicting diabetes based on clinical attributes. The system leverages supervised learning algorithms to classify whether a patient is diabetic or not using the Pima Indians Diabetes Dataset.

The project covers the complete ML workflow including data preprocessing, exploratory data analysis (EDA), model training, hyperparameter tuning, and evaluation.

---

### 🎯 Objectives

* Build an accurate diabetes prediction model
* Compare multiple machine learning algorithms
* Handle class imbalance effectively
* Optimize model performance using hyperparameter tuning

---

### 📊 Dataset Details

* **Dataset:** Pima Indians Diabetes Dataset
* **Total Samples:** 768
* **Features:**

  * Pregnancies
  * Glucose
  * Blood Pressure
  * Skin Thickness
  * Insulin
  * BMI
  * Diabetes Pedigree Function
  * Age
* **Target Variable:** Outcome (0 = Non-Diabetic, 1 = Diabetic)

---

### ⚙️ Methodology

#### 1. Data Preprocessing

* Replaced invalid zero values with NaN
* Applied median imputation (class-wise)
* Performed feature scaling using StandardScaler

#### 2. Handling Imbalanced Data

* Used SMOTE (Synthetic Minority Over-sampling Technique) to balance classes

#### 3. Model Development

The following models were implemented:

* Logistic Regression
* Support Vector Machine (SVM)
* Random Forest
* XGBoost

#### 4. Hyperparameter Tuning

* Applied GridSearchCV for optimizing model parameters

---

### 📈 Model Performance

| Model               | Accuracy   |
| ------------------- | ---------- |
| Logistic Regression | 75.32%     |
| SVM                 | 81.17%     |
| Random Forest       | 84.42%     |
| XGBoost             | **87.66%** |

**Best Model:** XGBoost

---

### 📊 Evaluation Metrics (Final Model)

* Accuracy: 88.31%
* Precision: 81.03%
* Recall: 87.04%
* F1-Score: 83.93%

---

### 🔍 Key Insights

* Glucose and BMI are strong indicators of diabetes
* Ensemble methods outperform linear models
* SMOTE improves detection of minority class (diabetic cases)

---

### 🚀 Getting Started

#### Requirements

Install dependencies using:

```
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
```

#### Run the Project

1. Open `Diabetes_Prediction.ipynb` in Jupyter Notebook or Google Colab
2. Upload the dataset file (`diabetes.csv`)
3. Execute all cells sequentially

---

### 📁 Project Structure

```
Diabetes-Prediction/
│
├── Diabetes_Prediction.ipynb
├── diabetes.csv
├── best_model.pkl (optional)
├── scaler.pkl (optional)
└── README.md
```

---

⭐ Star this repository if you find it useful!
