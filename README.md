# Customer-Segmentation-For-Financial-Services
![Arvato-Bertelsmann-Logo svg](https://user-images.githubusercontent.com/39211262/81550770-547fd100-939e-11ea-99d2-cdaae8ad4f4e.png)
## Overview 
In this project, I analyzed the demographic data for customers of a mail-order sales company in Germany. The unsupervised learning technique was used to reduce dimensionality and identify the important demographic features that may contribute to online purchase. The supervised learning, or Gradient Boosting Classifier, was used next to fit the training data. Parameters were tuned according to accuracy score. The tuned model was then used to predict the test data. Final prediction was submitted to Kaggle competition.

## Installation 
   - Python 3.7
   - Numpy
   - Pandas
   - Matplotlib
   - Seaborn
   - Scikit-Learn
   - xgboost
## Problem statement
The problem here is that Arvato company needs to know the audiences that are more likely to become a customer to work towards achieving it’s goals in marketing. Thus, on this project, I am aiming to predict the audiences who are most likely to become a customer. I will approach this problem by first pre-processing the datasets. second, I will use unsupervised learning techniques to create clusters of customer and general population, and then identify the difference. Finally, I will predict whether or not a person will become a customer of Arvato or not.

## Summary:
This challenge was provided by Arvato Financial Solutions for the Udacity Data Science Nanodegree Program for Term 2. This is one of the possible capstone projects.

There were three major steps in the project:

- Customer Segmentation Report - This analyzed demographics data for customers of a mail-order sales company in Germany, comparing it against demographics information for the general population. This used unsupervised learning techniques to perform customer segmentation, identifying the parts of the population that best describe the core customer base of the company. 

- Supervised Learning Model -This used the previous analysis to build a machine learning model that predicts whether or not each individual will respond to the campaign.

- Kaggle Competition - This used the chosen model to make predictions on the campaign data as part of a Kaggle Competition and see how it measures up to the other fellow students.


## Results
The main findings of the code can be found at the post available [here](https://medium.com/@dastoulik12/customer-segmentation-report-for-arvato-financial-services-1f8777f8cb45).

## Improvements
To increase accuracy of the project we could follow following steps:
- Drop some variables by using correlation coefficient matrix to avoid the collinearity issue.
- Increase the threshold to drop rows and columns.
- Use other algorithms and try more parameters in the GridSearch.

There are many ways to improve this project few of them are , Eg. there are other ways to preprocess the data: choose another threshold for dropping rows and columns, choose different transformations for the columns, apply MinMax Scaler instead of Standard Scaler, impute data in another way.
Improvement of supervised model can be tested by using PCA dimensionality reduction. We could also choose attributes that have the most difference in clustering for overrepresented and underrepresented data and build supervised model using only these attributes.

## Acknowledgements
Thanks Udacity and Arvato for providing these apportunity to organize this project.
