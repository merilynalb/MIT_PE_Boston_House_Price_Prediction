# MIT PE Elective Project: Boston House Price Prediction
As part of the MIT Professional Education's Applied AI and Data Science Program, this coursework explored the Boston House Price dataset and used basic machine learning regression tools to predict prices based on key features identified. 

## Overview of project
The objective of the project was to predict housing prices based on the features of the locality provided to us from the dataset. To understand the dataset, EDA was used to explore the features and identify correlations between the dependent and independent variables. The dataset was subsequently tidied for skewness, missing values, outliers, and prepared for linear regression modeling. An ordinary least squares (OLS) model was used to predict house prices on the training dataset, with iterations performed to improve prediction scores (R2, MAE, MSE, RMSE) and satisfy linear regression assumptions. The models were used on unseen test dataset and final model performance was evaluated. 

Key highlights:
- Using EDA to gain insights from the features
- Data preprocessing and preparation for regression modeling
- Building and iteratively improving the linear regression model
- Evaluating model performance using key metrics (R2, MSE, multicollinearity)
- Evaluating if the model over/under-fits the training data using cross-validation
- Checking the model satisfies linear regression assumptions
- Testing the model on unseen data

## Dataset
Each record in the database describes a suburb or town in a Boston. The data was drawn from the Boston Standard Metropolitan Statistical Area (SMSA) in 1970. Detailed attribute information can be found below:

Attribute Information:
CRIM: Per capita crime rate by town
ZN: Proportion of residential land zoned for lots over 25,000 sq.ft.
INDUS: Proportion of non-retail business acres per town
CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
NOX: Nitric Oxide concentration (parts per 10 million)
RM: The average number of rooms per dwelling
AGE: Proportion of owner-occupied units built before 1940
DIS: Weighted distances to five Boston employment centers
RAD: Index of accessibility to radial highways
TAX: Full-value property-tax rate per 10,000 dollars
PTRATIO: Pupil-teacher ratio by town
LSTAT: % lower status of the population
MEDV: Median value of owner-occupied homes in 1000 dollars

## Overview of this project
This project contains three files:
1. Boston.csv: The Boston House Price dataset
2. Learners_Notebook_Boston_house_price_Full_Code_MMA.ipynb: The Jupyter notebook
3. Learners_Notebook_Boston_house_price_Full_Code_MMA.html: HTML file to visualise the code and figures easily

## Libraries Used
This project used the following libraries in Python:

For general use and data tidying:
- Numpy
- Pandas

For visualisation:
- Seaborn
- Matplotlib

For regression modeling:
- statsmodel
- scikit-learn

## Conclusion
The final OLS model had a high R2 value of 0.773 and low RMSE value of 0.19. It predicted house prices with high accuracy up to $40,000, after which some confounding factors may have influenced the expensive house prices that this basic model couldn't account for.

The key features identified to contribute towards house price prediction was:
- NOX: nitric oxide concentration
- CHAS: location relative to the river
- RM: average number of rooms per house

This project was graded 59/60 by MIT PE examiners.
