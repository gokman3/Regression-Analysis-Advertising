# Advertising Sales Prediction: A Regression Analysis

This project explores the relationship between advertising expenditures across different channels (**TV, Radio, Newspaper**) and total **Sales**. Using various regression techniques, the model aims to predict future sales performance based on marketing budgets.

## 🚀 Project Overview
The primary goal is to determine which advertising mediums are most effective and to build a predictive model using:
* **Simple Linear Regression**
* **Ridge Regression (L2 Regularization)**
* **Lasso Regression (L1 Regularization)**

## 📊 Dataset Features
The dataset consists of 200 observations with the following features:
- **TV**: Advertising dollars spent on TV.
- **Radio**: Advertising dollars spent on Radio.
- **Newspaper**: Advertising dollars spent on Newspaper.
- **Sales (Target)**: Sales of a single product (in thousands of units).

## 🛠️ Key Steps
1. **Data Exploration:** Initial review, checking for null values, and descriptive statistics.
2. **Preprocessing:** Feature scaling using `StandardScaler` and splitting data into training (80%) and testing (20%) sets.
3. **Model Training:** Training Linear, Ridge, and Lasso models.
4. **Hyperparameter Tuning:** Using `GridSearchCV` to find the optimal alpha values for Ridge and Lasso.
5. **Evaluation:** Comparing models using **RMSE**, **MAE**, and **R² Score**.

## 📈 Results & Insights
* **Best Model:** Linear and Ridge regression performed almost identically, achieving an **R² score of ~0.90**.
* **Feature Importance:** **TV advertising** is the strongest predictor of sales, followed by Radio.
* **Lasso Selection:** Lasso Regression successfully identified that **Newspaper advertising** has a negligible impact on sales, setting its coefficient to zero.
* **Generalization:** Cross-validation confirmed that the model is robust and not overfitting.

## 💻 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
