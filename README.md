Car Price Prediction Model
Overview
This project aims to predict car prices based on various features using machine learning models. The dataset used contains information about car brands, models, year of manufacture, and other features that contribute to the car's value. The project utilizes multiple regression models to predict car prices and evaluates their performance to select the best model.

Features of the Project
Data Preprocessing: The dataset is cleaned, and necessary columns are dropped. Categorical features are one-hot encoded, and numerical features are scaled.
Multiple Models: Several regression models are trained, including Linear Regression, Random Forest, Gradient Boosting, and Lasso Regression.
Model Evaluation: The models are evaluated using metrics like R² Score and Mean Absolute Error (MAE).
Model Comparison: The results of each model are compared visually using scatter plots and a bar plot for R² scores.
Best Model Selection: The best-performing model is saved for future use and deployment.
Files
cars_info.csv: The dataset containing car details.
model_evaluation_results.csv: The CSV file storing the evaluation results of each model (R² Score and MAE).
best_model.pkl: The saved best model after training, ready for deployment or further use.
Dependencies
pandas
numpy
seaborn
matplotlib
scikit-learn
joblib
You can install these dependencies by running:

bash
Copy
Edit
pip install pandas numpy seaborn matplotlib scikit-learn joblib
How to Run
Place the cars_info.csv dataset in the Resources folder.
Run the Python script to train and evaluate the models.
The evaluation results will be saved in model_evaluation_results.csv.
The best-performing model will be saved as best_model.pkl for future use.
Model Evaluation
After training, the following models were evaluated:

Linear Regression
Random Forest Regressor
Gradient Boosting Regressor
Lasso Regression
The models were evaluated using:

R² Score: Measures the proportion of the variance in the dependent variable that is predictable from the independent variables.
MAE (Mean Absolute Error): Measures the average magnitude of the errors in a set of predictions, without considering their direction.
