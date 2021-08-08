# Understanding-Simple-Linear-Regression

## Introduction

### Goal 
This analysis will demonstrate how to quantify the relationship between two variables using a Linear Regression model.

_Simple linear regression is a technique that can be used to understand the relationship between a single independent variable and a single dependent variable. Linear regression quantifies the relationship between independent and dependent variables._

### Motivation
This analysis is my practice to master Simple Linear Regression as a technique to be used in Data Science field. 

### Data
Ice Cream Revenue dataset will be used for the analysis. It is public and available in Kaggle at [this link](https://www.kaggle.com/vinicius150987/ice-cream-revenue).

### Libraries
You need an installation of Python, plus the following libraries:
- pandas
- numpy
- matplotlib
- scipy
- statsmodels

### Summary
This analysis has been performed purely for the display purposes of the Simple Linear Regression model, as it's useful to have some notes on the steps. However, during the analysis I faced with outliers and decided to run the analysis in a couple of different scenarios depending on various manipulations on the outliers as they can have significant impact on the analysis. So, the first run of the model has been implemented as it is without any changes in the outliers as we cannot reach out SME on the dataset and clarify if those observations abnormally far away from other values are actually outliers or not. The first model has R-squared close to 100%, meaning that the dependent variable can be explained by the independent one for 98%, which indicates a highly reliable model. Furthermore, all the required assumptions are met.

The second model was run after replacing all outliers to median value of the dataset, but it produced a statistically insignificant outputs with two failed assumptions out of three, meaning that the results of the second model cannot be reliable.

The third model was run after removing the observations/rows with outliers and its results are close to the first model with statistically significant outputs and all required assumptions are met.

So, having demonstrated the above analysis in three different scenarios, I can conclude that outliers can significantly impact the model.
