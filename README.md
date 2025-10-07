# ⚡ Energy Consumption Time Series Forecasting

## ✅ Task Objective  
To analyze historical **energy consumption data** and build a **forecasting model** that predicts future consumption trends for efficient **resource management**, **inventory planning**, and **financial forecasting**.

---

## 🔍 Our Approach  

### 1️⃣ Dataset Preparation  
- Used an **Energy Consumption dataset** (hourly/daily readings).  
- Parsed the **Date/Time column** to create a time-indexed series.  
- Aggregated data to **monthly consumption** for trend analysis.  

### 2️⃣ Exploratory Data Analysis (EDA)  
- Visualized consumption trends over time.  
- Identified **seasonal peaks**, **cyclical patterns**, and **anomalies**.  
- Observed higher energy usage during **summer and winter months**, suggesting temperature dependency.

### 3️⃣ Data Preprocessing  
- Resampled data to **monthly intervals** using `pandas.resample('M')`.  
- Filled missing values using **forward fill** or **interpolation**.  
- Ensured stationarity for ARIMA using **differencing** if required.

### 4️⃣ Forecasting Models  
- **ARIMA Model**  
  - Tuned parameters `(p, d, q)` using **AIC minimization** and residual analysis.  
  - Captured trend but limited in handling strong seasonality.  

- **Facebook Prophet**  
  - Automatically modeled **trend**, **seasonality**, and **holidays**.  
  - Handled complex seasonal behavior efficiently.  
  - Provided intuitive visualizations and future predictions.

### 5️⃣ Model Evaluation  
- Evaluated models using:  
  - **Mean Absolute Error (MAE)**  
  - **Root Mean Squared Error (RMSE)**  
  - **Visual forecast comparison** with actual data.  

---

## 📊 Results and Findings  

| Model | MAE | Performance Notes |
|--------|------|------------------|
| ARIMA | Moderate | Struggled with seasonal fluctuations |
| Prophet | **Best** | Effectively captured yearly seasonality and trend |

- **Facebook Prophet outperformed ARIMA** due to its ability to model complex seasonality and trend patterns.  
- Forecasts indicate **peak energy consumption during summer and winter**, aligning with heating/cooling demands.  
- Businesses and utility providers can use this forecast for:  
  - **Demand planning**  
  - **Infrastructure scaling**  
  - **Energy cost optimization**

---

## ⚙️ Tools & Libraries Used  
- **Python**  
- **Pandas**  
- **Matplotlib**  
- **Seaborn**  
- **Statsmodels (ARIMA)**  
- **Facebook Prophet**

---

## 📂 Files Included  
| File Name | Description |
|------------|-------------|
| `Task-04.ipynb` | Jupyter Notebook containing full code, analysis, and results |
| `README.md` | This documentation file |

---

## 🚀 How to Run This Project  

### 1️⃣ Clone this repository:
```bash
git clone https://github.com/SayabArshad/Energy-Consumption-Time-Series-Forecasting.git
cd Energy-Consumption-Time-Series-Forecasting
