# 📉 Customer Churn Prediction

This project aims to predict customer churn and provide actionable insights to reduce churn risk using interpretable machine learning models.

## 🧭 Objective

Churn can be costly for businesses. This project focuses on:

- Identifying customers at high risk of churn
- Prioritizing recall to ensure we capture the most potential churners
- Leveraging model interpretability tools (e.g., SHAP) to understand key churn drivers
- Creating a reusable modeling pipeline for future applications

---

## 🛠️ Tools & Technologies

- **Python** (pandas, numpy, matplotlib, seaborn)
- **scikit-learn** (Logistic Regression, Decision Tree, Random Forest, Naive Bayes, XGBoost)
- **Imbalanced-learn** (SMOTE for oversampling)
- **SHAP** (Model explainability)
- **GridSearchCV** (Hyperparameter tuning)
- **Cross-validation** (StratifiedKFold, scoring='recall')

---

## 🧪 Workflow Summary

### 1. 📂 Data Preparation
- Feature encoding (One-hot encoding for categoricals)
- Train-test split
- Feature scaling (for applicable models)

### 2. 🧠 Modeling Pipeline
- Multiple models tested: Logistic Regression, Decision Tree, Random Forest, Naive Bayes, XGBoost
- SMOTE applied to address class imbalance
- Grid search for hyperparameter tuning
- Threshold optimization based on recall

### 3. 📊 Evaluation
- Metrics: Accuracy, Precision, Recall, F1 Score, ROC-AUC
- Cross-validation to validate recall across folds
- Model selection based on business-prioritized metric (recall)

### 4. 🔍 Interpretability
- SHAP values used to understand feature contributions
- Insights extracted to support retention strategies

---

## 🎯 Business Impact

By prioritizing **recall**, this model minimizes the risk of missing churners, ensuring the business can act on the most at-risk customers. Model explanations support non-technical stakeholders in understanding the “why” behind predictions.

---

## 📌 Next Steps

- Integrate the model into a batch prediction pipeline
- Test with simulated retention strategies
- Extend project with AB testing to validate interventions
- Deploy as an API or simple dashboard
