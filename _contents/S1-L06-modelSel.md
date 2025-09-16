---
layout: post
title: Workflow for model selection
lecture: S1-ModelSelect
lectureVersion: current
extraContent: 
notes: <a href="https://jakevdp.github.io/PythonDataScienceHandbook/05.03-hyperparameters-and-model-validation.html"> hyperpara select notebook </a> + <a href="http://scikit-learn.org/stable/model_selection.html">flow API </a> 
morenotes: <a href="https://web.stanford.edu/~hastie/ElemStatLearn/">ELS Ch5 </a>
video: <a href="https://youtu.be/QJC-GbMP95E"> M1</a>
categories: tabular
tags:
- 2Regression
- Nonlinear
- ModelSelection
- Local
---

- Notebook Resources: [notebook/L6-Hyperparameters-and-Model-Validation.ipynb]({{ site.baseurl }}/notebook/L6-Hyperparameters-and-Model-Validation.ipynb)


# Understanding Linear Regression with Basis Functions

## Study Guide

This study guide is designed to review your understanding of Linear Regression with Basis Functions Expansion, as presented in the provided lecture material.

## I. Core Concepts of Linear Regression

### Definition of Regression
**What is the primary characteristic of the y variable in a regression task?**

### Goal of Linear Regression with Basis Expansion
**How does Linear Regression (LR) achieve the ability to model non-linear relationships using basis functions?**

### Key Components of a Machine Learning Task
**Identify and briefly describe the four fundamental components mentioned for any machine learning task:**

- **Task**: What needs to be predicted
- **Representation**: How data and functions are structured
- **Score Function**: Metric to evaluate model performance
- **Search/Optimization**: Algorithms to find optimal parameters

### Parameters vs. Models
**Differentiate between "models" and "parameters" in the context of machine learning.**

### Optimization Methods
**List the three primary methods mentioned for optimizing the Sum of Squared Error:**

1. Normal Equation
2. Gradient Descent (GD)
3. Stochastic Gradient Descent (SGD)

### "KEY" Insight
**Explain the fundamental implication of having predefined basis functions on the nature of the learning problem.**

## II. Basis Functions Expansion

### Purpose of Basis Functions
**Why are basis functions introduced in linear regression?**

### Types of Basis Functions
**Name at least three different types of basis functions mentioned in the lecture:**

- Polynomial basis functions
- Radial Basis Functions (RBFs)
- Trigonometric basis functions

### Polynomial Regression

**What is the specific form of the basis function φ(x) for polynomial regression up to degree two (d=2)?**

For degree 2: φ(x) = [1, x, x²]ᵀ

**How is the prediction ŷ formulated using polynomial basis functions?**

ŷ = θᵀφ(x) = θ₀ + θ₁x + θ₂x²

### Radial Basis Functions (RBFs)

**Define what an RBF is in terms of its dependency.**
RBFs are functions whose output depends only on the distance from a central point.

**Describe the characteristic behavior of a Gaussian RBF as distance from its center increases.**
The output decreases exponentially as the distance from the center increases, creating a bell-shaped curve.

**What are the "hyperparameters" that users need to define for RBF basis functions?**

- **Centers (μⱼ)**: The central points where RBFs are located
- **Widths (λⱼ)**: Parameters controlling the spread of the RBF

**Provide the general mathematical form of a Gaussian RBF, specifically φⱼ(x).**

φⱼ(x) = exp(-λⱼ||x - μⱼ||²)

## III. Parametric vs. Non-Parametric Models

### Parametric Learning Algorithm
**Define a parametric learning algorithm, using (unweighted) linear regression as an example. What is a key characteristic regarding the need for training data after fitting?**

Parametric algorithms have a fixed number of parameters that are learned from data. Once trained, the training data can be discarded as predictions are made using only the learned parameters.

### Non-Parametric Learning Algorithm
**Define a non-parametric learning algorithm, providing examples like K-Nearest Neighbor (KNN) or Locally Weighted Linear Regression. How does the "amount of knowledge" required to represent the hypothesis differ from parametric models?**

Non-parametric algorithms require the entire training dataset to be kept for making predictions. The amount of knowledge grows with the size of the training set.

## IV. Mathematical Notations and Formulas

### General Prediction Equation
**Write down the general equation for ŷ (predicted output) using basis functions φ(x) and weights θ.**

ŷ = θᵀφ(x)

### Normal Equation
**Provide the formula for calculating the optimal weight vector θ* using the Normal Equation, given φ(x) and y.**

θ* = (ΦᵀΦ)⁻¹Φᵀy

where Φ is the design matrix with rows φ(xᵢ)ᵀ

## Quiz: Linear Regression with Basis Functions

**Instructions**: Answer each question in 2-3 sentences.

1. How does Linear Regression with basis functions expansion allow for the modeling of non-linear relationships, despite being fundamentally a "linear" model?

2. What is the significance of the "KEY" insight mentioned in the lecture regarding predefined basis functions?

3. Describe the primary goal of the "Search/Optimization" component in a machine learning task, as it relates to the score function.

4. If you are performing polynomial regression with a degree up to three, what would be the form of the basis function vector φ(x)?

5. Explain why Radial Basis Functions (RBFs) are often described as "bell-shaped" or having an output that decreases with distance from a center.

