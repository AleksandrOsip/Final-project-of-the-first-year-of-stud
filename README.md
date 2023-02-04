Property Price Prediction
Table of contents
1. Project description

2. What case do we solve?

3. Data overview

4. Project stages

5. Results

Project description
We are given with a dataset representing properties listed in the US. The project objectives are:

Clean the dataset
Oplimise the features for the neads of the project
Create a number of machine-learning models to predict price using the given features
What case do we solve?
A representative of a large real-estate agency has approached us with the following problem:

“My realtors spend a disastrous amount of time sorting listings and looking for great deals. Therefore, their reaction speed, and, frankly speaking, the quality of the analysis does not reach the level of our competitors. This affects our financial performance.

Your task is to develop a model that would allow us to beat competitors in terms of the speed and quality of transactions."

The objective of the project is to develop a service for predicting the cost of properties based on the history of offers.

Data overview
The full dataset is here.

There are 377,185 lines representing different properties and 18 columns describing their features.

Each property has the following features:

status
private pool
propertyType
street
baths
homeFacts
fireplace
city
schools
sqft
zipcode
beds
state
stories
mls-id
PrivatePool
MlsId
target - price of the property, the predicting value
Project stages
The project consists of the following parts:

Project Overview
Explonatory Data Analysis - Part 1
Data Overview
Data Preprocessing
target
status
private pool & PrivatePool
propertyType
street
baths
homeFacts
remodeled year
heating,
cooling,
parking
lotsize
fireplace
city
schools
schools rating
schools distance
sqft
beds
stories
year built
price/sq.ft. & lot_size & sqft
Explonatory Data Analysis - Part 2
Categorical features
Feature Engeneering
Removing outliers
Correlation heat map
Encoding categorical features
Reducing the number of features
Normalisation
Modeling
Evaluation metrics
Baseline
Linear Regression
Light Gradient Boosted Machine Regressor
Gradient Boosting
Extreme Gradient Boosting
Random Forest
Stacking Regressor
Results
Conclusion
Results
The code is displayed in the following file

The best results are shown by the Random Forest Regressor model. The Mean Absolute Error became $59,434.88, which is quite a lot. The Mean Absolute Percent Error is 15.47%. The R^2 score (coefficient of determination) shows a relatively good 0.85 (on a scale from -1 to 1).

Overall, the original dataset has a lot of issues and inconsistencies. Cleaning and unwrapping of these issues were one of the main objectives of this project, which was accomplished successfully.

Another objective of this project was to demonstrate different machine-learning algorithms. The hyperparameters for all models were found using Optuna, a hyperparameter optimization framework. We left these calculations outside this Notebook as they are quite time-consuming.