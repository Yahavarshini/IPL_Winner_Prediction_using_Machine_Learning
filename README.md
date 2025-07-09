# IPL Match Winner Prediction

This project predicts the winner of an Indian Premier League (IPL) cricket match using machine learning techniques. It analyzes historical match data and applies classification models to forecast outcomes based on match-related features.


## Project Objective
- Predict the winning team of an IPL match using features such as participating teams, toss winner, toss decision, and venue.
- Compare multiple machine learning models and select the best-performing approach.


## Dataset Overview
- Includes detailed IPL match records with columns like season, city, date, team1, team2, toss winner, toss decision, venue, and result.
- Target variable: **winner**.
- Data cleaned to remove missing values, standardize team and venue names, and exclude irrelevant rows (e.g., 'no result' matches).


## Feature Engineering
- **Feature Selection:** Used Recursive Feature Elimination (RFE) to select top features: team1, team2, toss_winner, toss_decision, and venue.
- **Feature Transformation:** Applied one-hot encoding to input features and label encoding to the target variable.
- **Feature Scaling:** Not applied since features were categorical.


## Data Cleaning Steps
- Filled missing `city` values by cross-referencing `venue`.
- Removed rows with `result = 'no result'`.
- Corrected inconsistencies in team and venue names.
- Extracted year from `season`.
- Dropped columns with too many missing values like `date` and `umpire3`.
- Excluded Kochi Tuskers Kerala matches due to limited data.


## Models Implemented
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Bernoulli Naive Bayes
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost


## Modeling Approach
- Balanced classes with sampling techniques.
- Split data into training and testing sets (typically 80/20).
- Applied cross-validation to evaluate model stability.
- Performed hyperparameter tuning (grid/random search) for optimal performance.


## Results Summary
- **Best Models:** Gradient Boosting and XGBoost.
- Achieved high accuracy, minimal overfitting, and consistent results across train, test, and cross-validation splits.
- Ensemble methods outperformed simpler models, highlighting their strength for this problem.


## Future Scope
- Add more seasons and matches to increase data size.
- Incorporate richer features like player stats, weather, and pitch conditions.
- Apply advanced sampling techniques (e.g., SMOTE for multiclass).
- Experiment with deep learning or ensemble stacking.
- Deploy as a web app or API for real-world use.



## Author
- Yahavarshini E
- yahaelamurugu2428@gmail.com


