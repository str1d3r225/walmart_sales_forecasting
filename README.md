📦 Dataset
Source: Walmart Recruiting - Store Sales Forecasting

Contains:

train.csv – Weekly sales data by store and department

features.csv – Additional info like temperature, fuel prices, CPI, and holidays

stores.csv – Store type and size

🧠 Project Workflow
1. Data Preparation
Merged train.csv, features.csv, and stores.csv

Converted Date to datetime format

Forward-filled missing values for economic indicators

2. Feature Engineering
Extracted year, month, week, and day from Date

Created lag features (Sales_Lag_1, Sales_Lag_2, Sales_Lag_3) to capture past trends

3. Time-Aware Train-Test Split
Trained on data before July 2012

Tested on data from July 2012 onward to avoid leakage

4. Model Training
✅ Linear Regression as a baseline

🚀 XGBoost Regressor for improved performance

Evaluated using RMSE, MAE, and R²

5. Visualizations
Plotted actual vs predicted weekly sales for top-performing Store-Dept pairs

Used rolling averages and seasonal decomposition to uncover trends and seasonality

📈 Sample Output Plots
📊 Actual vs. Predicted Sales for Top 5 Store-Dept Combinations

🔁 4-Week Rolling Average Visualization

📉 Seasonal Decomposition (Trend, Seasonality, Residuals)

🧰 Tech Stack
Python, Pandas, NumPy

Scikit-learn, XGBoost, Matplotlib, Statsmodels

✅ Key Insights
Sales show strong seasonality during November–December

XGBoost outperforms baseline model with significant reduction in RMSE

Lag features significantly improve predictive power

📌 Project Highlights
Time-aware modeling for real-world forecasting

Feature engineering using lag values and calendar features

Advanced evaluation through rolling means and seasonal patterns

🙌 Credits
Data: Walmart via Kaggle
Developed by: Saad Ur Rahman

