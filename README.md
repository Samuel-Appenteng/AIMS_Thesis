# Machine Learning for Predicting Agricultural and Wireless Communication Parameters in a Wireless Sensor Network

## Overview

This repository contains the Jupyter Notebook and supporting files for my research on machine learning approaches for imputing missing values in datasets. The goal of the project is to evaluate different models and determine which ones can reconstruct missing entries with high accuracy.

## Abstract

The Wireless sensor network is one of the major technologies used in precision farming. The network consists of devices that are equipped with sensors to monitor and collect data on the physical conditions of a farm. These devices are powered by batteries and so have a limited power supply. In addition, WSN is also prone to issues like packet loss due to interference from other foreign signals. These challenges affect the data collected, often resulting in incomplete data. For the data to be useful for precision farming, there is a need to impute the missing values. In this paper, we proposed four machine learning models that could impute the missing values accurately. They are: Iterative Singular Value Decomposition, Long Short-Term Memory, K-means and Agglomerative clustering.
Using the evaluation metrics: Mean Absolute Error, Mean Squared Error, and Coefficient of Determination, the results after testing the model on two Datasets showed that Iterative Singular Decomposition was the best-performing model.

---

## Research Objective

The main objective of this research is to investigate and compare machine learning approaches for imputing missing values in Wireless Sensor Network datasets.

The research focuses on evaluating whether different machine learning and data-driven techniques can accurately reconstruct missing observations while preserving the underlying patterns in the original datasets.

### Specific Objectives

* Identify and investigate missing values in Wireless Sensor Network datasets.
* Prepare and preprocess the datasets for machine learning-based imputation.
* Implement four different imputation approaches.
* Evaluate the performance of each approach.
* Compare the models using appropriate evaluation metrics.
* Identify the best-performing model for missing-value reconstruction.

---

## Datasets

Two datasets were used in this study to evaluate the performance of the proposed imputation approaches.

The datasets contain parameters associated with **agricultural monitoring and wireless sensor networks**. The experiments were designed to assess how accurately the different approaches could reconstruct missing observations.

## Methodology

The research follows a machine learning-based missing-value imputation workflow:

```text
Original Dataset
       │
       ▼
Data Preprocessing
       │
       ▼
Data Exploration
       │
       ▼
Missing-Value Preparation
       │
       ▼
┌──────────────────────────────┐
│      Imputation Models       │
│                              │
│  • Iterative SVD             │
│  • LSTM                      │
│  • K-Means                   │
│  • Agglomerative Clustering  │
└──────────────┬───────────────┘
               │
               ▼
       Imputed Values
               │
               ▼
      Performance Evaluation
               │
               ▼
        Model Comparison
```

---

## Data Preprocessing

The datasets were prepared before applying the different imputation techniques.

The preprocessing and exploratory analysis involved:

* Loading and inspecting the datasets.
* Examining the structure and characteristics of the data.
* Identifying missing observations.
* Preparing the data for the different models.
* Creating incomplete datasets for the imputation experiments.
* Preparing the data for model evaluation.

The processed data was then used as input for the four imputation approaches.

---

# Models Implemented

## 1. Iterative Singular Value Decomposition (SVD)

Iterative SVD uses matrix decomposition and low-rank approximation to reconstruct missing values.

The dataset is represented as a matrix, and Singular Value Decomposition is used to identify the underlying structure within the observed data.

The missing values are then estimated iteratively using the reconstructed matrix.

---

## 2. Long Short-Term Memory (LSTM)

Long Short-Term Memory (LSTM) is a type of recurrent neural network designed to learn patterns and dependencies within sequential data.

LSTM was implemented to investigate whether temporal relationships within the sensor observations could be used to reconstruct missing values.

---

## 3. K-Means Clustering

K-Means is an unsupervised machine learning algorithm that groups observations into clusters based on their similarity.

In this research, K-Means was investigated as a clustering-based approach for estimating missing values from similar observations within the dataset.

---

## 4. Agglomerative Clustering

Agglomerative Clustering is a hierarchical clustering technique that progressively groups similar observations.

The method was investigated as another clustering-based approach for reconstructing missing observations.

---

# Evaluation Metrics

The four approaches were evaluated using three metrics:

### Mean Absolute Error (MAE)

MAE measures the average absolute difference between the actual values and the imputed values.

**Lower MAE indicates better performance.**

