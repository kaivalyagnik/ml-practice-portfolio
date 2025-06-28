# 🧠 Machine Learning Practice Portfolio

Welcome to my **Machine Learning Practice Portfolio** — a curated collection of end-to-end projects across various regression and classification problems.

Each dataset project includes:
- 📃 A problem statement and evaluation metrics
- 📊 Model training and testing results
- 🔍 Key takeaways and insights

---

## 🔍 Key Takeaways

### ✅ California Housing
- **Random Forest** and **XGBoost** outperform Linear Regression significantly.
- Default Random Forest already gave a strong RMSE of ~48910.
- Tuning didn’t improve performance much—suggesting default parameters were well-balanced.

### ✅ Insurance Charges
- **Random Forest with One-Hot Encoding** gave the best overall performance.
- **One-Hot Encoding** consistently outperformed **Ordinal** in both linear and tree models.
- **XGBoost** was robust and less sensitive to encoding types.
- **Linear Regression** benefitted marginally from One-Hot Encoding but lagged behind ensembles.

### ✅ Heart Disease Classification
- **Logistic Regression (Fine-Tuned)** achieved the best accuracy (88.6%) and recall (93%) for detecting heart disease.
- **Random Forest (Default)** also performed well (accuracy ~87%), but tuned version slightly underperformed, indicating over-tuning risk.
- **GridSearchCV with StratifiedKFold** ensured robust tuning and evaluation.
- **Logistic Regression** remains a strong choice for interpretable and high-performing models on structured binary classification tasks.

---

## 📂 Project List

| Dataset Name           | Type         | Problem Description                                | Models Used                                | Notebook Link                                                                 |
|------------------------|--------------|----------------------------------------------------|---------------------------------------------|--------------------------------------------------------------------------------|
| California Housing     | Regression   | Predict house prices in California based on census data. | Linear Regression, Random Forest, XGBoost  | [🔗 View](https://colab.research.google.com/github/kaivalyagnik/ml-practice-portfolio/blob/main/california_housing_regression.ipynb) |
| Insurance Charges      | Regression   | Predict individual insurance charges using features like age, BMI, region, smoker status. | Linear, Decision Tree, Random Forest, XGBoost       | [🔗 View](https://colab.research.google.com/github/kaivalyagnik/ml-practice-portfolio/blob/main/insurance_charges_regression.ipynb#scrollTo=CP9uPmFXHmwE) |
| Heart Disease          | Classification   | Classify whether a patient has heart disease based on clinical and demographic features. | Logistic Regression, Random Forest      | [🔗 View](https://colab.research.google.com/drive/1wkLOF0s1YwpXrI5qdOk4UIT9AwUK44Gt?authuser=0#scrollTo=81cUOSK4yIZn) |

---

## 📊 Model Evaluation Summary (California Housing)

| Model                          | RMSE      | R² Score | Notes                                      |
|-------------------------------|-----------|----------|--------------------------------------------|
| Linear Regression             | ~70000    | 0.62     | Simple baseline                            |
| Random Forest (default)       | 48910     | 0.82     | Best performing so far                     |
| Random Forest (tuned)         | 50330     | 0.80     | Slightly worse than default                |
| XGBoost Regressor  (tuned)    | 48062 | 0.82 | Accurate and efficient gradient boosting   |


📈 Insurance Charges

| Model              | Encoding Type | RMSE      | R² Score | Notes                                       |
|-------------------|---------------|-----------|----------|---------------------------------------------|
| Linear Regression  | Ordinal       | 5799.59   | 0.783    | Slightly worse than One-Hot                 |
| Linear Regression  | One-Hot       | 5796.28   | 0.784    | Best linear model encoding                  |
| Decision Tree      | Ordinal       | 7000.15   | 0.684    | Weakest model overall                       |
| Decision Tree      | One-Hot       | 6162.92   | 0.755    | One-Hot helps trees too                     |
| Random Forest      | Ordinal       | 4591.37   | 0.864    | Very strong — encoding didn’t hurt          |
| Random Forest      | One-Hot       | 4588.23   | 0.864    | Best overall performer                      |
| XGBoost            | Ordinal       | 4819.85   | 0.850    | Strong even with ordinal encoding           |
| XGBoost            | One-Hot       | 4738.61   | 0.855    | Best XGBoost result                         |


## 🧪 Model Comparison: Default vs Fine-Tuned (Heart Disease Classification)

### 📊 Evaluation Summary

| Model                     | Accuracy | Recall (Class 1) | F1-Score (Class 1) | Macro F1 | Notes                        |
|---------------------------|----------|------------------|--------------------|----------|-----------------------------|
| Logistic Regression       | 0.869    | 0.93             | 0.90               | 0.88     | Default parameters          |
| Logistic Regression (Tuned)| **0.886**| **0.93**         | **0.90**           | **0.88** | Slight improvement with tuning |
| Random Forest             | **0.870**| 0.89             | 0.88               | 0.87     | Default parameters          |
| Random Forest (Tuned)     | 0.848    | **0.90**         | 0.87               | 0.84     | Tuning slightly reduced performance |


## 🧭 Purpose

This portfolio is designed to:
- Strengthen my hands-on understanding of real-world ML problems
- Document model experimentation and evaluation strategies
- Build a transparent and professional GitHub presence

---

## 🚧 Work in Progress

Upcoming additions:
- Student Exam Score Predictor

Stay tuned! 🚀

---

## 📬 Feedback & Suggestions

Feel free to raise issues, suggest improvements, or connect with me on [LinkedIn](https://www.linkedin.com/in/kaival-yagnik-16185728b).

