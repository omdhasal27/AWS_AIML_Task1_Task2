# AWS_AIML_Task1_Task2
Practical AI/ML tasks, data preprocessing, and model implementations running in Google Colab.

# House Price Prediction - AI/ML Volunteer Recruitment Task

This repository contains my submission for **Task 1** and **Task 2** of the AI/ML Volunteer recruitment for the **AWS Student Builder Group at VIT Pune**.

---

## 📌 Task Overview

- **Task 1: Data Handling with NumPy and Pandas**
  - Generated a synthetic dataset of **250 houses** with columns: `area`, `bedrooms`, `age`, and `price` (in ₹).
  - Calculated summary statistics and inspected the dataset using Pandas.
  - Handled missing values by randomly removing ~5% of entries and imputing them using the **median**.
  - Converted data into NumPy arrays to compute `price_per_sqft` using vectorized operations.
  - Analyzed group averages using `.groupby()` and visualized relationships with Matplotlib plots.

- **Task 2: House Price Prediction with Linear Regression**
  - Selected `area` and `bedrooms` as input features ($X$) to predict house `price` ($y$).
  - Split the data into an **80/20 train-test split**.
  - Trained a `LinearRegression` model using `scikit-learn`.
  - Evaluated the model using **MAE**, **RMSE**, and **$R^2$ Score**.
  - Tested predictions on a sample home and plotted actual vs. predicted prices.

---

## 📊 Dataset Summary

- **Total Rows:** 250
- **Features Used:**
  - `area` (in sq ft)
  - `bedrooms` (BHK count: 1 to 4)
  - `age` (in years)
  - `price` (Target variable in Indian Rupees - ₹)

---

## 🔑 Key Observations (Task 1)

1. **Strongest Factor:** House `area` has the strongest positive correlation with house `price`.
2. **Missing Data Handling:** The median was preferred over the mean for filling missing values because it avoids bias caused by extreme outliers.
3. **Bedrooms Impact:** Adding extra bedrooms increases the house price predictably across the dataset.

---

## 📈 Model Performance & Results (Task 2)

- **Model:** Linear Regression (`scikit-learn`)
- **Train / Test Split:** 80% / 20%
- **Evaluation Metrics:**
  - **MAE:** Measurable average prediction error in Rupees (₹).
  - **$R^2$ Score:** Shows high correlation and explanation of price variations based on area and bedrooms.

### Sample Prediction:
- **Input:** 1,200 sq. ft. area, 3 bedrooms (3 BHK)
- **Predicted Price:** ~₹75,00,000 (₹75 Lakhs)

---

## 🛠️ Tools & Libraries Used

- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
- **Environment:** Google Colab / Jupyter Notebook
