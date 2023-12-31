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

![Waist_BMI](https://github.com/krisbarbier/Prediction-of-Metabolic-Syndrome/assets/134635095/0b8ca348-da34-421a-99be-161708301690)

- Here we can see that on average, those with higher waist circumferences and BMI measurements are more likely to develop metabolic syndrome.

**Visual 2: Other Health Measures Related to Metabolic Syndrome**

![Health_Measures](https://github.com/krisbarbier/Prediction-of-Metabolic-Syndrome/assets/134635095/52b92642-31ef-408b-9b89-9807757028e6)

- In these charts, we can see that on average, those with higher blood glucose and triglyceride levels are more likely to develop metabolic syndrome, while having higher HDL levels has the opposite effect.

## Models:

- The results of the best machine learning model are as follows:

![Random Forest Metrics](https://github.com/krisbarbier/Prediction-of-Metabolic-Syndrome/assets/134635095/630d96c4-a0cf-4bc3-96d4-c5a55ba06a09)

- From these metrics, we see that this tuned random forest model performed with an overall accuracy of 88%. The number of false negatives (located in the bottom left corner of each matrix) was 32, or about 16% of the predictions. This was the lowest value for false negatives across all models that were tried and tuned.

## Recommendations:

Based on this data analysis, I would recommend the following:

  - Patients at risk of developing metabolic syndrome should strive to maintain a healthy lifestyle in order to maintain lower measurements of waist circumference, BMI, blood glucose, and triglycerides.
  - Patients wishing to reduce their risk of developing metabolic syndrome further should try to increase their HDL, or "good cholesterol" levels.

## Limitations and Next Steps:

One of the limitations of this data set is that it was missing data pertaining to another important idenifier for metabolic syndrome, which is blood pressure. While it included other health measures related to albumin levels in urine (which can relate to a complication from diabetes), blood pressure would have been a better predictor of metabolic syndrome.

In the future, I would focus on getting an even more accurate prediction model than the one presented here. While this model does well, I would really like to see even less Type II errors, as these patients get mis-diagnosed as not having metabolic syndrome when they really do. In order to improve the model's performance, I could look at several factors including further research to remove outlying values, lowering the decision threshold for the model, and trying different strategies to improve class balance.

## For Further Information:

For any additional questions, please contact:

- Kris Barbier: krisbarbier02@gmail.com

To see Tableau generated visuals of the data, visit:
- https://public.tableau.com/views/MetabolicSyndrome/LandingPage?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link 
