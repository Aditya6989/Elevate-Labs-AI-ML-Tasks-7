# SVM Binary Classification

## Overview

This project demonstrates binary classification using Support Vector Machines (SVM) in Python. The script loads a dataset, trains SVM models with both linear and RBF kernels, visualizes the decision boundary (if data is 2D), and evaluates model performance through cross-validation and hyperparameter tuning.

## Features

* Loads and preprocesses a binary classification dataset.
* Trains SVM models with both Linear and RBF kernels.
* Visualizes the decision boundary for 2D data.
* Tunes hyperparameters (C and gamma) using GridSearchCV.
* Cross-validates the model to evaluate its performance.

## Requirements

* Python 3.x
* pandas
* numpy
* matplotlib
* scikit-learn
* mlxtend (for visualization)

## Installation

To install the required packages, run:

```
pip install pandas numpy matplotlib scikit-learn mlxtend
```

## Usage

1. Place your dataset file (CSV format) in the same directory.
2. Run the script:

```
python svm_binary_classification.py
```

## Output

* Prints dataset information and model accuracy for both kernels.
* Displays the optimal hyperparameters from GridSearchCV.
* Plots the decision boundary if the data is 2D.

## Notes

* The dataset should have the features in columns except the last one, which should be the target label.
* If the data has more than 2 features, decision boundary visualization will be skipped.

## License

MIT License
