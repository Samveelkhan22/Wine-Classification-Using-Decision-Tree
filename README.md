# Wine Classification Using Decision Tree

This repository contains the implementation of a decision tree classifier to predict wine classes based on chemical analysis data. The classifier is trained using the ID3 algorithm and visualized to understand the classification process.

## Problem Definition and Design

The problem involves creating a predictive decision tree model to classify wine types (class_0, class_1, and class_2) based on 13 features obtained from chemical analysis. The dataset includes wines from three different cultivators in Italy.

## Methodology

1. **Data Loading and Preparation**:
   - Load the wine dataset using `sklearn.datasets`.
   - Convert the dataset into a pandas DataFrame for easier manipulation.
   - Split the data into training and testing sets.

2. **Model Training**:
   - Use `DecisionTreeClassifier` from `scikit-learn` with the `entropy` criterion to implement the ID3 algorithm.
   - Train the model using the training data.

3. **Evaluation**:
   - Predict the wine classes for the test data.
   - Calculate the accuracy of the model using `accuracy_score`.

4. **Visualization**:
   - Visualize the trained decision tree using `plot_tree` from `matplotlib`.

## Detailed Explanation of Trained Decision Tree

The decision tree classifier splits the data at each node based on the feature that provides the highest information gain (measured by entropy). Each leaf node represents a wine class. The depth and complexity of the tree depend on the training data and the features used.

## Insightful Discussion

The decision tree visualization provides insights into the decision-making process. Important features for classification, such as alcohol content and phenol levels, are highlighted in the tree. The model achieved an accuracy of 85.19%, indicating good performance.

## Implementation

The implementation is provided in the Jupyter notebook `Wine_Classification.ipynb`.

## Requirements

Install the required packages using the following command:

```bash
pip install -r requirements.txt
