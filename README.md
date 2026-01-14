
# ⚡ Electricity Consumption Prediction using Linear Regression

## 📌 Project Overview

This project predicts **household electricity consumption** using **Linear Regression** based on historical numerical energy data.
It demonstrates a **complete machine learning pipeline**, including data preprocessing, feature scaling, model training, prediction, and evaluation.

The project is implemented in **Python** and executed on **Google Colab**, using the **UCI Electric Power Consumption Dataset**.

---

## 📂 Dataset Information

* **Source:** UCI Machine Learning Repository (via Kaggle)
* **Dataset Name:** Individual Household Electric Power Consumption
* **Link:**
  [https://www.kaggle.com/datasets/uciml/electric-power-consumption-data-set](https://www.kaggle.com/datasets/uciml/electric-power-consumption-data-set)

### 📊 Dataset Description

The dataset contains time-series measurements of electric power consumption in a single household.
Only **numerical features** are used in this project.

---

## 🧾 Features Used

**Input Features (Independent Variables):**

* Voltage
* Global Intensity
* Sub Metering 1
* Sub Metering 2
* Sub Metering 3

**Target Variable (Dependent Variable):**

* Global Active Power (Electricity Consumption)

---

## 🛠️ Tools & Technologies

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Kaggle Dataset

---

## 🔍 Methodology

1. Load dataset into Google Colab
2. Handle missing values (`?` replaced and removed)
3. Select numerical features
4. Convert columns to numeric data types
5. Apply **Standard Scaling**
6. Split data into:

   * 70% Training
   * 30% Testing
7. Train **Linear Regression Model**
8. Predict continuous electricity consumption values
9. Evaluate model performance
10. Visualize actual vs predicted values

---

## 📈 Model Evaluation

### 🔹 Regression Prediction

The model predicts **continuous electricity consumption values** using Linear Regression.

### 🔹 Binary Evaluation (Optional)

For demonstration purposes, predicted values are converted into:

* **High Consumption**
* **Low Consumption**

This is done using the **mean of the target variable as a threshold**, allowing the use of:

* Accuracy
* Confusion Matrix
* Classification Report

> ⚠️ Note:
> Accuracy and confusion matrix are **classification metrics**.
> For regression problems, metrics such as **R², MAE, and MSE** are more appropriate.
> Binary evaluation is included only to demonstrate classification-style analysis.

---

## ✅ Results

* **Accuracy:** **99.44%**
* Model shows **strong predictive performance**
* Predictions are well-aligned with actual consumption values
* Scatter plot confirms a strong linear relationship

---

## 📊 Visualization

The following visualization is included:

* **Actual vs Predicted Electricity Consumption Scatter Plot**

This helps verify how closely the model predictions match real values.

---

## 📁 Project Structure

```
📦 Electricity-Consumption-Prediction
 ┣ 📜 electricity_prediction.ipynb
 ┣ 📜 household_power_consumption.csv
 ┣ 📜 README.md
```

---

## 🚀 How to Run (Google Colab)

1. Upload `household_power_consumption.csv` to Colab
2. Open the notebook
3. Update file path if needed:

   ```python
   data = pd.read_csv('/content/household_power_consumption.csv',
                      sep=';', low_memory=False, na_values='?')
   ```
4. Run all cells

---

## 👩‍💻 Author

**Aayat Akhris**
🔗 GitHub: [https://github.com/ayatakhris15](https://github.com/ayatakhris15)

---

## ⭐ Final Notes

* This project is suitable for **ML coursework, semester projects, and beginner ML portfolios**
* Clean, simple, and well-structured Linear Regression implementation
* Easily extendable using advanced models (Ridge, Lasso, XGBoost, LSTM)


