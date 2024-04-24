# SC1015_proj

## Table of Contents
- [SC1015 Data Science and Analytics Project - Telco Churn Prediction](#sc1015-data-science-and-analytics-project---telco-churn-prediction)
- [Table of Contents](#table-of-contents)
- [Video Presentation](#video-presentation)
- [Background](#background)
- [Problem Statement](#problem-statement)
- [Approach](#approach)
- [Introduction to Codebase](#introduction-to-codebase)
  - [Exploratory Data Analysis](#exploratory-data-analysis) 
  - [Machine Learning Algorithms](#machine-learning-algorithms)


## Video Presentation 
insert link

## Background
The global telecom services market is expanding given the rapid advancements in technology, such as 5G, and increased digital communications usage. However, given how prevalent telecom services are in people's lives, customers easily get frustrated at any performance errors and have a high tendency to switch away.

High churn rate is relevant in the telecom industry and this is problematic given the industry's large fixed infrastructures that need to be covered by revenue.

## Problem Statement 
Will customer A churn if he has the following attributes?

## Dataset
We used the Telco Customer Churn dataset from Kaggle, which simulates the customer statistics of a telecom company.

## Approach 
- We first explored the dataset, finding the variables with highest correlation to churn. We note that there is a large class imbalance in the dataset and thus applied resampling techniques to ensure that the dataset is more balanced, in hopes of improving the model's accuracy. After cleaning the data, we then identified the 5 most correlated variables as inputs to our ML/AI models. The output will be a yes/no prediction
## Introduction to Codebase 
### Exploratory Data Analysis
The dataset includes:
  - Services provided by the company
  - Account information
  - Customer demographic data
  - Churn status (whether customers left within the last month)
  
- #### Data Cleaning Steps:
  - Standardization: Each variable was standardized according to its context to ensure data consistency.
  - Handling Missing Values: Entries with null values were removed to improve data quality.
  - Removing Irrelevant Columns: Columns that were not relevant to our analysis or were redundant (e.g., TotalCharges, which can be derived from MonthlyCharges * tenure) were excluded.
- #### Data Analysis
  - Univariate Analysis:
      Initial exploration of data distribution for each variable was conducted.
  - Bivariate Analysis:
     - Numerical Variables: Utilized box plots and swarm plots to analyze the relationship between numerical variables and Churn.
     - Categorical Variables: Conducted Chi-Square tests to explore dependencies between categorical variables and Churn.

Identified and selected the top 5 variables most strongly related to Churn.

- #### Data Preprocessing
  - Encoding: Applied one-hot encoding for categorical variables and label encoding for ordinal variables.
  - Normalization: Normalized numerical variables to ensure model accuracy and performance.

### Machine Learning 
- #### Algorithms Used
  - #### 1. K-Nearest Neighbours
    - Simple model that classifies a new data point based on the majority vote of its 'k' nearest neighbors. The nearest neighbour will be defined by a distance metric and classifies the new point based on the predominant class of the neighbors. 
  - #### 2. Support Vector Machines
    - Finds a best fit hyperplane that distinctly classifies the data points. The best fit hyperplane is the one that leaves the maximum margin from both classes. This is especially useful in high dimensional spaces or when dealing with non-linear data (using a non-linear kernel).
  - #### 3. Random Forest Classifiers
    - An ensemble learning method that constructs multiple decision trees, selecting the class that is modal of the 2 classes. It adds randomness , searching for the best feature in a subset of features then aggregates the predictions made by each individual tree to decide on the final output. 
  - #### 4. Artificial Neural Networks
    - Consists of multiple layers of neurons, with each neuron having a set of weights and baises. These parameters are tuned for every batch of data to minimise a loss function fed into the model through backpropagation. 
  - #### Choice of Algorithms
    - These algorithms were chosen for their strengths and robustness in classification tasks. Given the simplicity of our dataset, small number of variables that were identified with data cleaning and the strong relationships of each individual dataset to churn, we believed that simple models, such as the above, would be able to sufficiently achieve good accuracy in our classification task.
    - Moreover, these models are all inherently different, using different principles for classification. By using these range of models, we hope to find the best performing one. 
