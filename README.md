# 🏡 House Price Prediction using Machine Learning

<p align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge\&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge\&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge\&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge\&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blueviolet?style=for-the-badge)
![Kaggle](https://img.shields.io/badge/Kaggle-Competition-20BEFF?style=for-the-badge\&logo=kaggle)

</p>

<p align="center">

An end-to-end Machine Learning project that predicts residential house prices using the Ames Housing Dataset.
The project covers the complete supervised learning pipeline including data preprocessing, feature engineering, model building, evaluation, and Kaggle submission.

**🏆 Final Kaggle Public Score: 0.14413**

</p>

---

# 📌 Project Overview

House prices are influenced by numerous factors such as location, overall quality, living area, garage capacity, basement area, neighborhood, and many other property characteristics.

The objective of this project is to build an accurate regression model capable of predicting house prices using these features while demonstrating a complete machine learning workflow—from raw data exploration to final model deployment.

---

# 📊 Dataset

* **Dataset:** Ames Housing Dataset
* **Source:** Kaggle - House Prices: Advanced Regression Techniques
* **Training Samples:** 1460
* **Test Samples:** 1459
* **Target Variable:** `SalePrice`
* **Original Features:** 79

---

# 🔄 Machine Learning Workflow

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

# 📈 Exploratory Data Analysis

Several visualizations were created to better understand the dataset and identify relationships between different housing features and sale prices.

The analysis included:

* Correlation Heatmap
* Overall Quality vs Sale Price
* Living Area vs Sale Price
* Garage Capacity vs Sale Price
* Basement Area vs Sale Price

> *(Add screenshots of these visualizations inside the `images/` folder and embed them here for a more attractive repository.)*

---

# ⚙️ Data Preprocessing

The following preprocessing techniques were applied before model training.

### ✔ Missing Value Handling

* Removed features with excessive missing values
* Filled numerical missing values using statistical methods
* Filled categorical missing values using appropriate category labels

### ✔ Feature Encoding

Two encoding techniques were used:

* **Ordinal Encoding** for ordered categorical features
* **One-Hot Encoding** for nominal categorical features

Finally, both training and testing datasets were transformed into identical feature spaces before model training.

---

# 🤖 Models Implemented

Three regression models were trained and compared.

| Model                   | Purpose                                       |
| ----------------------- | --------------------------------------------- |
| Linear Regression       | Baseline model                                |
| Decision Tree Regressor | Capture non-linear relationships              |
| Random Forest Regressor | Improve generalization and reduce overfitting |

---

# 📊 Model Performance

| Model             |        MAE |       RMSE |  R² Score |
| ----------------- | ---------: | ---------: | --------: |
| Linear Regression |     19,748 |     49,408 |     0.562 |
| Decision Tree     |     22,446 |     32,371 |     0.812 |
| **Random Forest** | **14,715** | **21,750** | **0.915** |

Random Forest consistently outperformed the other models across all evaluation metrics and was therefore selected as the final model.

---

# 🏆 Final Results

| Metric              | Result                  |
| ------------------- | ----------------------- |
| Final Model         | Random Forest Regressor |
| Kaggle Public Score | **0.14413**             |
| Evaluation Metrics  | MAE, RMSE, R² Score     |

---

# 📂 Repository Structure

```text
House-Price-Prediction
│
├── notebooks/
│   └── House_Price_Prediction.ipynb
│
├── data/
│   ├── train.csv
│   ├── test.csv
│   ├── sample_submission.csv
│   └── data_description.txt
│
├── images/
│
├── results/
│   └── submission.csv
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

# 🚀 Getting Started

Clone the repository

```bash
git clone https://github.com/aryanvjain/House-Price-Prediction.git
```

Move into the project directory

```bash
cd House-Price-Prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch the notebook

```bash
jupyter notebook
```

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* Kaggle

---

# 🎯 Key Learnings

This project strengthened my understanding of:

* Exploratory Data Analysis (EDA)
* Missing Value Treatment
* Feature Engineering
* Ordinal & One-Hot Encoding
* Regression Algorithms
* Model Evaluation Metrics
* Hyperparameters
* Machine Learning Workflow
* Kaggle Model Submission

---

# 🚀 Future Improvements

Some potential improvements include:

* Hyperparameter tuning using GridSearchCV or RandomizedSearchCV
* Cross Validation
* Feature Selection
* Log Transformation of the Target Variable
* Gradient Boosting Models (XGBoost, LightGBM, CatBoost)
* Model Explainability using SHAP

---

# 👨‍💻 Author

**Aryan Jain**

* GitHub: https://github.com/aryanvjain
* LinkedIn: *(Add your LinkedIn profile here)*

---

⭐ If you found this repository helpful, consider giving it a star!
