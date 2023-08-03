# Prediction of Metabolic Syndrome

## Understanding the Relationship Between Health Measures and Metabolic Syndrome

Author: Kris Barbier

### Business Problem:

What is the relationship between certain health measures and the diagnosis of metabolic syndrome?
How can patients manage their lifestyle in order to reduce the risk of developing metabolic syndrome?

### Data:

Data source: https://data.world/informatics-edu/metabolic-syndrome-prediction

Data Dictionary:

![Data Dictionary](https://github.com/krisbarbier/Prediction-of-Metabolic-Syndrome/assets/134635095/412cc5dc-a38a-41e7-83fa-fceead148905)

## Methods:

- The following methods were used to clean, explore, process, and model the data:
  - Data Cleaning: The data was cleaned by looking for duplicates, dropping unnecessary columns, checking data type and value inconsistencies, identifying missing values, and researching outlying values.
  - EDA: Exploratory Data Analysis allowed me to view and compare each feature alone and in relationship to the target. This helped to identify correlations between different features and the target, while also allowing me to find features that were not likely strong predictors of the target so that only correlated features would be used in machine learning models.
  - Pre-Processing: The data was then pre-processed for machine learning. Missing values were identified and imputed, numeric data was scaled, and categorical data was encoded.
  - Machine Learning Models: The following models were implemented and tuned as necessary:
      - Random Forest
      - K-Nearest Neighbors
      - Logistic Regression
      - Gradient Boosting
      - LightGBM Boosting
      - XGBoosting
      - AdaBoosting
  - Feature Engineering: I used a selection of the more correlated features in my models, and also attempted PCA with the highest performing machine learning model.


## Results:

From the analysis of this project, we can see that the five most correlated health measures with the diagnosis of metabolic syndrome were waist circumference, BMI, blood glucose, HDL, and triglycerides, which is consistent with the research that exists for metabolic syndrome. 

**Visual 1: Waist Circumference and BMI Related to Metabolic Syndrome**

