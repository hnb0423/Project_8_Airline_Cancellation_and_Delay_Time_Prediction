# Project8: Airline Cancellation and Delay Time Prediction
## Business Problem
Online travel agency has been a popular way for customers to book flight tickets given that they often provide cheaper prices and offer choices from multitude of airlines that cater to the needs of their customers.

The scope of the project is to add on to the existing features of these online travel agency platform by providing them with information on flight delays and cancellation status. 

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
Encode categorical variables. <br/>
Utilize SMOTE resampling method to resolve the issue of imbalanced response variables for airline cancellation prediction. <br/>
Standardize data for regression predictive analysis. <br/>

## Models Construction and Evaluation:
Apply logistic regression random forest, logistic regression, and GRNN nerual network to training dataset.Plot confusion matrix and ROC curves. For stroke dataset, random forest has the highest accuracy, and for heart disease dataset, GRNN nerual network performs the best.
