# 🌳 Employee Attrition Prediction using Decision Tree & Random Forest

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical-blue?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

</p>

---

# 👨‍🎓 Student Information

| Field | Details |
|-------|---------|
| **Name** | Taran Ali Ahmed |
| **Registration Number** | 23BCE10952 |
| **Application Number** | IN26009846 |
| **Batch** | 2B |

---

# 📌 Project Objective

The objective of this project is to build machine learning models capable of predicting whether an employee is likely to leave the company (**Employee Attrition**).

Early prediction enables organizations to:

- Reduce employee turnover
- Improve retention strategies
- Lower hiring costs
- Increase workforce satisfaction

---

# 📂 Dataset

**IBM HR Analytics Employee Attrition & Performance Dataset**

🔗 https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

> **Note:** The dataset file is excluded from GitHub using `.gitignore`.

---

# 🛠 Technologies Used

| Library | Purpose |
|----------|----------|
| Pandas | Data Loading & Manipulation |
| NumPy | Numerical Operations |
| Scikit-Learn | Machine Learning |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Plots |

---

# 🔄 Project Workflow

```text
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Feature Encoding
   │
   ▼
Train/Test Split
   │
   ▼
Decision Tree
   │
   ├────────────┐
   ▼            ▼
Random Forest  Evaluation
        │
        ▼
Performance Comparison
```

---

# 📊 Data Preprocessing

✔ Checked missing values

✔ Removed constant columns

- EmployeeCount
- Over18
- StandardHours

✔ Removed identifier column

- EmployeeNumber

✔ Label Encoded categorical features

✔ Train-Test Split

- Training : **80%**
- Testing : **20%**

---

# 🤖 Models Implemented

## 🌳 Decision Tree Classifier

- Baseline Classification Model
- Default Hyperparameters

---

## 🌲 Random Forest Classifier

- Ensemble Learning
- 100 Decision Trees
- Bootstrap Sampling
- Majority Voting

---

# 📈 Model Performance

| Model | Accuracy | Precision | Recall | F1 Score |
|:------|:-------:|:---------:|:------:|:-------:|
| 🌳 Decision Tree | **78.23%** | 31.91% | **31.91%** | **31.91%** |
| 🌲 Random Forest | **84.35%** | **54.55%** | 12.77% | 20.69% |

---

# 📉 Visualizations

## Confusion Matrix

<p align="center">
<img src="confusion_matrices.png" width="750">
</p>

---

## Feature Importance

<p align="center">
<img src="rf_feature_importance.png" width="700">
</p>

---

# 📌 Model Comparison

| Metric | Decision Tree | Random Forest |
|---------|--------------|---------------|
| Accuracy | 78.23% | ⭐ **84.35%** |
| Precision | 31.91% | ⭐ **54.55%** |
| Recall | ⭐ **31.91%** | 12.77% |
| F1 Score | ⭐ **31.91%** | 20.69% |

---

# 🔍 Key Observations

### ✅ Random Forest

- Higher Accuracy
- Better Precision
- Reduced Overfitting
- More Robust Predictions

### ✅ Decision Tree

- Better Recall
- Higher F1 Score
- Easier Interpretation

---

# ⭐ Important Features

The Random Forest model identified the following features as the most influential:

🥇 MonthlyIncome

🥈 OverTime

🥉 Age

🏅 TotalWorkingYears

🏅 DailyRate

These variables significantly influence employee attrition.

---

# ⚙ Hyperparameter Tuning

## 🌳 Decision Tree

| Max Depth | Accuracy | Precision | Recall | F1 |
|-----------|----------|-----------|--------|------|
| 3 | 82.31% | 41.38% | 25.53% | 31.58% |
| **5** | **84.35%** | **52.94%** | 19.15% | 28.12% |
| 7 | 81.97% | 41.67% | **31.91%** | **36.14%** |
| 10 | 80.27% | 35.90% | 29.79% | 32.56% |
| None | 78.23% | 31.91% | 31.91% | 31.91% |

---

## 🌲 Random Forest

| Max Depth | Accuracy | Precision | Recall | F1 |
|-----------|----------|-----------|--------|------|
| 3 | 84.01% | 50.00% | 4.26% | 7.84% |
| 5 | 83.67% | 44.44% | 8.51% | 14.29% |
| 10 | 83.67% | 45.45% | 10.64% | 17.24% |
| **None** | **84.35%** | **54.55%** | **12.77%** | **20.69%** |

---

# 💡 Conclusions

### 🌳 Decision Tree

**Advantages**

- Easy to understand
- Interpretable
- Better Recall

**Limitations**

- High variance
- Overfits easily
- Lower overall accuracy

---

### 🌲 Random Forest

**Advantages**

- Higher Accuracy
- Better Precision
- Reduces Overfitting
- Stable Predictions

**Limitations**

- Lower Recall
- Less Interpretable
- Slightly Higher Computational Cost

---

# 🏆 Final Result

| Winner | Reason |
|---------|--------|
| 🥇 **Random Forest** | Highest Accuracy & Precision |
| 🥈 **Decision Tree** | Better Recall & Interpretability |

Random Forest is the preferred model for this dataset due to its superior predictive performance, while the Decision Tree remains useful for explainable AI and understanding decision rules.

---

# 📜 License

This project is developed for educational purposes as part of a Machine Learning assignment.
