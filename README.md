# Churn Analysis

## Project Overview

This project focuses on predicting customer churn using various machine learning models and comparing their performance. The analysis is performed within a single Jupyter notebook, documenting the end-to-end workflow starting from data exploration to model evaluation. The primary goal is to build a reliable model for predicting customer churn and identify key factors that contribute to customer retention.

## Dataset

The dataset used for this analysis can be found [here](https://www.kaggle.com/datasets/muhammadshahidazeem/customer-churn-dataset). It includes various features about customer demographics, services subscribed, and account information.

## Exploratory Data Analysis (EDA)

The notebook begins with an exploratory data analysis to understand the distribution of features and the relationship between them. Various visualization libraries such as seaborn, matplotlib, and plotly are used to gain insights from the data.

## Model implementation and Cross-Validation

Several machine learning models are implemented and evaluated, like XGBoost, LightGBM, CatBoost and Logistic Regression.

Then, based on the **recall** metric, a parameter hypertuning with Bayesian Optimization is done in the XGBoost model, which had the best score.

### Results

The XGBoost model had a mean Recall of 0.95, meaning that only 5% of the actual positive cases were missed by the model. This resulted in less than 3% of the total predictions being false negatives.