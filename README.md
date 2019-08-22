 # AI Skunkworks Project - Hyperparameters Database
## Goals and Objectives :
In statistics, hyperparameter is a parameter from a prior distribution; it captures the prior belief before data is observed.
In any machine learning algorithms, these parameters need to be initialized before training amodel.
Hyperparameters are important because they directly control the behaviour of the training algorithm and have a significant impact on the performance of the model is being trained.
Our aim is to find proper hyperparameter with proper tuning for our dataset which would help the database team in modelling the database schema in an efficient way. We would create H2O models for this dataset for getting proper hyperparameters.
Background Research:
Hyperparameters are variables that we need to set before applying a learning algorithm to a dataset. In machine learning scenarios, a significant part of model performance depends on the hyperparameter values selected. The goal of hyperparameter exploration is to search across various hyperparameter configurations to find the one that results in the optimal performance. The challenge with hyperparameters is that there are no magic number that works everywhere. The best numbers depend on each task and each dataset. The hyperparameter database to be developed as a part of this project is an open resource with algorithms, tools, and data that allows users to visualize and understand how to choose hyperparameters that maximize the predictive power of their models. Phase I of the project involves selecting a unique dataset containing predicted target variables, hyperparameters, meta-data etc. by running different models (with varying hyperparameters) on it using H2O.

## Hyperparameters can be divided into 2 categories: 

## Optimizer hyperparameters
They are related more to the optimization and training process
If our learning rate is too small than optimal value then it would take a much longer time (hundreds or thousands) of epochs to reach the ideal state
If our learning rate is too large than optimal value then it would overshoot the ideal state and our algorithm might not converge

## Model Specific hyperparameters
They are more involved in the structure of the model
Currently, the hyperparameter database analyzes the effect of hyperparameters on the following algorithms: Distributed Random Forest (DRF), Generalized Linear Model (GLM), Gradient Boosting Machine (GBM). Nai¨ve Bayes Classifier, Stacked Ensembles, XGBoost and Deep Learning Models (Neural Networks).

Algorithms and code sources:

Deciding the algorithms based on the type of dataset(Classification or Regression algorithm)
We would be using H20 python module.
This Python module provides access to the H2O JVM, as well as its extensions, objects, machine-learning algorithms, and modeling support capabilities, such as basic munging and feature generation.
How and what the team will work on?:

## Find a dataset
Figure out the algorithms that will work for that dataset. The type of algorithm like classification or Regression algorithm.
Perform H2O in python for generating various models at various runtime.
Suppose hypothetically if five algorithms are used then the best models for those algorithms will be selected to get the hyperparameter.
All the models will be stored for reference irrespective of it being best or the worst model.
Further communicate with the database team to give them the insight of the data and the conclusions drawn from the H2O analysis. This would help them in designing the ER Diagrams and designing the data models and schema.
We will try to follow this process on as many datasets as possible within the given time constraint.
Challenges:

## Implementing H2O analysis.
Getting optimized hyperparameters.
The model might overfit for the training dataset which will not work well on the test dataset.
Other challenge would be to tune model and feature parameters well.