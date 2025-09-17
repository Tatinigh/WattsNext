# ⚡ WattsNext
**Forecast tomorrow’s energy demand today: enabling sustainable, carbon-aware buildings**  

## 📖 Overview  
Energy consumption accounts for nearly one-third of global energy use. Accurate forecasting is critical for reducing waste and enabling smarter, sustainable energy systems.  

**WattsNext** is a time series forecasting project focused on short-term energy demand prediction across Indian states. By leveraging historical load data (2013–2023), the project builds a foundation for carbon-aware, data-driven energy planning.  

---

## 🛠️ Solution Approach  

1. **Data Exploration & Cleaning**  
   - Historical load data (2013–2023)  
   - Removed duplicates, handled missing values, and filtered outliers  

2. **Stationarity Checks**  
   - Applied **Augmented Dickey-Fuller (ADF)** test to confirm stationarity  

3. **Modeling**  
   - Experimented with **ARIMA** for capturing temporal trends and spikes  
   - Used **ACF/PACF** plots for parameter tuning  
   - Found weak autocorrelation in dataset → ARIMA forecasts lacked accuracy  

4. **Validation**  
   - Used rolling forecasts  
   - Evaluated accuracy with **MAE** and **RMSE**  

5. **Visualization**  
   - Comparative plots of actual vs. predicted load  
   - Insights into model behavior and performance gaps  

---

## 📂 Dataset  
- **Source:** [Daily Power Generation in India (2013–2023) – Kaggle](https://www.kaggle.com/datasets/krishnadaskv/daily-power-generation-in-india-2013-2023)  

---

## 📚 Tools & Libraries  
- **Python** → Primary development language  
- **Pandas, NumPy** → Data preprocessing & cleaning  
- **Matplotlib** → Visualization  
- **Statsmodels** → ARIMA, ADF test, ACF & PACF plots  
- **Scikit-learn** → Error metric evaluation  
- **Jupyter Notebook** → Exploration & experimentation  

---

## 🎯 Expected Outcomes  
- A working **time series forecasting pipeline** for short-term energy demand across Indian states  
- Insights into **trade-offs** between classical statistical models and modern foundation models for forecasting  
- A **scalable foundation** for real-world applications supporting:  
  - Policy makers & building managers in demand planning  
  - Grid operators in aligning consumption with renewable energy availability  
  - Integration of anomaly detection for proactive energy management  

---

## 🚀 Future Extensions  
- Deploy **Time Series Foundation Models (TSFMs)** for improved generalization  
- Build **real-time anomaly detection** modules  
- Design **dashboards for smart city energy tracking**  
