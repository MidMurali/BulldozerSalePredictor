# Predicting the Sale Price of Bulldozers using Machine Learning

In this notebook, we're going to go through a machine learning project with the goal of predicting the sale price of bulldozers. The tools used are **pandas, numpy, matplotlib and scikit-learn**. 
Note: This project is completely done on a Colab notebook, hence no environment setup is explained/added in the repo.

Link: https://colab.research.google.com/drive/1yEBBdetJ02N8YSI5MeM7Dd0eLY2GA-IJ#scrollTo=E28KXRQZSSeQ

## Approaches
1. Problem Definition
2. Data
3. Evaluation
4. Features
5. Modelling
6. Experimentation

## 1. Problem Definition
How well can we predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?

## 2. Data
The data is downloaded from the Kaggle Bluebook for Bulldozers competition: https://www.kaggle.com/c/bluebook-for-bulldozers/data

Also given in the repo bluebook_bulldozer.rar

There are 3 main datasets:
* Train.csv is the training set, which contains data through the end of 2011.
* Valid.csv is the validation set, which contains data from January 1, 2012 - April 30, 2012. The predictions are made on this set throughout the majority of the competition. The score on this set is used to create the public leaderboard.
* Test.csv is the test set. It contains data from May 1, 2012 - November 2012. The score on the test set determines your final rank for the competition.

## 3. Evaluation
The evaluation metric for this competition is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

For more on the evaluation of this project check: https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation

**Note:** The goal for most regression evaluation metrics is to minimize the error. For example, the goal for this project will be to build a machine learning model which minimises RMSLE.


## 4. Features

Kaggle provides a data dictionary detailing all of the features of the dataset. The data dictionary can be found in the repository (Data Dictionary.xlsx)

## 5. Data Analysis and Modelling:

### 1. Saledate vs Saleprice for first 1000 entries.

![feature-importance](https://user-images.githubusercontent.com/25824881/81528961-6ac86580-937b-11ea-9a7e-47937fb99d80.png)

### 2. Feature Importance (year vs price)

![saledata-saleprice-1000](https://user-images.githubusercontent.com/25824881/81528995-86337080-937b-11ea-992d-448b76bc2b82.png)

## 6. Result

The csv with the predicted prices is uploaded in the repo as test_predictions_result.csv
