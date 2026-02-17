# ML-House-Pricing-Model

# Contact Info

Want to hire me? Check out my LinkedIn here: https://www.linkedin.com/in/jesse-o-03476a102/

Want to comission me for a project? Check out my Upwork profile here: https://www.upwork.com/freelancers/~0193f57dd84700cb81

# Melbourne Housing Price Prediction (Laptop-Safe ML Model)

A lightweight machine learning project that predicts housing prices using structured property data from Melbourne.

This project demonstrates a clean end-to-end ML pipeline using classical methods — no deep learning, no overkill, just disciplined fundamentals.

# Project Objective

To build a regression model that:

Cleans real-world tabular data

Encodes categorical variables

Trains a supervised learning model

Evaluates predictive error

Generates real vs predicted price comparisons

The goal is clarity and performance — optimized to run safely on a standard laptop without excessive memory usage.

# Model Overview

Algorithm Used:
RandomForestRegressor from sklearn

Why Random Forest?

Strong baseline performance for tabular data

Handles nonlinear relationships well

Reduces overfitting via ensemble averaging

Computationally efficient for medium-sized datasets

# ML Workflow

# Data Loading
df_raw = pd.read_csv("MELBOURNE_HOUSE_PRICES_LESS.csv")

# Feature Cleaning

Dropped high-cardinality and non-predictive columns:

Address

SellerG

Date

Postcode

Latitude/Longitude

Regionname

Propertycount

Removed missing values

# Feature Engineering

One-hot encoding for categorical variables:

Suburb

Type

CouncilArea

etc.

# Train/Test Split
train_test_split(X, y, test_size=0.2, random_state=42)

# Model Training
model = RandomForestRegressor(
    n_estimators=100,
    max_depth=None,
    random_state=42,
    n_jobs=-1
)

# Evaluation Metric

Mean Absolute Error (MAE)

MAE answers one simple question:
On average, how wrong is our model in dollar terms?

# Output

The project generates:

Model performance metrics

Real vs Predicted price comparisons

A safe, memory-conscious CSV output:

melbourne_property_price_comparison_laptop_safe.csv

# Laptop-Safe Optimizations

This repo was intentionally built to avoid:

Memory overuse from high-cardinality encoding

Massive feature explosions

Excessive model complexity

GPU dependency

It runs comfortably on:

Standard MacBook / Windows laptop

8–16GB RAM

No cloud compute required

# Why This Project Matters

Structured mathematics

Applied probability

Feature engineering

Error measurement

Iterative improvement

This project shows that powerful predictive systems do not require enormous infrastructure — just solid fundamentals.

# Tech Stack

Python

Pandas

scikit-learn

NumPy

# Future Improvements

Potential next steps:

Hyperparameter tuning (GridSearchCV)

Feature importance analysis

Cross-validation

Deployment as a Flask API

SHAP analysis for interpretability

Expansion into financial asset price modeling

# Author

Built by Jesse Olivarez
Finance / Credit Risk / Data Analytics /  Machine Learning

If you're building at the intersection of quantitative finance and applied ML — let's connect
