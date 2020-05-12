# Customer-Segmentation-For-Financial-Services
<p align="center">
  <img  src="https://user-images.githubusercontent.com/39211262/81551006-b93b2b80-939e-11ea-882d-8ef875117210.png">
</p>

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

## Metrics
For XGBRegressor, the training score keeps decreasing, and the testing score keeps increasing. While for the RandomForestRegressor, the training score remains constant at a high level and the cross-validation score is low. It is clear that the best model is XGBRegressor because the RandomForestRegressor overfits the data.
![download (8)](https://user-images.githubusercontent.com/39211262/81636042-690ca980-9430-11ea-8e54-d76c3921a2aa.png)
![download (9)](https://user-images.githubusercontent.com/39211262/81636045-6ad66d00-9430-11ea-9cbf-dacd3d0d6927.png)
## Results
![Capture](https://user-images.githubusercontent.com/39211262/81639877-cad21100-943a-11ea-8853-6cd954712092.PNG)
From quick comparison of above charts, we can see drastic difference in the distribution of the most important feature "D19_SOZIALES". In Cluster 5 the over represented cluster of customer, there is a single bar and in Cluster 10 under represented cluster of customer there is a distribution and not a consolidation in 1 particular value

The main findings of the code can be found at the post available [here](https://medium.com/@dastoulik12/customer-segmentation-report-for-arvato-financial-services-1f8777f8cb45).

## Improvements
To increase accuracy of the project we could follow following steps:
- Drop some variables by using correlation coefficient matrix to avoid the collinearity issue.
- Increase the threshold to drop rows and columns.
- Use other algorithms and try more parameters in the GridSearch.

There are many ways to improve this project few of them are , Eg. there are other ways to preprocess the data: choose another threshold for dropping rows and columns, choose different transformations for the columns, apply MinMax Scaler instead of Standard Scaler, impute data in another way.
Improvement of supervised model can be tested by using PCA dimensionality reduction. We could also choose attributes that have the most difference in clustering for overrepresented and underrepresented data and build supervised model using only these attributes.

## Acknowledgements
Thanks [Udacity](https://www.udacity.com/) and [Arvato](https://www.bertelsmann.com/divisions/arvato/#st-1) for providing these apportunity to organize this project.
