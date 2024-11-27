# Keras Based Hybrid Transformer LSTM Model for Customer Lifetime Value
Hybrid Transformer-LSTM for Customer Lifetime Value Prediction
This repository contains a self-contained Jupyter notebook implementing a hybrid architecture for handling irregular customer purchase patterns and predicting customer lifetime value.

## Introduction

- Traditional approaches often treat each customer's purchase history as an isolated timeseries, much like how basic forecasting models handle independent sequences. However, customer behavior exists within a complex network of interactions, influenced by various factors such as seasonal patterns, demographic similarities, and purchase dependencies - similar to how we observe interconnected patterns in financial and human activity data.

- This approach leverages the power of recurrent neural networks and transformer architecture, which maintain state between inputs and can effectively process sequential customer interaction data. This is particularly valuable because, like other predictive tasks, CLV prediction requires understanding both historical patterns and temporal dependencies in customer behavior.

## Key Features

- **Efficient Processing of Irregular Data**: Combines principles from statistical ARMA based time series forecasting models with deep learning capabilities to handle non-linear relationships in customer purchase patterns

## Evaluation Metrics

The model is evaluated using:
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R2 Coefficiecnt of Model Variation (R2)
- Symmetric Mean Absolute Error Percentage (sMape)
- Lorenz Curves
- Mutual Gini

## Usage

To run:
1. Open the Jupyter notebook
2. All required packages and implementations are included within
3. Execute cells sequentially

For Tensorflow dependencies please refer https://www.tensorflow.org/install/source#tested_build_configurations

Dependencies note: When installing keras-hub, brief snapshot of automatic upgrade of tensorflow and tensorboard to 2.18.0. If this is not desired use a virtual environment for this piece of code. 

Installing collected packages: tensorboard, tensorflow, tensorflow-text, keras-hub
  Attempting uninstall: tensorboard
    Found existing installation: tensorboard 2.17.1
    Uninstalling tensorboard-2.17.1:
      Successfully uninstalled tensorboard-2.17.1
  Attempting uninstall: tensorflow
    Found existing installation: tensorflow 2.17.1
    Uninstalling tensorflow-2.17.1:
      Successfully uninstalled tensorflow-2.17.1
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
tf-keras 2.17.0 requires tensorflow<2.18,>=2.17, but you have tensorflow 2.18.0 which is incompatible.
Successfully installed keras-hub-0.17.0 tensorboard-2.18.0 tensorflow-2.18.0 tensorflow-text-2.18.0

## Model Comparison

Benchmarked against:
- Traditional LSTM approaches

This tutorial implements a LSTM/Transformer based neural network architecture for predicting customer lifetime value, addressing key challenges including forecasting accuracy, long-term customer behavior patterns, and nonlinear purchasing patterns. The model demonstrates strong performance on multi-step CLV forecasting.
