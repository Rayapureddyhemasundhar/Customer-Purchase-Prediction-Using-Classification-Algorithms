# Customer Purchase Prediction - Machine Learning Project

## Project Overview

This project builds a classification model to predict whether a customer will purchase a product based on their demographic and behavioral data. The project compares multiple machine learning algorithms to find the best-performing model.

---

# Dataset Information

The dataset contains **1000 customer records** with the following features:

| Feature | Description |
|---------|-------------|
| **Age** | Customer age (18–65 years) |
| **Gender** | Male/Female (encoded to 0/1) |
| **Annual Income** | Customer income (20,000–120,000) |
| **Spending Score** | Customer spending behavior (1–100) |
| **Previous Purchases** | Number of previous purchases (0–20) |
| **Website Visits** | Number of website visits (1–50) |
| **Time on Site** | Minutes spent on website (1–30) |
| **Purchase** | Target variable (0 = No Purchase, 1 = Purchase) |

---

# Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
joblib
```

Install all dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

---

# Project Structure

```text
├── customer_purchase_prediction.ipynb    # Main notebook
├── best_model.pkl                        # Saved best model
└── README.md                             # Project documentation
```

---

# How to Run

### 1. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

### 2. Launch Jupyter Notebook

```bash
jupyter notebook customer_purchase_prediction.ipynb
```

### 3. Execute all cells

Run every notebook cell sequentially from top to bottom.

---

# Project Workflow

## 1. Data Preprocessing

- Encoded **Gender** using `LabelEncoder`
- Standardized features using `StandardScaler`
- Split the dataset:
  - **80% Training**
  - **20% Testing**

---

## 2. Exploratory Data Analysis (EDA)

Performed:

- Distribution plots
- Correlation heatmap
- Feature importance analysis
- Purchase behavior analysis

---

## 3. Machine Learning Models

| Model | Description |
|--------|-------------|
| Logistic Regression | Baseline linear classifier |
| Decision Tree | Tree-based classifier (`max_depth=5`) |
| Random Forest | Ensemble model (`n_estimators=50`) |
| K-Nearest Neighbors | Distance-based classifier (`k=5`) |

---

## 4. Evaluation Metrics

The following metrics were used to evaluate model performance:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# Results Summary

## Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score |
|--------|---------:|----------:|-------:|---------:|
| Logistic Regression | ~0.60 | ~0.60 | ~0.70 | ~0.65 |
| Decision Tree | ~0.58 | ~0.60 | ~0.65 | ~0.62 |
| Random Forest | **~0.62** | **~0.62** | **~0.72** | **~0.67** |
| K-Nearest Neighbors | ~0.55 | ~0.57 | ~0.60 | ~0.58 |

> **Note:** Exact values may vary because the dataset is randomly generated.

---

# Best Model

🏆 **Random Forest** achieved the highest overall performance with the best Accuracy and F1-Score.

---

# Key Insights

- Spending Score is one of the strongest indicators of future purchases.
- Previous Purchases significantly improve prediction accuracy.
- Annual Income has a moderate relationship with purchasing behavior.
- Customers who spend more time on the website and visit frequently are more likely to purchase.

---

# Business Recommendations

- Target customers with high spending scores.
- Improve website engagement through better content and recommendations.
- Deploy the Random Forest model for customer purchase prediction.
- Collect additional customer information such as:
  - Customer satisfaction
  - Product preferences
  - Seasonal purchasing behavior

---

# Learning Outcomes

This project demonstrates:

- Data preprocessing
- Feature encoding
- Feature scaling
- Exploratory Data Analysis (EDA)
- Classification algorithms
- Model evaluation
- Model comparison
- Saving trained models
- Business interpretation of machine learning results

---

# Future Improvements

Potential enhancements include:

- Feature engineering
- Hyperparameter tuning using `GridSearchCV`
- Cross-validation
- Class imbalance handling
- Advanced algorithms:
  - XGBoost
  - LightGBM
  - CatBoost
  - Neural Networks
- Deploying the model using:
  - Flask
  - FastAPI
  - Streamlit

---

# License

This project is intended for **educational purposes only**.

---

# Author

**Machine Learning Intern**

Beginner → Intermediate Level Machine Learning Project
