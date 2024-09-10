# Breast-Cancer-binary-classification
Implemented a stochastic gradient descent model with regularization for binary classification of malignant and benign tumors
Data Preprocessing:

Loaded and cleaned the dataset by dropping unnecessary columns and mapping the 'diagnosis' column to binary values (1.0 for Malignant, -1.0 for Benign).
Explored data with heatmaps, count plots, and violin plots.
Standardized features by transforming them to have a mean of 0 and standard deviation of 1.
Feature Reduction:

Correlation-Based Reduction: Removed highly correlated features (correlation > 0.9).
Statistical Significance Reduction: Dropped features with p-values > 0.05 using OLS regression.
Model Training (SVM using Stochastic Gradient Descent):

Defined functions for gradient calculation and cost evaluation with regularization.
Implemented stochastic gradient descent (SGD) to iteratively update weights, minimizing hinge loss.
Evaluation:

Split the data into training and test sets.
Made predictions on both sets and evaluated accuracy using accuracy_score.
Visualized the results by plotting y_test vs y_test_pred.
This process combines feature reduction and SGD to train an SVM model for tumor classification, with accuracy as the evaluation metric.
