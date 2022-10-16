# House Price Prediction

<p align="justify">House is the primary need of everyone. Almost everyone when starting to start a family chooses to buy a house, this is indicate that the need to own a home will increase over time. Buying a house is commonly the most important financial transaction. The fact that most prices are negotiated individually (unlike a stock exchange system) creates an environment that results in an inefficient system. That's why many of real estate agency using house prediction concept to drive the efficiency of house pricing.</p>

<p align="justify">House price prediction can help real estate agency to determine the selling price of a house. It can also help the customer to make a better decision to purchase a house. There are some factors that influence the price of a house which depends on physical conditions, concept, location and others. House prices vary for each place and in different communities. There are various techniques for predicting house prices. One of the efficient ways is by the use of the regression technique. Regressions are an exciting area of data analysis since it enables us to make very specific predictions, incorporating different variables simultaneously.</p>

## About
This project using The Boston Housing Dataset. The Boston Housing Dataset is a derived from information collected by the U.S. Census Service concerning housing in the area of Boston MA. From this dataset, we want to predict the house price (medv) using some features. The following describes the dataset columns / features: 
1. CRIM - per capita crime rate by town
2. ZN - proportion of residential land zoned for lots over 25,000 sq.ft.
3. INDUS - proportion of non-retail business acres per town.
4. CHAS - Charles River dummy variable (1 if tract bounds river; 0 otherwise)
5. NOX - nitric oxides concentration (parts per 10 million)
6. RM - average number of rooms per dwelling
7. AGE - proportion of owner-occupied units built prior to 1940
8. DIS - weighted distances to five Boston employment centres
9. RAD - index of accessibility to radial highways
10. TAX - full-value property-tax rate per $10,000
11. PTRATIO - pupil-teacher ratio by town
12. BLACK - the proportion of blacks by town
13. LSTAT - % lower status of the population
14. MEDV - Median value of owner-occupied homes in $1000's

## Objective & Method
This project uses several methods of regression, we want compare it and get the best model to predict the house price. Here are some of the methods that used :
1. Multiple linear regression
2. Regularized linear regression with the best lambda (Lasso & Ridge Regression)
3. Random forest regression

## Conclusion
   Here is the comparison of the evaluation metrics among those methods :
   
| Metric | Multiple Linreg | Lasso Reg | Ridge Reg | Random Forest Reg |
| :---: | :---: | :---: | :---: | :---: | 
| R2 | 0.714963 | 0.484510 | 0.713695 | 0.971135 |
| RMSE | 5.463073| 5.315646 | 5.446738 | 4.061765 |
| MAE | 3.376244| 3.535684 | 3.375222 | 2.538490 |
| MAPE | 0.180371| 0.293518 | 0.252971 | 0.130002 |

From those metrics score, we can conclude that :
1. Random Forest Regression Model has the highest R2 Score, that is 0.971135. It means that 97,11% of the total variability of medv was successfully modeled using that features. 
2. Random Forest Regression Model has the smallest RMSE, MAE, & MAPE Value.
3. The three most important features that affect the house price (medv) based on random forest model are rm, ptratio, & zn.

## Requirements

```
pandas, numpy, sklearn, statsmodels, seaborn, matplotlib