6. What role do the "centers" and "widths" play in defining Radial Basis Functions?

7. Differentiate between the "Task" and "Representation" components of a machine learning problem.

8. Briefly explain the main difference in how parametric and non-parametric learning algorithms utilize training data after the initial fitting phase.

9. Which optimization methods, other than the Normal Equation, are mentioned for finding the optimal regression coefficients?

10. In the context of the general prediction equation ŷ = θᵀφ(x), what do θ and φ(x) represent, respectively?

## Quiz Answer Key

1. **Non-linear Modeling**: Linear Regression with basis functions models non-linear relationships by transforming the input features x into a higher-dimensional space using non-linear basis functions φ(x). The relationship between the transformed features φ(x) and the output y remains linear, allowing linear regression techniques to be applied.

2. **KEY Insight**: The "KEY" insight is that even when non-linear basis functions are used, the problem of learning the parameters from the data is still considered Linear Regression. This is because the model is linear with respect to the parameters θ, even if it's non-linear with respect to the original input x.

3. **Search/Optimization Goal**: The "Search/Optimization" component's primary goal is to find the set of model parameters that minimize (or maximize, depending on the objective) the score function. This process iteratively adjusts the parameters to achieve the best possible fit to the training data according to the defined score.

4. **Polynomial Basis Vector**: For polynomial regression with a degree up to three, the basis function vector φ(x) would be [1, x, x², x³]ᵀ. This expands the single input feature x into a set of features including its powers.

5. **RBF Bell Shape**: RBFs are "bell-shaped" because their output typically reaches a maximum at a central point and then decreases symmetrically as the input moves further away from that center. For Gaussian RBFs, this decay is exponential, creating a characteristic bell-like curve.

6. **RBF Centers and Widths**: In RBFs, "centers" (μⱼ) define the point in the input space where the basis function's influence is maximal, while "widths" (λⱼ) determine how rapidly the function's output decreases as the input moves away from that center, thus controlling the spread or local influence of the RBF.

7. **Task vs Representation**: "Task" defines what needs to be predicted (e.g., y is continuous for regression). "Representation" refers to how the input data x and its potential transformations f() are structured for the model, essentially defining the features used for prediction.

8. **Parametric vs Non-parametric Data Usage**: Parametric algorithms, once trained, can discard the training data as predictions are made solely using the learned, fixed parameters. Non-parametric algorithms, in contrast, require the entire training dataset to be kept available for making future predictions, as their "knowledge" grows with the data size.

9. **Other Optimization Methods**: Besides the Normal Equation, the lecture also mentions Gradient Descent (GD) and Stochastic Gradient Descent (SGD) as optimization methods for finding optimal regression coefficients by minimizing the Sum of Squared Error.

10. **Prediction Equation Components**: In ŷ = θᵀφ(x), θ represents the vector of regression coefficients (weights) that the model learns from the data. φ(x) represents the basis function expansion of the input x, which transforms the original features into a potentially higher-dimensional space.



## Glossary of Key Terms

- **Regression**: A type of machine learning task where the target variable (y) is continuous.

- **Linear Regression (LR)**: A statistical model that establishes a linear relationship between input features and a continuous output variable.

- **Basis Functions Expansion**: The process of transforming original input features (x) into a new set of (often non-linear) features (φ(x)) to allow linear models to capture non-linear relationships.

- **φ(x) (Phi(x))**: The vector or matrix representing the basis function expansion of the input data x.

- **θ (Theta)**: The vector of regression coefficients or weights that the model learns to associate with each basis function.

- **ŷ (y-hat)**: The predicted output value by the regression model.

- **Sum of Squared Error (SSE) / Least Squares**: A common loss function used in regression, which measures the sum of the squared differences between predicted and actual values. The goal is to minimize this error.

- **Normal Equation**: A closed-form solution for finding the optimal regression coefficients (θ*) that minimize the Sum of Squared Error. It involves matrix operations and does not require iterative optimization.

- **Gradient Descent (GD)**: An iterative optimization algorithm used to minimize the loss function by moving in the direction of the steepest descent of the gradient.

- **Stochastic Gradient Descent (SGD)**: A variant of Gradient Descent that updates parameters using the gradient of the loss function calculated on a single randomly chosen training example (or a small batch) at each step, making it faster for large datasets.

- **Polynomial Regression**: A type of linear regression that models the relationship between the independent variable x and the dependent variable y as an n-th degree polynomial in x, achieved through polynomial basis functions.

- **Radial Basis Functions (RBFs)**: A class of basis functions whose output depends on the distance from a central point. Gaussian RBFs are a common type, characterized by bell-shaped curves.

- **Hyperparameters (of RBFs)**: Parameters of the RBF basis functions themselves that are not learned from the data, but rather predefined by the user, such as the "centers" (μⱼ) and "widths" (λⱼ) of the RBFs.

- **Parametric Learning Algorithm**: A type of machine learning algorithm that has a fixed, finite number of parameters that are fit to the data. Once fit, the training data is no longer needed for predictions. Example: Linear Regression.

- **Non-Parametric Learning Algorithm**: A type of machine learning algorithm where the amount of knowledge required to represent the hypothesis grows with the size of the training set. The entire training set is often needed to make future predictions. Examples: K-Nearest Neighbor (KNN), Locally Weighted Linear Regression.