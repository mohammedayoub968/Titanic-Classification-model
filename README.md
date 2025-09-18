# Titanic Survival Prediction

This project aims to predict the survival of passengers on the Titanic using machine learning models. The analysis is based on the Titanic dataset from Kaggle.

---

## 🔹 Project Overview

The goal of this project is to build a predictive model that accurately determines whether a passenger survived the Titanic disaster. The project involves data exploration, data cleaning, feature engineering, and building and evaluating several classification models.

---

## 🔹 Dataset

The dataset used in this project is the "Titanic-Dataset.csv" from Kaggle. It contains information about the passengers on the Titanic, such as their age, sex, class, and whether they survived or not.

---

## 🔹 Methodology

The project follows these steps:
1.  **Data Loading and Exploratory Data Analysis (EDA)**: The dataset is loaded, and an initial analysis is performed to understand the data's structure and features.
2.  **Data Cleaning and Preprocessing**: Missing values in the 'Age' and 'Embarked' columns are handled. The 'Cabin' feature is dropped due to a high percentage of missing values. Inconsistent 'Fare' values (equal to zero) are removed.
3.  **Model Building**: Several classification models are trained on the preprocessed data:
    * Logistic Regression
    * Support Vector Classifier (SVC)
    * Random Forest
    * XGBoost
4.  **Model Evaluation**: The performance of the models is compared based on accuracy scores, with and without feature scaling and selection.

---

## 🔹 Results

The following table summarizes the performance of the different models:

| Model               | Accuracy (Baseline) | Accuracy (with Scaling) | Accuracy (with Feature Selection) |
| ------------------- | ------------------- | ----------------------- | --------------------------------- |
| Logistic Regression | 0.7670              | 0.7670                  | 0.7670                            |
| SVC                 | 0.8068              | 0.8068                  | 0.8068                            |
| Random Forest       | 0.7557              | 0.7557                  | 0.7898                            |
| XGBoost             | 0.7330              | 0.7330                  | 0.7614                            |

---

## 🔹 Insights

* **Logistic Regression**: Performance remained constant across all scenarios.
* **SVC (Support Vector Classifier)**: Achieved the **highest accuracy (0.807)** and was not affected by scaling or feature selection, showing robustness in this dataset.
* **Random Forest**: Improved significantly after **Feature Selection** (from 0.756 to 0.790).
* **XGBoost**: Started weaker but improved with **Feature Selection**.

---

## 🔹 Conclusion

* **SVC** delivered the best overall performance.
* **Feature Selection** had the largest positive effect on **tree-based models** (Random Forest and XGBoost).
* **Scaling (RobustScaler)** had little impact in this case.

---

## 🔹 How to run the code

1.  Download the `titanic-analysis-models.ipynb` file.
2.  Ensure you have the "Titanic-Dataset.csv" file in the same directory.
3.  Open the notebook in a Jupyter environment.
4.  Run the cells sequentially to reproduce the analysis and results.
