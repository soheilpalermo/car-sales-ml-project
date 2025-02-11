# Car Price Prediction Model 🚗
### Project Overview
    This repository contains a machine learning project focused on predicting car prices using various regression models. The system analyzes car attributes like brand, model, manufacturing year, and mileage to accurately predict market prices.
    
### Key Features

- Advanced-Data Processing: Implements thorough preprocessing, including missing value handling and categorical variable transformation using One-Hot Encoding
- Multiple Model Comparison: Tests several regression algorithms, including Linear Regression, Random Forest, Gradient Boosting, and Lasso Regression
- Robust Evaluation: Uses R² score and Mean Absolute Error (MAE) for comprehensive model assessment
- Production-Ready: Includes model serialization for easy deployment

### Project Structure
├── Resources/
│   └── cars_info.csv           # Main dataset
├── outputs/
│   ├── model_evaluation_results.csv    # Model performance metrics
│   └── best_model.pkl          # Serialized production model
├── src/
│   ├── preprocessing.py        # Data cleaning and transformation
│   ├── model_training.py       # Model implementation
│   └── evaluation.py           # Performance assessment
└── README.md

### Dependencies
pandas
NumPy
seaborn
matplotlib
sci-kit-learn
joblib
### Model Performance
#### Our system evaluates multiple regression models:

Linear Regression: Simple, interpretable baseline model
Random Forest: Robust ensemble learning approach
Gradient Boosting: Sequential tree-based learning
Lasso Regression: L1 regularized linear model

Models are compared using:

R² Score: Explains variance in price predictions
Mean Absolute Error: Measures prediction accuracy
