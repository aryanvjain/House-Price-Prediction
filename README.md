# House Price Prediction using Machine Learning

<p align="center">
An end-to-end Machine Learning project that predicts residential house prices using the Ames Housing Dataset. This project demonstrates the complete supervised learning workflow, including data preprocessing, feature engineering, model building, evaluation, and Kaggle submission.

**Final Kaggle Public Score: 0.14413**

</p>

---

# Project Overview

House prices are influenced by numerous factors such as location, overall quality, living area, garage capacity, basement area, neighborhood, and several other property characteristics.

The objective of this project is to build an accurate regression model capable of predicting house prices using these features while demonstrating a complete machine learning workflow—from raw data exploration to final model deployment.

---

# Dataset

* **Dataset:** Ames Housing Dataset
* **Source:** Kaggle – House Prices: Advanced Regression Techniques
* **Training Samples:** 1460
* **Test Samples:** 1459
* **Target Variable:** `SalePrice`
* **Original Features:** 79

---

# Machine Learning Workflow

```text
Load Dataset
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Missing Value Treatment
      │
      ▼
Feature Engineering
      │
      ▼
Ordinal Encoding
      │
      ▼
One-Hot Encoding
      │
      ▼
Train / Validation Split
      │
      ▼
Model Training
      │
      ▼
Model Evaluation
      │
      ▼
Random Forest Selected
      │
      ▼
Retrain on Complete Dataset
      │
      ▼
Kaggle Submission
```

---

# Exploratory Data Analysis

Several visualizations were created to understand the dataset and identify relationships between housing features and sale prices.

The analysis included:

* Correlation Heatmap
* Overall Quality vs Sale Price
* Living Area vs Sale Price
* Garage Capacity vs Sale Price
* Basement Area vs Sale Price

> Add screenshots of these visualizations inside the `images/` folder and embed them here to showcase the analysis.

---

# Data Preprocessing

The following preprocessing techniques were applied before model training.

### Missing Value Handling

* Removed features with excessive missing values
* Filled numerical missing values using statistical methods
* Filled categorical missing values using appropriate category labels

### Feature Encoding

Two encoding techniques were used:

* **Ordinal Encoding** for ordered categorical features
* **One-Hot Encoding** for nominal categorical features

Finally, both training and testing datasets were transformed into identical feature spaces before model training.

---

# Models Implemented

Three regression models were trained and compared.

| Model                   | Purpose                                       |
| ----------------------- | --------------------------------------------- |
| Linear Regression       | Baseline model                                |
| Decision Tree Regressor | Capture non-linear relationships              |
| Random Forest Regressor | Improve generalization and reduce overfitting |

---

# Model Performance

| Model             |        MAE |       RMSE |  R² Score |
| ----------------- | ---------: | ---------: | --------: |
| Linear Regression |     19,748 |     49,408 |     0.562 |
| Decision Tree     |     22,446 |     32,371 |     0.812 |
| **Random Forest** | **14,715** | **21,750** | **0.915** |

Random Forest consistently outperformed the other models across all evaluation metrics and was therefore selected as the final model.

---

# Final Results

| Metric              | Result                  |
| ------------------- | ----------------------- |
| Final Model         | Random Forest Regressor |
| Kaggle Public Score | **0.14413**             |
| Evaluation Metrics  | MAE, RMSE, R² Score     |

---

# Repository Structure

```text
House-Price-Prediction
│
├── notebook/
│   └── house-price-prediction.ipynb
│
├── data/
│   ├── train.csv
│   ├── test.csv
│   ├── sample_submission.csv
│   └── data_description.txt
│
├── images/
│   ├── github-banner.png
│   ├── heatmap.png
│   └── overallqual_vs_saleprice.png
│
├── results/
│   └── submission.csv
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

# Getting Started

Clone the repository:

```bash
git clone https://github.com/aryanvjain/House-Price-Prediction.git
```

Move into the project directory:

```bash
cd House-Price-Prediction
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* Kaggle


# Key Learnings

This project strengthened my understanding of:

* Exploratory Data Analysis (EDA)
* Missing Value Treatment
* Feature Engineering
* Ordinal Encoding and One-Hot Encoding
* Regression Algorithms
* Model Evaluation Metrics (MAE, RMSE, R²)
* Hyperparameter Selection
* End-to-End Machine Learning Workflow
* Kaggle Model Submission


# Future Improvements

Potential enhancements include:

* Hyperparameter tuning using GridSearchCV or RandomizedSearchCV
* Cross-validation
* Feature selection
* Log transformation of the target variable
* Gradient Boosting models (XGBoost, LightGBM, CatBoost)
* Model explainability using SHAP

---

# Author

**Aryan Jain**

* GitHub: https://github.com/aryanvjain
* LinkedIn: www.linkedin.com/in/aryan-vineet-jain

---

If you found this project useful, consider giving the repository a star.
