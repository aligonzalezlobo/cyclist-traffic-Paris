# Predicting Cyclist Traffic in Paris

**Authors:** Nazila Sharifi Amina and Alicia González Lobo
**RAMP Project - December 2022**

## Project Overview

This project focuses on predicting cyclist traffic in Paris using machine learning techniques. We conducted a thorough analysis of the data, merged various datasets, and employed regression models to achieve this goal. Below, we outline the key aspects of our project.

## Problem Statement

The task involves finding an optimal estimator to predict cyclist traffic in Paris. We performed data analysis, preprocessing, and model selection to develop a reliable regression model. Our goal was to predict the number of cyclists in Paris at a given time.

## Data

### Original Data
The original dataset contains hourly information about cyclist traffic, including features like counter name, counter site name, date, counter installation date, latitude, and longitude. Some variables were dropped as they were redundant.

### Weather Data
We incorporated weather data to consider factors like rainfall, temperature, and wind, which may affect cyclist traffic.

### Vehicles Data
We included data on the traffic of heavy vehicles in Paris, as it could be correlated with cyclist traffic.

### Significant Periods
We considered important dates such as Covid-19 lockdowns and public holidays, as they significantly impact bike traffic.

After data manipulation, merging, and feature selection, our final dataset includes categorical, numerical, binary, and date variables.

## Model Selection

### Choosing the Regressor
We performed model selection to find the best estimator for our regression task. We started with simple regression models (e.g., Linear Regression, Ridge) and later explored more complex models (e.g., RandomForestRegressor, XGBoostRegressor). XGBoostRegressor performed the best, considering the RMSE scores.

### Tunnning the Hyper-parameters
We tuned hyperparameters to improve the XGBoostRegressor model's performance. Due to time constraints, we couldn't perform an exhaustive hyperparameter search but managed to find suitable parameters.

## RAMP Submissions

We submitted different versions of the XGBoostRegressor model to the RAMP platform to test its performance. The best-performing estimators were selected for submissions.

## Limitations of Our Work

- Limited time for hyperparameter tuning.
- Possible overfitting issues.
- The ramp-test results performed better than the RAMP platform, indicating room for improvement.

## Jupyter Notebook and Data

In this repository, you will find a Jupyter Notebook (`cyclist_traffic_Paris.ipynb`) that was used at the beginning of the project. This notebook was primarily used for the following purposes:

- Data Exploration: We used it to perform initial data exploration and understand the structure of the datasets.

- Data Preprocessing: We performed data preprocessing steps such as data merging, feature selection, and handling missing values.

- Simple Models: We experimented with simple regression models like Linear Regression and SGD Regressor to gain insights into the data before moving on to more powerful models.

- Data Visualization: We created visualizations to better understand the relationships between various features and the target variable.

The data used in the notebook can be found in the `data/` directory.

## Contact Us

If you would like to access the final estimator created for submission on the RAMP platform, inquire about how other models performed, or explore our full project report, please don't hesitate to contact us. We are happy to provide you with additional information and assistance.


## References

- [Comptage vélo - Compteurs](https://www.paris.fr/equipements/comptage-velo-compteurs-1804)
- [Comptage vélo - Données compteurs](https://www.paris.fr/equipements/comptage-velo-compteurs-1804)
- [Open-Meteo Historical Weather API](https://open-meteo.com/)
- [Comptage multimodal (Vélo, Trottinette, 2RM, VL, PL, Autobus-car) - Comptages](https://www.paris.fr/equipements/comptage-multimodal-velo-trottinette-2rm-vl-pl-autobus-car-comptages-19525)
- [XGBoost Tutorials - Introduction to Boosted Trees](https://xgboost.ai/)

Feel free to explore the code and data in this repository to gain more insights into our project.
