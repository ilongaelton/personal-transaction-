# Personal-Transactions-Machine-Learning
Project 4


#  Personal Finance Forecasting Dashboard

Using a transactions data file from Kaggle (https://www.kaggle.com/datasets/entrepreneurlife/personal-finance) This project leverages machine learning and interactive visualization tools to help individuals forecast monthly expenses based on historical financial transactions. It includes an interactive dashboard built with Plotly and HTML/CSS, and a predictive model using Linear Regression.

---

##  Problem Statement

Many individuals lack clear visibility into their personal spending habits and upcoming expenses. This makes it difficult to budget effectively or plan for the future. This project solves that by:
- Grouping past transactions into meaningful categories
- Forecasting upcoming expenses using historical patterns
- Visualizing income vs. expenses over time

---

##  Solution Overview

The solution is a Python-powered forecasting tool that:
- Uses historical transactions from an Excel file
- Applies data preprocessing and feature engineering
- Trains a Linear Regression model to predict monthly spending per category
- Visualizes results using Plotly in an interactive dashboard

---

##  Features

- Excel-based input for ease of use
-  Machine Learning (Linear Regression) with lag features
-  Forecasting by month and category
- Interactive charts built with Plotly:
  - Monthly income trends
  - Predicted expenses by category
  - Actual vs. predicted spending comparison
-  Web dashboard using HTML/CSS + JavaScript

---

## Tools & Technologies Used

| Category        | Tools & Libraries                      |
|----------------|----------------------------------------|
| Programming     | Python, HTML, CSS, JavaScript          |
| Data Handling   | pandas, numpy                          |
| ML Modeling     | scikit-learn                           |
| Visualization   | Plotly, Matplotlib                     |
| Deployment      | HTML file (can be hosted on GitHub Pages, Streamlit, etc.) |
| Data Source     | Excel (.xlsx) transaction logs         |

---

## Project Structure

```
 personal-finance-forecast
├── transactions.xlsx           # Input transaction data
├── finance_forecast_model.py   # Python script (preprocessing, model, plots)
├── financial_dashboard.html    # Interactive dashboard
├── financial_model.pkl         # (Optional) Saved model
├── README.md                   # Project documentation
```

---

## Results

- **MSE:** 0.2660  
- **R² Score:** 0.8323  
- **RMSE (USD):** $72.10  
- Forecast accuracy significantly improved after including:
  - Lag features (previous month’s spend)
  - Temporal features (month, year)

---

## Future Improvements

- Use other features (e.g., account balance, weather, holiday flags)
- Deploy as a hosted web app
- Incorporate real-time bank feeds
- Add classification model for overspending alerts
- Include savings and investment tracking

---

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/personal-finance-forecast.git
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib scikit-learn plotly
   ```

3. Run the script:
   ```bash
   python finance_forecast_model.py
   ```

4. Open `financial_dashboard.html` in your browser to explore the dashboard.

