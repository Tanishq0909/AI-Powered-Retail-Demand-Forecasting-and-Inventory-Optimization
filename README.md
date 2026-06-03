# AI-Powered Retail Demand Forecasting & Inventory Optimization

## Overview
This project develops an end-to-end retail analytics solution to forecast product demand and optimize inventory management using Machine Learning and Power BI.

## Business Problem
Retail businesses often face:
- Overstocking and increased holding costs
- Understocking and lost sales
- Limited visibility into future demand

This project addresses these challenges through demand forecasting and inventory optimization.

## Dataset
- Online Retail transaction dataset
- ~392,000+ cleaned transaction records
- Features include product details, quantities, prices, customers, countries, and transaction timestamps

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Google Colab
- Power BI

## Project Workflow

### 1. Data Cleaning & Preparation
- Removed missing values and invalid transactions
- Created revenue metrics
- Processed date and time features

### 2. Feature Engineering
Created:
- Lag_1
- Lag_7
- Rolling_7
- Rolling_30
- Month
- Quarter
- DayOfWeek

### 3. Demand Forecasting
Models evaluated:
- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

Final Model:
- Linear Regression

Performance:
- MAE: 6581
- RMSE: 9463
- R² Score: 0.375

### 4. Inventory Optimization
Implemented:
- Reorder Point Calculation
- Safety Stock Logic
- Inventory Health Classification
- Automated Reorder Recommendations

Results:
- Products Analyzed: 20
- Products to Reorder: 8
- Products with Sufficient Stock: 12

### 5. Power BI Dashboard
Pages:
1. Executive Overview
2. Demand Forecasting
3. Inventory Optimization

## Key Insights
- Rolling_7 was the most influential forecasting feature.
- Recent sales history was more predictive than seasonal variables.
- Linear Regression outperformed Random Forest and XGBoost on the prepared dataset.
- Inventory optimization identified products requiring immediate replenishment.

## Repository Structure

```text
Retail-Demand-Forecasting/
├── data/
├── notebooks/
├── dashboard/
├── screenshots/
└── README.md
```

## Future Improvements
- Streamlit Deployment
- SQL Database Integration
- Real-Time Forecasting
- Cloud Deployment

## Author
**Tanishq Belhekar**  
GitHub: Tanishq0909
