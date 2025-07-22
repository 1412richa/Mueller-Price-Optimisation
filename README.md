# Mueller-Price-Optimization
Price Optimization on a simple test data using OLS and Random Forest

# Sales Price and Product Analytics
## Overview
This project analyzes how product prices and characteristics influence sales volume using a dataset of daily sales and product details. It includes exploratory data analysis, statistical modeling, and revenue optimization simulations. Both traditional econometric and machine learning methods are applied to predict sales and support pricing strategy decisions.

## Contents
### Data Exploration:
Summary statistics and visualizations to understand distributions, correlations, and the impact of product features on sales.

### Elasticity Modeling (OLS Regression):
Log-linear regression estimating the price elasticity of demand and the influence of brand, flavour, and packsize on units sold.

### Revenue Optimization Simulation:
Using the regression model to simulate pricing changes (e.g., a 10% price increase) and predict resulting sales and revenue impacts.

### Machine Learning Model:
Random Forest regression to predict log-units sold based on price and product attributes, compared with the linear model for predictive accuracy.

## Getting Started
### Prerequisites
 - Python 3.x
 - Required libraries:
   - pandas
   - numpy
   - matplotlib
   - seaborn
   - statsmodels
   - scikit-learn

Install dependencies using:
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn

## Data
 - sales.csv: Daily sales data with columns like date, product_id, price, units.
 - products.csv: Product details including brand, flavour, volume, packsize.

Make sure the CSV files are placed in the working directory or update the file paths in the code.

## Usage
1. Load and explore data:
Run descriptive statistics and visualize relationships between price, product features, and sales.

2. Fit elasticity model:
Use OLS regression with log-transformed units and price, including product features as categorical variables.

3. Evaluate model:
Check R-squared, coefficients, and RMSE to understand model fit and predictive power.

4. Simulate pricing strategies:
Use the model to predict sales and revenue under different price change scenarios.

5. Apply a machine learning model:
Train and evaluate a Random Forest regressor on log-transformed units to compare performance.

## Results Summary
- Strong negative relationship between price and units sold (price elasticity ≈ -0.61).
- Significant effects of brand and flavour on sales volume.
- Revenue simulation indicates a 10% uniform price increase slightly reduces total revenue, reflecting price sensitivity.
- Random Forest model achieved an RMSE of ~0.55 on log-units but did not outperform the linear model in this case.

## Future Work
- Tune machine learning models and explore other algorithms (e.g., Gradient Boosting).
- Incorporate additional features or external data (e.g., promotions, seasonality).
- Perform cross-validation and more robust model evaluation.
- Extend simulations to optimize pricing strategies for specific products or segments.

