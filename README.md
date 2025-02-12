# Car Price Prediction 

## Project Objective
The goal of this project is to develop a machine learning model that predicts car prices based on various attributes, assisting buyers and sellers in determining fair market values.

## Data Collection
The dataset includes the following attributes:
- Brand
- Model
- Year of Manufacture
- Kilometers Driven
- Fuel Type
- Engine Capacity (CC)
- Price

## Data Preprocessing
- **Handling Missing Values**: Ensured dataset completeness.
- **Feature Engineering**: Created new features for improved predictions:
  - *Car_Age*: 2024 minus year of manufacture.
  - *Kilometers_per_Year*: Total kilometers driven divided by Car_Age.
- **Encoding Categorical Variables**: Converted categorical features into numerical representations.
- **Train-Test Split**: Used an 80-20 ratio for model evaluation.

## Exploratory Data Analysis (EDA)
Key predictors identified:
- *Car_Age*: Older cars have lower prices.
- *Engine Capacity (CC)*: Larger engines correlate with higher prices.
- *Year of Manufacture*: Newer models command higher prices.
- *Fuel Type*: Influences car value.
- *Kilometers Driven*: Higher mileage generally reduces value.

## Model Development
- **Algorithm Selection**: Chose *Random Forest Regressor* for its robustness.
- **Hyperparameter Tuning**: Optimized parameters using *RandomizedSearchCV*:
  - `n_estimators`: 200
  - `max_depth`: 20
  - `min_samples_split`: 2
  - `min_samples_leaf`: 1

## Model Evaluation
Performance Metrics:
- **Before Tuning**:
  - RMSE: 5093.63
  - R² Score: 0.9138
- **After Tuning**:
  - RMSE: 5068.54
  - R² Score: 0.9146
- **Residual Analysis**: Residuals centered around zero indicate a well-fitted model.

## Model Deployment
- **Model Saved As**: `random_forest_model.pkl`
- **Deployment Considerations**:
  - Web application using *Streamlit* or *Dash*
  - API implementation via *Flask* or *FastAPI*
  - Batch processing for new predictions

## Conclusion and Next Steps
**Key Takeaways**:
- Strong predictive performance (R² = 0.9146).
- *Car_Age* is the most significant predictor.
- Potential for further improvement by addressing outliers and adding features.

**Future Directions**:
- Deploy as a user-friendly web application.
- Validate with real-world data.
- Explore advanced modeling techniques for improved accuracy.


