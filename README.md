# Insurance Charges Prediction using Machine Learning

## Overview

This repository contains a project that analyzes medical insurance charges based on various factors such as age, BMI, smoking status, and region using machine learning techniques. The goal is to build predictive models to estimate medical expenses and explore the most important features affecting the costs.

## Table of Contents
1. [Project Description](#project-description)
2. [Data](#data)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Model Building](#model-building)
5. [Feature Importance](#feature-importance)


## Project Description

The dataset used in this project is a medical insurance dataset that includes various factors influencing the medical charges billed to individuals. We explore and analyze these factors, visualize trends, and implement machine learning models like Linear Regression and Random Forest to predict insurance charges.

## Data

The dataset `insurance.csv` contains 1,338 rows and 7 columns:
- `age`: Age of the individual.
- `sex`: Gender (male/female).
- `bmi`: Body Mass Index (BMI).
- `children`: Number of children/dependents.
- `smoker`: Whether the person smokes (yes/no).
- `region`: The region where the person lives (northwest, northeast, southwest, southeast).
- `charges`: Medical charges billed to the individual.

### Sample of the Data:
| age | sex   | bmi  | children | smoker | region    | charges     |
|-----|-------|------|----------|--------|-----------|-------------|
| 19  | female| 27.9 | 0        | yes    | southwest | 16884.92400 |
| 18  | male  | 33.77| 1        | no     | southeast | 1725.55230  |

## Exploratory Data Analysis (EDA)

We start with basic exploratory data analysis to understand the distribution and relationship of features. Key visualizations include:

1. **Distribution of Insurance Charges**:
   - The medical charges are right-skewed, and we applied log transformations to bring the data closer to a normal distribution.

2. **Charges by Region, Smoking Status, and Other Factors**:
   - Bar plots, scatter plots, and violin plots are used to identify relationships between the charges and factors like smoking status, BMI, age, and children.

   ![Sample Plot](path_to_image_if_any.png) <!-- You can add images or remove this line -->

## Model Building

We built two models to predict the insurance charges:

i. **Linear Regression**:
   - After splitting the data into training and testing sets, we trained a linear regression model.
   - **R² score** on the test data: `0.783`.


2. **Random Forest Regressor**:
-Random Forest was also applied to capture more complex relationships between the features.
-Feature importance was derived from the model to understand the most impactful factors.

5. **Feature Importance**:

-The Random Forest model identified the following features as the most important:

-`Smoker`: Has the highest impact on insurance charges.
-`BMI`: Highly correlated with higher charges.
-`Age`: Shows a moderate effect on charges.
-`Children`: Less significant compared to other factors.
The importance of each feature is visualized using bar plots.


