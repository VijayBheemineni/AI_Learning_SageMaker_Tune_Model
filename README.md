# AI_Learning_SageMaker_Tune_Model

This repository is part of my AI learning journey using AWS SageMaker, with a focus on tuning machine learning models to improve performance. After training an initial model, this repo explores how adjusting hyperparameters can impact results such as accuracy, recall, and overall model quality.

Using SageMaker and XGBoost, I experiment with different hyperparameter values and observe how small changes influence model behavior.

## Task 1: What Are Hyperparameters and Why Are They Used?

When training a machine learning model, hyperparameters are settings that we choose before training starts. They control how the model learns from the data, not what the final learned values are.

You can think of hyperparameters like rules or knobs that guide the training process. For example, they decide how fast the model should learn, how complex it is allowed to become, or how long it should keep training.

Hyperparameters are important because:
- They affect how well the model learns patterns from data
- They help prevent the model from overfitting or underfitting
- They allow us to adjust model behavior without changing the data
