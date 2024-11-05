# Heart Disease Risk Prediction
This project provides an in-depth exploratory data analysis (EDA) and predictive modeling approach for understanding heart disease risk factors using R. 
It follows a structured process, from data loading and cleaning to outlier detection and feature engineering. 
The aim is to identify key variables associated with heart disease risk, making this repository a comprehensive guide for anyone analyzing health-related data in R.

## Access the Project
[Explore the Heart Disease Risk Prediction on RPubs](https://rpubs.com/jasminemutia/1241036)

## Project Workflow
1. Load Data

Started by loading the dataset and necessary libraries, including ggplot2, dplyr, caret, and others.
The data is imported from heartData.csv, and an initial check is performed to ensure there are no missing values.
The dataset consists of 918 observations and 12 variables.

2. Exploratory Data Analysis (EDA)

EDA is conducted to understand the structure and distribution of the data. Key steps include:
- Checking data dimensions and types: Understanding variable types and distributions.
- Outlier Detection: Custom functions like ThreeSigma, Hampel, and BoxplotRule are used to detect outliers in key numeric variables (Age, RestingBP, Cholesterol, MaxHR, and Oldpeak). Outliers are addressed by filtering based on specified ranges.
- Univariate Analysis: Histograms of numeric and categorical variables to visualize distributions.
- Bivariate and Multivariate Analysis: Analyzing relationships between variables, especially the impact of various features on HeartDisease.

3. Data Preparation

For model training, specific columns relevant to heart disease prediction are selected, excluding certain less relevant features such as RestingBP, FastingBS, and ST_Slope.

4. Modeling

The cleaned data is used to train a decision tree classifier:
- Training a Decision Tree Model: rpart is used to train a decision tree on the preprocessed data.
- Evaluation: The model’s performance is evaluated using the caret package to assess prediction accuracy.

## Results
Model accuracy and key findings from EDA, including patterns and relationships in the data, are analyzed to draw insights regarding heart disease risk factors.

## Conclusion
This project demonstrates a workflow for predicting heart disease risk, from data cleaning to model evaluation. 
This workflow can be extended with additional machine learning techniques or integrated with new datasets for broader applications in health risk prediction.
