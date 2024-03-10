# Phase 3 Project: SyriaTel Customer Churn Prediction

**Author**: Neville Ngenzi

## Introduction

### Overview
The telecommunication industry is rapidly evolving, with media transmission being a standout amongst the most developing sectors. Customer churn, defined as the rate at which subscribers switch to competitors, is a major concern in this industry. This project focuses on developing a hybrid predictive model for churn prediction and feature selection to enable service providers like SyriaTel to predict customer churn propensity.

## Project Structure

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Exploratory Data Analysis
5. Modelling
6. Model Evaluation
7. Recommendations and Conclusions

## 1. Business Understanding

### Business Problem
Customer churn poses a significant challenge for telecom companies like SyriaTel, impacting revenue, marketing expenses, and brand perception. Losing customers not only reduces immediate income but also escalates the expenses associated with acquiring new ones. This project aims to understand the reasons behind customer departures and mitigate further churn to foster long-term profitability and customer loyalty.

### Objectives
- Create a machine learning model to predict customer churn accurately.
- Identify key factors contributing to churn.
- Utilize the model to estimate churn probability.

## 2. Data Understanding

### Dataset
The dataset titled "Churn in Telecom" sourced from Kaggle provides details on customer activity, specifically whether they have terminated their subscription with the telecom company. This dataset aims to aid the telecom industry in minimizing financial losses attributed to short-term customer retention. Data understanding involves familiarizing with the dataset, identifying data quality issues, and conducting exploratory data analysis.

## 3. Data Cleaning

This step involves examining the dataframe for anomalies, including missing values, placeholder values, or distinct values.

## 4. Exploratory Data Analysis

### 4.1 Univariate EDA

Univariate data analysis focuses on analyzing individual variables. This involves studying each feature's distribution to comprehend its properties and detect anomalies like outliers.

### 4.2 Bivariate Analysis

Bivariate analysis examines the relationship between two variables. This will help understand how different features relate to customer churn.

### 4.3 Multivariate Analysis

Multivariate analysis investigates the interplay among multiple variables, focusing on their correlation with the target variable, customer churn. A correlation matrix will be utilized to discern associations among variables.

## 5. Modeling

In the churn prediction project, various models will be created, evaluated, and fine-tuned to predict customer churn based on dataset features.

### 5.1 Logistic Regression

Logistic regression is a statistical technique for binary classification tasks, estimating the probability of an observation belonging to a specific class.

### 5.2 Decision Tree Classifier

The Decision Tree Classifier partitions the dataset into refined subsets, predicting the class of new data based on feature values.

### 5.3 Random Forest Classifier

Random Forest creates multiple decision trees and derives predictions by averaging their outputs, suitable for classification tasks.

### 5.4 XGBoost

XGBoost merges weak models, like decision trees, using gradient boosting and ensemble learning, forming a potent predictive model.

The ROC_AUC metric will evaluate the performance of these models.

## 6. Model Evaluation

During this stage, models will be assessed using recall scores and ROC_AUC. The top two models will then be selected for further fine-tuning.

### 6.1 Model Comparison - Recall Score

The recall score quantifies the proportion of actual positive instances that the model correctly identifies.

### 6.2 Model Tuning

After assessing the models, it's evident that both XGBoost and RandomForest classifiers exhibit promising performance. Fine-tuning via GridSearch will be employed to enhance their effectiveness further.

#### 6.2.1 Tuning Random Forest

#### 6.2.2 Tuning XGBoost

## Conclusion

This analysis successfully achieved the objectives of building a machine learning model for customer churn prediction and estimating churn probability. 

Two models, Random Forest and XGBoost, were compared for effectiveness in predicting churn. 

Both models demonstrated strong performance, with Random Forest showcasing robust overall performance and XGBoost achieving a high recall score.

**Recommendation**: SyriaTel should prioritize the Random Forest Classifier as the primary model for predicting customer churn due to its superior overall performance and accurate identification of potential churners.

## Recommendation

The analysis identified key factors significantly impacting customer churn prediction:

- Call minutes and charges (daytime, evening, international)
- Customer service calls
- Usage of value-added services (voicemail plan)

SyriaTel should implement strategic customer retention efforts addressing these factors:

- Personalized offers and discounts
- Reduction of customer service calls
- Promotion of value-added services

## Future Work and Challenges

### Future Work:

- Continuous Model Monitoring: Ensure the model's effectiveness and relevance over time.
- Explore Advanced Techniques: Investigate ensemble methods or deep learning to further improve churn prediction.

### Challenges:

- Multicollinearity Issues: Address multicollinearity among predictor variables.
- Class Imbalance: Mitigate bias towards the majority class by preprocessing data effectively.
