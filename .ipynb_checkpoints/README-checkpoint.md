# Portfolio 2: Analysis of an E-commerce Dataset

This repository contains my solutions for the Portfolio 2 assignment for the course COMP6200 – Data Science. The assignment involves analyzing an e-commerce dataset, training linear regression models to predict user ratings, and evaluating the impacts of feature selection and training/testing data sizes on model performance.

## Contents

- `Portfolio 2_Analysing E-Commerce Data.ipynb`: The Jupyter notebook containing the questions, solutions, code, and analysis for Portfolio 2.

## Assignment Details

### Analysis of an E-commerce Dataset

The goal of this analysis task is to train linear regression models to predict users' ratings towards items. This involves a standard Data Science workflow: exploring data, building models, making predictions, and evaluating results. In this task, we explore the impacts of feature selections and different sizes of training/testing data on model performance using a cleaned combined e-commerce sub-dataset.

### Tasks and Solutions

#### Import Cleaned E-commerce Dataset
**Task:** Import the cleaned e-commerce dataset from a CSV file and print its total length.
- **Actions:**
  - Loaded the dataset using Pandas `read_csv` method.
  - Printed the total number of records in the dataset.

#### Explore the Dataset
**Task:** Get an overview of the dataset using `head()` and `info()`, and compute correlations between features and the target variable (rating).
- **Actions:**
  - Utilized `head()` and `info()` methods to understand the dataset structure and data types.
  - Converted categorical features (gender, category, review) to numerical values using `OrdinalEncoder`.
  - Calculated correlations between helpfulness, gender, category, review, and rating using the `corr()` method.
  - Provided explanations on the most and least correlated features and discussed their potential impact on prediction results.

#### Split Training and Testing Data
**Task:** Randomly split the data into training and testing sets with different sizes to investigate the impact on model performance.
- **Actions:**
  - Split the data into training and testing sets with 10% and 90% training data, respectively.
  - Printed the shapes of the training and testing sets for both cases.

#### Train Linear Regression Models with Feature Selection under Cases 1 & 2
**Task:** Train four linear regression models with different feature selections and training/testing data sizes.
- **Actions:**
  - Selected the two most correlated and two least correlated features with rating.
  - Trained four models:
    - **Model A:** Case 1 (10% training data) with two most correlated features (category, review).
    - **Model B:** Case 1 (10% training data) with two least correlated features (helpfulness, gender).
    - **Model C:** Case 2 (90% training data) with two most correlated features (category, review).
    - **Model D:** Case 2 (90% training data) with two least correlated features (helpfulness, gender).

#### Evaluate Models
**Task:** Evaluate the performance of the four models using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-Squared (R2).
- **Actions:**
  - Calculated and printed MSE, RMSE, and R2 for all four models.

#### Visualize, Compare, and Analyze the Results
**Task:** Visualize the results and perform insightful analysis on the obtained results.
- **Actions:**
  - Created visualizations to compare model performances.
  - Analyzed whether models with more correlated features and larger training data performed better.
  - Provided explanations for any deviations from expected results.

## Repository Structure

- `README.md`: This file, providing an overview of the repository contents and assignment details.
- `Portfolio 2_Analysing E-Commerce Data.ipynb`: The main assignment file containing questions, solutions, code, and analysis.

## Contact Information

For any queries or further information, please contact me at [nafialhasan@gmail.com].
