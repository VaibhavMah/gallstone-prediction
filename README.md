# Gallstone Prediction using Clinical and Bioimpedance Data 🩺

This project uses clinical and bioimpedance features to predict the presence of gallstones using machine learning models.

## 🧪 Workflow

- Exploratory Data Analysis (EDA)
- Feature Selection using multiple techniques:
  - Mutual Information, Chi2, ANOVA, RFE, Lasso, SFS, XGBoost
- Final features selected from features appearing in ≥4 methods
- Logistic Regression model trained with:
  - Standard Scaling
  - Class Weight Balancing
  - ROC AUC + Recall tuning via threshold adjustment
- Evaluation: Accuracy, Recall, F1, ROC AUC
- Comparison with Random Forest and XGBoost
- Model saved using `pickle`
- Final deployment-ready prediction threshold: **0.40**

## 📈 Final Model (Logistic Regression)

- **ROC AUC:** 0.88
- **Accuracy:** 81%
- **Recall (Class 1):** 75%
- **Precision (Class 1):** 86%

## 🗂️ Files

- `gallstone_.csv` — Dataset (anonymized)
- `gallstone_model.ipynb` — Full notebook with feature selection, modeling, evaluation, and model saving
- `model.pkl` — Final trained model (with threshold wrapper)
- `README.md` — Project overview

---

## 📦 Requirements

- Python ≥ 3.7
- scikit-learn
- pandas
- numpy
- matplotlib / seaborn (for EDA)
