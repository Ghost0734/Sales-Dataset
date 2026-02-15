# Sales Dataset Case Project

## Overview

This project analyzes the relationship between advertising spending across TV, Radio, and Newspaper channels and their impact on sales. Using linear regression, we build a predictive model to understand which advertising channels are most effective at driving sales.

## Dataset

The dataset contains advertising expenditure data and corresponding sales figures:

- **TV** - Television advertising spending (in thousands of dollars)
- **Radio** - Radio advertising spending (in thousands of dollars)
- **Newspaper** - Newspaper advertising spending (in thousands of dollars)
- **Sales** - Total sales revenue (in thousands of dollars)

## What This Project Does

1. **Correlation Analysis** - Measures how strongly each advertising channel correlates with sales
2. **Predictive Modeling** - Builds a linear regression model to predict sales based on ad spending
3. **Model Evaluation** - Compares model performance using different combinations of advertising channels
4. **Sales Prediction** - Makes sales predictions for new advertising expenditure scenarios

## Key Results

### Correlation with Sales

- TV: 0.9012 (strongest correlation)
- Radio: 0.3497 (moderate correlation)
- Newspaper: 0.1580 (weak correlation)

TV advertising shows the strongest relationship with sales, followed by Radio and then Newspaper.

### Model Performance

**Full Model (All 3 channels):**
- R² Score: 0.90
- MSE: 2.71
- The model explains 90% of the variance in sales

**Limited Model (Radio & Newspaper only):**
- R² Score: 0.12
- MSE: 24.35
- Without TV, the model performs poorly

The significant drop in performance when TV is excluded demonstrates its critical importance as a predictor of sales.

### Prediction Example

For advertising spending of TV: $200K, Radio: $40K, Newspaper: $50K, the model predicts sales of $19.81K.

## Technologies Used

- Python 3
- Pandas - Data manipulation
- NumPy - Numerical computations
- scikit-learn - Machine learning (LinearRegression, SimpleImputer, StandardScaler)
- Matplotlib - Data visualization

## Project Structure

- `Sales_Dataset_Case_Project.ipynb` - Main Jupyter notebook with all analysis and code
- `advertising_sales_data.xlsx` - Dataset file
- `README.md` - Project documentation

## How to Run

1. Open the Jupyter notebook in Google Colab or locally
2. Upload the `advertising_sales_data.xlsx` file when prompted
3. Run each cell sequentially to:
   - Load and explore the data
   - Calculate correlations
   - Train the regression model
   - View model performance metrics
   - Generate sales predictions

## Conclusions

TV advertising is the most effective channel for driving sales with a correlation of 0.90. The full model using all three channels provides reliable predictions with an R² of 0.90. Radio and Newspaper advertising have minimal impact on sales when used alone, highlighting the importance of TV in an advertising strategy.