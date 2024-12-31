Linear Regression Project
This repository contains files related to a linear regression project under my ML internship at Prodigy InfoTech. The project is divided into two main files, each serving a specific purpose. Here's a brief overview of each file:

File 1: Data.ipynb
Description
This Jupyter Notebook file focuses on data preprocessing and analysis. It prepares the dataset for building a linear regression model.

Steps:
Imported the 'Houseprice' dataset.
Dropped irrelevant columns and checked for zero values in the dataset. Converted 0 values to NaN and determined whether the zero value makes sense for the column or not.
Imputed the zero values based on the distribution of the column.
Rounded the decimal points in the dataset.
Converted the "sqft_basement" and "yr_renovated" columns into binary columns and renamed them.
Conducted statistical analysis on the dataset columns.
Addressed outliers in the columns based on the "Winsorization" technique and addressed skewness using the "Box-Cox" technique.
Saved the modified data into a file named "After_Modifications.csv".
File 2: LRModel.ipynb
Description
This Jupyter Notebook file is focused on building and evaluating a linear regression model. It uses the modified dataset prepared in 'Data.ipynb'.

Steps:
Import the modified data from 'After_Modifications.csv'.
Split the data into training and testing sets for model evaluation.
Build a linear regression model and evaluate its performance.
Use Recursive Feature Elimination (RFE) to select the top 5 features and build a new linear regression model with these features.
Attempt Lasso regression and cross-validation techniques to increase the model's accuracy.