### Mean Squared Error (MSE)

MSE measures the average squared difference between the actual values and the imputed values.

**Lower MSE indicates better performance.**

### Coefficient of Determination (R²)

The coefficient of determination measures how well the imputed values correspond to the actual observations.

**Higher R² indicates better performance.**

| Metric | Better Performance |
| ------ | ------------------ |
| MAE    | Lower ↓            |
| MSE    | Lower ↓            |
| R²     | Higher ↑           |

---

# Model Performance Comparison

The performance of the four imputation approaches was compared using MAE, MSE, and R² across the two datasets.

## Dataset 1

**Insert your Dataset 1 model-comparison chart here.**

```text
[ INSERT DATASET 1 MODEL COMPARISON CHART ]
```

*Figure 1: Performance comparison of the four imputation approaches on Dataset 1.*

---

## Dataset 2

**Insert your Dataset 2 model-comparison chart here.**

```text
[ INSERT DATASET 2 MODEL COMPARISON CHART ]
```

*Figure 2: Performance comparison of the four imputation approaches on Dataset 2.*

---

## Overall Model Comparison

**Insert your overall model-comparison chart here, if you have one.**

```text
[ INSERT OVERALL MODEL COMPARISON CHART ]
```

*Figure 3: Overall comparison of the four imputation approaches.*

---

# Results

The four approaches were evaluated based on their ability to reconstruct missing observations.

The evaluation was conducted using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Coefficient of Determination (R²)

The results obtained from the two datasets showed that **Iterative Singular Value Decomposition (SVD) was the best-performing approach** among the four methods investigated.

This indicates that the underlying structure within the datasets could be effectively captured through the low-rank matrix representation used by Iterative SVD.

---

# Key Findings

The main findings of the research are:

* Missing values can significantly affect the usefulness of Wireless Sensor Network datasets.
* Machine learning approaches can be used to reconstruct missing sensor observations.
* The performance of an imputation method depends on the characteristics of the dataset.
* The four approaches produced different levels of imputation accuracy.
* **Iterative SVD achieved the best overall performance across the two datasets.**

---

# Technologies Used

### Programming Language

* Python

### Development Environment

* Jupyter Notebook

### Data Processing

* NumPy
* Pandas

### Machine Learning

* Scikit-learn

### Deep Learning

* TensorFlow / Keras

### Data Visualization

* Matplotlib




---

# Installation

## 1. Clone the repository

```bash
git clone https://github.com/Samuel-Appenteng/YOUR-REPOSITORY-NAME.git
```

Move into the repository:

```bash
cd YOUR-REPOSITORY-NAME
```

## 2. Create a virtual environment

### Windows

```bash
python -m venv venv
```

Activate the environment:

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
python3 -m venv venv
```

Activate it:

```bash
source venv/bin/activate
```

## 3. Install dependencies

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow jupyter
```

---

# Running the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Or start JupyterLab:

```bash
jupyter lab
```

Open the research notebook and run the cells sequentially.

The notebook contains the data preprocessing, implementation of the four imputation approaches, evaluation procedures, and model comparisons used in the research.

---

# Reproducibility

To reproduce the analysis:

1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install the required dependencies.
4. Ensure the datasets are located in the appropriate directories.
5. Open the Jupyter Notebook.
6. Run the notebook cells sequentially.
7. Review the resulting evaluation metrics and model-comparison charts.

---

# Future Work

Possible directions for future research include:

* Testing the approaches on larger Wireless Sensor Network datasets.
* Investigating different percentages and patterns of missing data.
* Exploring additional deep-learning architectures.
* Investigating hybrid machine learning imputation methods.
* Incorporating both spatial and temporal relationships in sensor data.
* Exploring Transformer-based approaches for sequential sensor data.
* Evaluating the computational cost of the approaches.
* Testing the approaches in real-time Wireless Sensor Network environments.

---

# Author

**Samuel Appenteng**

Master's Student in Mathematical Sciences

Research interests include:

* Machine Learning
* Artificial Intelligence
* Mathematical Modelling
* Scientific Computing
* Statistical Modelling
* Wireless Sensor Networks
* Precision Agriculture
* Data-driven scientific computing

---

## Acknowledgements

This repository contains computational work associated with my research on machine learning approaches for missing-value imputation in Wireless Sensor Networks and their potential application to precision agriculture.
