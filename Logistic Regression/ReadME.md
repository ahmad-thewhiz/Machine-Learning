# Logistic Regression in Machine Learning

## Introduction
Logistic Regression is a classification technique used in machine learning. It's used when the outcome variable is categorical. In this article, we'll explore the basics of Logistic Regression, including gradient descent, and how to build a classification model.

## Why Not Linear Regression for Classification?
Linear Regression is not suitable for classification problems because it produces continuous values, making it challenging to set a classification threshold. This can lead to incorrect classifications, which can have serious consequences.

## Logistic Regression
Logistic Regression is a classification technique that models a dependent variable with two possible classes. It's used for binary data and overcomes the limitations of linear regression for classification problems.

## Types of Logistic Regression
Logistic Regression can be categorized into three types:
1. **Binomial**: For binary target variables (e.g., spam or not spam).
2. **Multinomial**: For three or more possible types without quantitative significance (e.g., disease prediction).
3. **Ordinal**: For ordered categories (e.g., web series ratings).

## Sigmoid Function
In Logistic Regression, a sigmoid function is used to map predicted values to probabilities, ensuring the output is between 0 and 1. This function has a non-negative derivative at each point and a single inflection point.

The sigmoid function is defined as follows:
Where `z = θ_0 + θ_1 * x_1 + θ_2 * x_2 + ... + θ_n * x_n`

## Cost Function
The cost function measures the error between predicted and expected values. For Logistic Regression, the cost function is defined as follows:

## Gradient Descent for Logistic Regression
Gradient descent is used to find the optimal values of model parameters (θ) that minimize the cost function. The update rule for gradient descent in logistic regression is:

Where:
- θ_j is the j-th model parameter.
- α is the learning rate.
- m is the number of training examples.
- h_θ(x^(i)) is the predicted value for the i-th example.
- y^(i) is the actual target value.
- x_j^(i) is the j-th feature for the i-th example.

## Decision Boundary
The decision boundary in logistic regression is the boundary that separates the two classes in a binary classification problem. It's a line (in 2D) or a hyperplane (in higher dimensions) where the probability of belonging to one class is equal to the probability of belonging to the other class.

The decision boundary can be linear or non-linear, depending on the model and data. In a 2D space, the decision boundary can be represented as:

Solving for x_2 yields:
In higher dimensions, the decision boundary is a hyperplane determined by the model parameters.

## Building a Logistic Regression Model

### Step 1: Importing Libraries
- Import Pandas and Numpy libraries.
- Read the dataset (e.g., Heart Diseases data).

### Step 2: Cleaning the Dataset
- Handle missing data.
- Drop unnecessary columns.

### Step 3: Analyzing the Dataset
- Create separate dataframes for high and low-risk heart disease groups.
- Scale the data.

### Step 4: Preparing the Model
- Split the dataset into training and testing data.
- Fit the Logistic Regression model.
- Evaluate the model's performance.

## Advantages of Logistic Regression
- Efficient for classification problems.
- Easy to implement and interpret.
- Good performance with linearly separable datasets.

## Disadvantages of Logistic Regression
- Assumes linearity between variables.
- Limited to simple boundaries.
- Can be outperformed by more complex algorithms.

## Conclusion
Logistic Regression is a powerful tool for classification problems. We've covered its basics, types, cost function, gradient descent, decision boundaries, and the steps to build a classification model. Consider its advantages and limitations when choosing it for your machine learning tasks.



