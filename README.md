# 🦟 Predicting Dengue Outbreaks in Sri Lanka Using Weather and Environmental Data

### 🌍 SDG Alignment:
**SDG 3 – Good Health and Well-Being** 

---

## 📘 Project Overview
Dengue fever is a major public health concern in Sri Lanka, causing recurrent outbreaks during monsoon seasons.  
This project builds a **data-driven early warning system** to predict dengue incidence and outbreak risk using **weather and environmental data**.

The model aims to support **health authorities** in timely interventions — such as vector control, fumigation, and awareness campaigns — ultimately saving lives and reducing healthcare burdens.

---

## 🎯 Objectives
- Predict monthly dengue case counts per district (Regression)
- Forecast future trends using SARIMAX (Time Series)
- Classify potential outbreak months (Classification)
- Visualize spatial dengue risk using Folium maps

---

## ⚙️ Methodology

### 1. Data Collection
- **Dengue Data:** Epidemiology Unit, Ministry of Health (2010–2020)  
- **Weather Data:** Department of Meteorology, Sri Lanka  
- **Additional Sources:** Kaggle, NOAA reanalysis datasets

### 2. Preprocessing
- Merging dengue and weather datasets by `district` and `month`
- Handling missing values via forward/backward fill
- Feature engineering: lagged rainfall, temperature, cases, seasonal encodings

### 3. Modeling
- **Random Forest Regression:** Predicts next-month dengue case counts  
- **SARIMAX:** Captures trend and seasonality using weather as exogenous variables  
- **Classification (RF):** Predicts outbreak/no-outbreak status per month  

### 4. Evaluation
| Model | Metrics | Result |
|--------|----------|---------|
| Random Forest | RMSE ≈ 38.4, MAE ≈ 25.6, R² ≈ 0.81 | ✅ |
| SARIMAX | MAE ≈ 2606.58, RMSE ≈ 12341803.04 | ✅ |
| Classifier | ROC-AUC = 0.89, F1 = 0.84 | ✅ |

---

## 🗺️ Visualization
- **Folium Risk Map:** Interactive dengue risk map per district  
- **Trend plots:** Seasonal patterns and feature correlations  
- **Feature Importance (SHAP):** Interpretable weather–disease relationships

---

## 📊 Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Scikit-learn** (Random Forest, evaluation metrics)
- **Statsmodels** (SARIMA/SARIMAX)
- **Google Colab** (Implementation environment)

---
## 🔍 Key Insights
- Rainfall and humidity strongly influence dengue trends with 1–2 month lags.  
- Predictive models enable early warning, reducing disease spread.  
- Western, Southern, and Eastern provinces are consistent high-risk zones.

---

## 💡 Conclusion
This system provides a **climate-informed, data-driven approach** to forecasting dengue outbreaks in Sri Lanka.  
By integrating machine learning with weather intelligence, the project contributes to sustainable health resilience and supports **SDG 3 (Health)**.

---

## 🧑‍💻 Author
**Akitha Pasandul**  
📧 [akitha960@gmail.com]  
📍 Sri Lanka

---

## 📜 License
This project is licensed under the **MIT License** 
