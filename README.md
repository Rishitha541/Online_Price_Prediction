# Onion Price Prediction using Machine Learning & Deep Learning

## 📌 Overview
This project focuses on forecasting **onion prices** using modern **machine learning (ML)** and **deep learning (DL)** techniques.  
The dataset (`cleaned_onion_prices.csv`) contains historical onion price records from Warangal markets, with temporal features (day, month, year).  
The study compares three models:
- **Random Forest (RF)**
- **XGBoost**
- **Long Short-Term Memory (LSTM)**

---

## ⚙️ Methodology
- **Data Preprocessing**
  - Filled missing values using market averages.
  - Applied **MinMaxScaler** for feature scaling.
  - Engineered temporal features (Day, Month, Year).

- **Models Implemented**
  - **Random Forest** → Ensemble of decision trees, robust for structured tabular data.
  - **XGBoost** → Gradient boosting algorithm, optimized for precision forecasting.
  - **LSTM** → Sequential deep learning model for time-series prediction.

- **Evaluation Metrics**
  - Root Mean Squared Error (RMSE)
  - R² Score

---

## 📊 Results

| Model          | RMSE   | R² Score |
|----------------|--------|----------|
| LSTM           | 213.03 | -0.80    |
| Random Forest  | 157.58 | 0.99     |
| XGBoost        | 146.77 | 0.99     |

- **XGBoost** achieved the **lowest RMSE (146.77)** and highest accuracy, making it the best performer.  
- **Random Forest** also performed strongly, capturing structured data patterns effectively.  
- **LSTM** struggled with sharp price fluctuations, leading to higher error rates.

---

## 🔑 Key Insights
- Tree-based models (**RF & XGBoost**) outperform deep learning (LSTM) for volatile agricultural price data.
- **XGBoost** is the most reliable model for onion price forecasting in this dataset.
- Feature engineering (Day, Month, Year) significantly improved prediction accuracy.

---

## 🚀 Future Scope
- Incorporate **weather and climate data** for higher accuracy.
- Add **demand-supply metrics** and seasonal trends.
- Expand forecasting to other commodities (wheat, rice, pulses, vegetables).
- Develop a **mobile/web application** for farmers with real-time price predictions and crop recommendations.
- Integrate **IoT sensor data** (soil, rainfall, temperature) for precision agriculture.
- Explore **hybrid AI models** combining ML and DL for improved robustness.
