# Missing Value Imputation Using Machine Learning Models

## Overview
This repository contains the Jupyter Notebook and supporting files for my research on machine learning approaches for imputing missing values in datasets. The goal of the project is to evaluate different models and determine which ones can reconstruct missing entries with high accuracy.

## Abstract
The Wireless sensor network is one of the major technologies used in precision farming. The network consists of devices that are equipped with sensors to monitor and collect data on the physical conditions of a farm. These devices are powered by batteries and so have a limited power supply. In addition, WSN is also prone to issues like packet loss due to interference from other foreign signals. These challenges affect the data collected, often resulting in incomplete data. For the data to be useful for precision farming, there is a need to impute the missing values. In this paper, we proposed four machine learning models that could impute the missing values accurately. They are: Iterative Singular Value Decomposition, Long Short-Term Memory, K-means and Agglomerative clustering.  
Using the evaluation metrics: Mean Absolute Error, Mean Squared Error, and Coefficient of Determination, the results after testing the model on two Datasets showed that Iterative Singular Decomposition was the best-performing model.

## Models Implemented
- **Iterative SVD** – Uses low-rank matrix approximations to fill in missing values.
- **LSTM** – A neural network capable of modeling sequential data and temporal dependencies.
- **K-Means** – Assigns samples to clusters and imputes missing values using cluster centroids.
- **Agglomerative Clustering** – A hierarchical clustering approach for estimating values based on similarity.



