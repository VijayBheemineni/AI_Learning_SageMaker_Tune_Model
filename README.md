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

### XGBoost Hyperparameters (Beginner Learning Notes)

**Reference:** [AWS SageMaker XGBoost Hyperparameters Documentation](https://docs.aws.amazon.com/sagemaker/latest/dg/xgboost_hyperparameters.html)

**TODO:**
- Learn more indepth about XGBoost Hyperparameters

While learning how XGBoost works in AWS SageMaker, I learned that **hyperparameters** are settings that control *how* the model learns from data. XGBoost groups its hyperparameters into a few main categories. Below is my high-level understanding of them.

---

#### 1️⃣ General Parameters

These hyperparameters control the **overall behavior** of the XGBoost model.

**Example:**
- **booster**  
  Decides what type of model XGBoost should use for each training step (for example, tree-based models).

---

#### 2️⃣ Booster Parameters

These hyperparameters control **how the model grows and becomes more complex**. They directly affect model performance and overfitting.

**Examples:**
- **max_depth**  
  Controls how deep each decision tree can grow.  
  A deeper tree can learn more patterns but may overfit the data.

- **num_round**  
  The number of trees used during training.  
  More trees can improve accuracy but also increase the risk of overfitting.

---

#### 3️⃣ Learning Task Parameters

These hyperparameters define **what the model is trying to optimize** and how its performance is measured.

**Examples:**
- **objective**  
  Defines the loss function the model tries to minimize.  
  For binary classification problems, common values include:
  - `binary:logistic`
  - `binary:logitraw`
  - `binary:hinge`

- **eval_metric**  
  Specifies how the model is evaluated on validation data.  
  A common example is `auc`, which measures how well the model separates classes.

---

### Hyperparameter tuning approaches

**TODO:**
- Learn more indepth about manual and automated tuning options

Hyperparameter tuning can be done manually or through automation using tool (AMT :- Amazon Sagemaker Automatic Model Tuning)

---

#### 1️⃣ Manual

- **Grid Search**
- **Random Search**
- **Bayesian Search**

---

#### 2️⃣ Automated

We can perform automated hyperparameter tuning using "AMT" (Amazon Sagemaker Automatic Model Tuning)

---
