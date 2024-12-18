# Machine Learning Project - Predicting Airbnb Prices

This is the final project for the Machine Learning course at KeepCoding. The goal of this project is to predict the price of Airbnb listings based on various features such as number of bedrooms, location, and amenities.

## Project Overview

In this project, I have implemented several machine learning models to predict the prices of Airbnb listings. The models used include Linear Regression, Polynomial Regression, Random Forest, and K-Nearest Neighbors (KNN). I performed feature engineering, hyperparameter tuning using GridSearchCV, and model evaluation to obtain the best predictions.

## Models Used

The following models were applied to predict the price of the Airbnb listings:

- **Linear Regression**: A linear model to predict the target variable based on the features.
- **Polynomial Regression**: Extends linear regression by adding polynomial features to capture non-linear relationships.
- **Random Forest**: An ensemble method that uses multiple decision trees to predict the target variable.
- **K-Nearest Neighbors (KNN)**: A non-parametric model that predicts the target based on the nearest neighbors.

## Data

The data used for this project is from Airbnb listings, and it contains various features related to the properties and their availability.

### Key Features:
- `Price`: The target variable we are trying to predict.
- `Bedrooms`: Number of bedrooms in the property.
- `Accommodates`: Number of guests the property can accommodate.
- `Security Deposit`: Security deposit required for the booking.
- `Cleaning Fee`: The cleaning fee associated with the listing.
- `Extra People`: The extra charge per additional person.
- `Minimum Nights`: Minimum number of nights required to book the listing.

The models were evaluated using the following metrics:
- **RMSE (Root Mean Squared Error)**
- **R² Score**

GridSearchCV was used to tune hyperparameters, especially for models like KNN and Random Forest, to ensure optimal performance.

### Model Performance:
(FF: full features, SF:selected features)

| Model Used            | Train Accuracy | Test Accuracy |
|-----------------------|----------------|---------------|
| Random Forest (SF)    |     96.2 %      |     72 %     |
| Random Forest (FF)    |     93.8 %      |    70.1 %    |
| KNN (SF)              |      100 %      |    65.6 %    |
| KNN (FF)              |      100 %      |    62.4 %    |
| Linear Regression     |     65.5 %      |     61 %     |
| Polynomial Regression |     76.2 %      |    66.5 %    |
