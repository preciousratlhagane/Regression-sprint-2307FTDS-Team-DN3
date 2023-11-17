# Spain Electricity Shortfall Challenge

Aim: To provide a tool that will enable assist the Spanish government to predict the load shortfall in the upcoming months in order to consider the expansion of the country's natural resource energy infrastructure.

## Repository Overview

This repository consist of code created alongside resources for the creation of an appropriate machine building model to predict the electricity shortfalls in Spain in order to drive forth the decison of whether expansion of infrastructure is necessary. It also contains the data needed in order to solve the problem at hand.

## Data Overview

The data used for the training and testing of the predictive modelling is contained in two CSV files each containing past data on the load shortfall across five cities namely Madrid, Valencia, Bilbao, Seville and lastly Barcelona on a three hourly basis from 2015-2017 with the following weather conditions:

*wind speed
*wind degree
*rain 1h
*rain 3h
*humidity
*clouds all
*pressure
*snow 3h
*weather id
*temp max
*temp min
*temp

_Note: Some cities will not have features of certain weather conditions._

A starter notebook is attached where the feature enginerring is performed to handle outliners, missing values, and inconsistent data types.

## Dependencies

The starter notebook attached runs on the following dependencies:

*Python (version 3.x)
*NumPy
*Pandas
*Scikit-learn
*Matplotlib
*Seaborn

## Model Building

The models chosen to model the load shortfall was the Multiple Linear Regression, Decision Tree, Ensemble Models, AdaBoost, Gradient Boosting and lastly the Random Forest. The hyperparameters and parameters were tuned accordingly based on the cross-validation results.
The appropriate model was selected using the lowest Root Mean Square Error(RMSE) value out of the five models.

## Model Deployment

The model was deployed using the Flask API.
