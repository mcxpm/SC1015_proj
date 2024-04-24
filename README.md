# SC1015_proj

## Table of Contents
- [SC1015 Data Science and Analytics Project - Telco Churn Prediction](#sc1015-data-science-and-analytics-project---telco-churn-prediction)
- [Table of Contents](#table-of-contents)
- [Video Presentation](#video-presentation)
- [Current Problems](#current-problems)
  - [1. Problem One](#1-problem-one)
  - [2. Problem Two](#2-problem-two)
- [Problem Statement](#problem-statement)
- [Approach](#approach)
- [Introduction to Codebase](#introduction-to-codebase)
  - [Data Cleaning](#data-cleaning)
  - [Data Exploration](#data-exploration)
  - [Data Visualisation](#data-visualisation)
  - [Data Preprocessing](#data-preprocessing)
  - [Machine Learning Algorithms](#machine-learning-algorithms)


## Video Presentation 
insert link

## Current Problems 
### 1. ??? 

### 2. ??? 


## Problem Statement 

## Approach 

## Introduction to Codebase 
### Data Cleaning 
### Data Exploration 
### Data Visualisation 
### Data Prepreprocessing 
### Machine Learning Algorithms 
[Algorithms Used]
- [1. K-Nearest Neighbours]
  - Simple model that classifies a new data point based on the majority vote of its 'k' nearest neighbors. The nearest neighbour will be defined by a distance metric and classifies the new point based on the predominant class of the neighbors. 
- [2. Support Vector Machines]
  - Finds a best fit hyperplane that distinctly classifies the data points. The best fit hyperplane is the one that leaves the maximum margin from both classes. This is especially useful in high dimensional spaces or when dealing with non-linear data.
- [3. Random Forest Classifiers]
  - An ensemble learning method that constructs multiple decision trees, selecting the class that is modal of the 2 classes. It adds randomness , searching for the best feature in a subset of features then aggregates the predictions made by each individual tree to decide on the final output. 
- [4. Artificial Neural Networks]
  - Consists of multiple layers of neurons, with each neuron having a set of weights and baises. These parameters are tuned for every batch of data to minimise a loss function fed into the model through backpropagation. 
- [Choice of Algorithms]
  - These algorithms were chosen for their strengths and robustness in classification tasks. Given the simplicity of our dataset, small number of variables that were identified with data cleaning and the strong relationships of each individual dataset to churn, we believed that simple models, such as the above, would be able to sufficiently achieve good accuracy in our classification task.
  - Moreover, these models are all inherently different, using different principles for classification. By using these range of models, we hope to find the best performing one. 
