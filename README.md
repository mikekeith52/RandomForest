# Random Forest
 Using Random Forest to predict the presence of heart disease. See [RandomForestClassifier documentation](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html) from scikit-learn.

## About
With Random Forest, it is important to avoid overfitting and maximize out-of-sample accuracy by optimizing the model's hyperparameters. The following parameters are optimized in this example:
- `n_estimators`
- `max_depth`
- `max_features`

The following optimization techniques are used:
- OOB error reduction
- grid search with 10-folds cross validation

The following feature importance techniques are used:
- Gini impurity
- Permutation feature importance

## Installation
- Download [Anaconda](https://www.anaconda.com/)
- Download source code and install [requirements](requirements.txt)

## Data
The heart disease dataset from [Kaggle](https://www.kaggle.com/ronitf/heart-disease-uci) is utilized

## Results
Using the following parameters:
- `n_estimators = 90`
- `max_depth = 2`
- `max_featres = 'sqrt'`

An in-sample F1 score of 88.81% and an out-of-sample F1 score of 88% are obtained. With any machine learning model, ideally you hope to obtain an in-sample of accuracy a bit better than an out-of-sample accuracy. That way, you know your model is neither over nor underfit. Use these criteria, the modeling project was a success.