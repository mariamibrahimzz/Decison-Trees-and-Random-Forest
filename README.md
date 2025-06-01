# 🧠 HR Attrition Analysis with Decision Trees & Random Forest

## 📍 Overview

This project leverages **Decision Tree** and **Random Forest** models to analyze and predict employee attrition using the [IBM HR Analytics Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset). Through rigorous preprocessing, feature engineering, and model evaluation, this pipeline demonstrates hands-on application of supervised learning in solving real-world HR problems.

---

## 📦 Tools & Libraries Used

- `pandas`, `numpy` – Data preprocessing and manipulation  
- `matplotlib`, `seaborn` – Exploratory Data Analysis and visualizations  
- `scikit-learn` – Modeling, evaluation, and hyperparameter optimization  
- `LabelEncoder`, `GridSearchCV`, `RandomizedSearchCV` – Feature encoding and model tuning  
- `IPython.display`, `pydot`, `graphviz` – Decision tree visualization

---

## 🔍 Key Highlights

### 🔧 Data Preprocessing
- Removed irrelevant and constant columns (`EmployeeCount`, `EmployeeNumber`, `Over18`, `StandardHours`)
- Encoded categorical features using `LabelEncoder`
- Converted the target `Attrition` into numerical binary labels

### 🌲 Decision Tree Classifier
- Trained baseline Decision Tree model
- Applied `GridSearchCV` for hyperparameter tuning:
  - `criterion`, `splitter`, `max_depth`, `min_samples_split`, `min_samples_leaf`
- Visualized the final tree using `export_graphviz` and `pydot`

### 🌳 Random Forest Classifier
- Trained with 100+ estimators for ensemble learning
- Performed hyperparameter optimization using:
  - `RandomizedSearchCV` and `GridSearchCV`
  - Tuned parameters: `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `bootstrap`
- Evaluated using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-Score)

---

## 📈 Model Evaluation

A custom `print_score()` function was implemented to display:

- **Training vs Testing Results**
- **Confusion Matrices**
- **Classification Reports**
- **Overfitting Indicators**

Comparative evaluation showed **Random Forest** outperforming baseline models in both precision and recall.

---

## 💡 Outcome

With powerful tree-based classifiers and optimized hyperparameters, the models achieved strong generalization in predicting attrition. This project stands as a showcase of practical machine learning workflows and thoughtful model tuning using Scikit-learn.

---

## 📁 Dataset

> [IBM HR Analytics Attrition Dataset on Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

## 🚀 Author

**Mariam Ibrahim**  
Aspiring Embedded Systems & Data Science Engineer  


