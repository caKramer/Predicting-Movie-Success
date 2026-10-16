# Predicting-Movie-Success

Investigating the relationship between a movie's production budget, and its reception by audiences and critics, to determine if a large production budget is enough to predict success of a movie, or if there are more variables that dictate if a movie will be a hit or a miss. 

If you haven't pulled data before start with my [Python Data Gathering](https://github.com/caKramer/Python-data-gathering/tree/main) repository for learning how to ingest a CSV, a website, and API. 

Launch the PredictingMovieSucces_code.ipynb in Jupyter lab/notebook. Run the notebook to walk through the EDA plus visualizations and models.


## Data Sources

The Movie Database (TMDB) 5000 Movie Dataset from Kaggle

Open Movie Database (OMDb) API RESTful web service

Includes Exploratory Data Analysis, combining multiple datasets, analysis, visualizations, and feature engineering

## Models

Predicting how budget, votes, and critic metrics help to predict revenue

### Multiple linear regression
  NOTE: Log values were inverse-transformed and smearing correction applied.
  Duan's Smearing Factor (phi): 1.9661
  Linear Regression -> R²: 0.3802 | MAE: $525.26M | RMSE: $5896.79M


### Optimized Decision Tree Regressor
Decision Tree Regressor -> R²: 0.6610 | MAE: $64.58M | RMSE: $122.28M

### Random Forest Regression
Random Forest Regressor -> R²: 0.7252 | MAE: $57.90M | RMSE: $110.10M


### Random Forest Regression with Tuning and Optimizations
Optimal Parameters: {'max_depth': 10, 'max_features': 0.4, 'min_samples_leaf': 1, 'min_samples_split': 2, 'n_estimators': 500}
Duan Smearing Factor: 1.2965
Optimized Random Forest Regressor -> R²: 0.7393 | MAE: $58.54M | RMSE: $107.25M
