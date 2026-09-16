# Decision Tree and Random Forest Assignment

This folder contains an experiment-driven participant assignment using the UCI Dry Bean classification dataset.

## Dataset

The UCI Dry Bean dataset contains 13,611 observations, 16 numerical shape features, and seven bean varieties. The notebook downloads the dataset through the official UCI Python interface.

Dataset: https://archive.ics.uci.edu/dataset/602/dry+bean

## Topics Covered

- Multiclass classification with Decision Trees and Random Forests
- Stratified train-validation-test splitting
- Underfitting and overfitting
- Maximum tree depth
- Minimum samples per leaf
- Gini, entropy, and log-loss split criteria
- Number of trees and out-of-bag score
- Random feature sampling with `max_features`
- Decision Tree and Random Forest impurity-based feature importance
- Feature-subset experiments
- Validation-based model selection
- Final evaluation with accuracy, macro precision, macro recall, macro F1, classification report, and confusion matrix

## Expected Performance Hints

Exact scores will vary with the selected hyperparameters, but these ranges can be used as a general check:

- A reasonable Decision Tree should reach approximately `0.89-0.91` validation accuracy.
- A well-tuned Random Forest should usually reach more than `0.91` accuracy and `0.92` macro F1.
- An OOB score close to `0.92` is a sensible Random Forest result.
- Very shallow trees should perform noticeably worse because they underfit.
- An unrestricted Decision Tree may achieve almost perfect training accuracy while performing worse on validation data.

Do not optimize only for these numbers. The experiment trends, validation-based model selection, and explanation of underfitting and overfitting are equally important. Scores below approximately `0.85` may indicate an issue with the split, target, model configuration, or evaluation code.

## Recommended Reading

[Comparison of Multiclass Classification Techniques Using Dry Bean Dataset](https://www.sciencedirect.com/science/article/pii/S2666307423000013?via%3Dihub)

Participants should go through this paper once. It is a very helpful example of how a research study approaches the same classification problem: understanding the dataset, preparing the data, handling class imbalance, comparing multiple machine-learning models, selecting evaluation metrics, and interpreting experimental results.

Use the paper to understand the research process and compare its methodology with your assignment. Your results do not need to reproduce the paper's exact scores because the data split, preprocessing choices, balancing methods, and model settings may differ.

## File

- `dry_bean_decision_tree_random_forest_assignment.ipynb`: participant assignment notebook
