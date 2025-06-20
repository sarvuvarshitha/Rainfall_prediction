# Rainfall_prediction
Web-based rainfall predictor using ML with 10-day input and 5-day forecast, built in 4 weeks to improve early warnings and climate resilience.
---

## 🌧️ Rainfall Prediction Using Machine Learning

### 📌 Project Overview

This project aims to predict short-term rainfall using historical climate data by applying machine learning techniques. A clean dataset covering multiple years and Indian divisions is used to analyze seasonal rainfall patterns and predict future rainfall to assist in planning and early warning systems.

---

### 📊 Dataset Description

* **Source**: Historical rainfall dataset
* **Columns**:

  * `DIVISION`, `YEAR`, `JAN`, `FEB`, ..., `DEC`, `ANNUAL`
* **Scope**: Covers various regions in India from **1901 to 2017**
* **Purpose**: Used to build an ML model for predicting rainfall based on past values

---

### 🔍 Project Workflow

1. **Data Loading & Cleaning**

   ```python
   import pandas as pd
   d = pd.read_csv('/content/rainfall_prediction(1).csv')
   print(d.head())
   ```

2. **Feature Engineering**

   * Monthly rainfall data used as features
   * Aggregated annual and seasonal trends
   * Handled missing values and outliers

3. **Model Selection**

   * Regression-based model chosen
   * Tried multiple ML algorithms: `Linear Regression`, `Random Forest`, `Decision Tree`
   * Final model selected based on R² score and RMSE

4. **Training and Evaluation**

   ```python
   from sklearn.model_selection import train_test_split
   from sklearn.ensemble import RandomForestRegressor
   ```

   * Training set: 80%
   * Testing set: 20%
   * Evaluation metrics:

     * R² Score
     * Mean Absolute Error
     * Root Mean Squared Error

5. **Prediction Example**

   ```python
   model.predict([[jan, feb, ..., dec]])
   ```

6. **Visualization**

   * Actual vs Predicted rainfall plots
   * Regional rainfall trends over the years

---

### 🛠️ Tools & Technologies

* **Language**: Python
* **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
* **Platform**: Google Colab / Jupyter Notebook

---

### ✅ Key Outcomes

* Successfully trained and validated rainfall prediction models
* Demonstrated model accuracy using R² and error metrics
* Visual insights into rainfall variation across Indian regions
* Built a pipeline for seasonal rainfall forecasting using historical data

---

### 🚀 Future Work

* Integrate real-time data via weather APIs
* Develop a web interface using Flask
* Use LSTM for sequential rainfall prediction
* Extend prediction to drought/flood forecasting

---

### 📁 Repository Structure

```
Rainfall-Prediction-ML/
├── rainfall_prediction.ipynb
├── rainfall_prediction.csv
├── Rainfall_Prediction_Report.md
├── model.pkl
└── README.md
```

---

### 🙋‍♀️ Author

**Sarvu Varshitha**
B.Tech 3rd Year, Computer Science Engineering
SR University

---




