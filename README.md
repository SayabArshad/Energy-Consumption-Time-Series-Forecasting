# Task-3-Energy-Consumption-Time-Series-Forecasting

## ✅ Task Objective
To analyze historical sales data and build a model that forecasts future sales trends for better inventory and financial planning.

## 🔍 Our Approach
- Used the Global Superstore dataset and parsed the Order Date column to create a time series by aggregating monthly sales.
- Visualizations revealed seasonal patterns, upward trends, and occasional dips.
- Preprocessing included resampling to monthly sales and filling missing values.
- Forecasting was done using both ARIMA and Facebook Prophet:
  - ARIMA was tuned using AIC and residual analysis.
  - Prophet handled seasonality and trend components more efficiently.
- Models were evaluated using Mean Absolute Error (MAE) and visual comparison.

## 📊 Results and Findings
- Facebook Prophet outperformed ARIMA due to its ability to model holidays and seasonal components.
- The forecast predicted sales peaks during November and December, likely due to holiday seasons.
- Business can now use this forecast to plan promotions, staffing, and inventory accordingly.
