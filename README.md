# DATA-ANALYST-INTERNSHIP-Elevate-Labs-Task-16

# Sales Forecasting Project - Store Item Demand Forecasting

## Objectives
- Convert date column into proper datetime format
- Aggregate daily sales into monthly totals
- Visualize sales trends over time
- Analyze seasonality using rolling averages
- Split data into train and test sets based on time
- Apply Exponential Smoothing forecasting model
- Predict future sales values
- Evaluate model performance using MAE and MAPE
- Export forecast results as CSV

---

## Dataset
**Dataset Used:** Store Item Demand Forecasting  
**Main File:** `train.csv`

### Dataset Columns
- `date` - Sales date
- `store` - Store ID
- `item` - Item ID
- `sales` - Number of items sold

---

## Tools & Libraries
- Python
- Pandas
- Matplotlib
- NumPy
- Statsmodels
- Scikit-learn

---

## Project Workflow

### Data Loading & Preprocessing
- Loaded CSV dataset
- Converted `date` column to datetime
- Set date as index for time-series analysis

### Data Aggregation
- Resampled daily sales into **monthly sales**
- Used `groupby` and `resample()` for aggregation

### Trend Visualization
- Plotted monthly sales to observe long-term trends

### Seasonality Analysis
- Applied rolling mean to identify patterns and fluctuations

### Train/Test Split
- Used time-based split
- Last 6 months reserved as test dataset

### Forecasting Model
- Applied **Exponential Smoothing**
- Modeled trend component

### Forecast Visualization
- Compared Train vs Actual vs Forecasted sales

### Model Evaluation
Performance metrics:

- **MAE (Mean Absolute Error):** 190724.01  
- **MAPE (Mean Absolute Percentage Error):** 22.81%

Interpretation:
- Forecast accuracy is acceptable
- Model captures general trend but can be improved with seasonal modeling


---

## Key Insights
- Sales show steady growth over time.
- Rolling mean indicates presence of seasonality.
- Exponential Smoothing captures trend but aggregated data increases error.
- Forecasting individual store-item combinations could improve accuracy.

---

## Future Improvements
- Apply seasonal Exponential Smoothing
- Forecast per store-item combination
- Use weekly aggregation
- Try advanced models like ARIMA or Prophet
- Deploy dashboard using Streamlit or Power BI

---

## Conclusion
This project demonstrates a complete **end-to-end sales forecasting pipeline** including preprocessing, time-series analysis, modeling, and evaluation.  
It highlights practical forecasting techniques that can be applied to real-world retail sales data.
