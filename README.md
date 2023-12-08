# Diabetes Detection using Machine Learning with Feature Engineering

This repository deals with the development of a model which can detect whether a person has diabetes or not by looking at Diabetes Health Indicators Dataset provided by survey responses from cleaned BRFSS 2015
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset

Here's how the training and evaluation can be done as per the code provided in different files:

1. First step is to generate the training data after applying the pre-processing on the data using `pre_processing.ipynb`
2. Then we can train and evaluate different models on the processed dataset using `Binary_Split5050` dataset as well as the `3 Class Imbalanced` dataset
3. Use `logreg_svm.ipynb` to train and evaluate logistic regression and svm models
4. Use `final_project_rf_notebook.ipynb` to train and evaluate random forest model
5. Use `mlp_diabetes_simple.ipynb` to train and evaluate MLP classifier
6. Use `xgboost_diabetes.ipynb` to train and evalute XGBoost classifier
7. For the evaluation of all the models, use `diabetes_classification.ipynb` since it includes training and evaluation code for all the models
8. The training parameters for `MLP Classifier` were finalized using GridSearch and KFold cross validation. The training code and evaluation code can be found in the directory `mlp_gridsearch`
9. The training parameters for `XGBoost Classifier` were finalized using GridSearch and KFold cross validation. The training code and evaluation code can be found in the directory `xgboost_parameter_finding.ipynb`
10. An experiment was conducted using an undersampling technique to cater for imbalanced data which is provided in `undersampling_experiment.ipynb`