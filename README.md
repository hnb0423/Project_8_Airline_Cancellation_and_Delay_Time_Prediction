# Project8: Airline Cancellation and Delay Time Prediction
## Business Problem
Online travel agency has been a popular way for customers to book flight tickets given that they often provide cheaper prices and offer choices from multitude of airlines that cater to the needs of their customers.

The goal of this project is to analyze domestic flight delay and cancellation data over the past 10 years to predict a future flight delay time through regression models and cancellation status through classification models.

## Raw Data
Kaggle: https://www.google.com/url?q=https://www.kaggle.com/yuanyuwendymu/airline-delay-and-cancellation-data-2009-2018&sa=D&source=editors&ust=1647210752669909&usg=AOvVaw2x2wMrs_CqHGYWqO5wDf_I

Open Flights: https://openflights.org/data.html

## Data Processing:
Drop columns with over 70% missing values, and remove the rest of null values. <br>
Rename columns and inner join two datasets on airport code. 
Export three datasets: one for EDA, one for regression (delay time prediction), and one for classification (cancellation prediction). 

## EDA
Compute a series of plots, including bar charts, time series line charts, and map plot. Generate useful insights from data. 

## Feature engineering:
Construct "season" column based on flight date <br/>
Encode categorical variables. <br/>
Utilize SMOTE resampling method to resolve the issue of imbalanced response variables for airline cancellation prediction. <br/>
Standardize data for regression predictive analysis. <br/>

## Models Construction and Evaluation:
Split data into 80% train and 20% test. Apply 3-fold cross validation to the train dataset. Then, make predictions with the best models.

### Airline Delay Time Prediction
Apply random forest, multiple linear regression, and penalized multiple linear regression (lasso, ridge, and elastic net) to train models. Since multiple linear regression has the lowest RMSE, I use this model to make predictions.
### Airline Cancellation Prediction 
Apply random forest, logistic regression, penalized logistic regression (lasso, ridge, and elastic net) to train models. Since logistic regresison has the highest accuracy, I use this model to make predictions. 
