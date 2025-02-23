# Customer Churn Prediction (Deep Learning)

## Overview
This project predicts customer churn using an Artificial Neural Network (ANN) built with TensorFlow and Keras. The dataset contains customer details such as demographics, transaction history, and banking details. The goal is to classify whether a customer is likely to churn.

## Features
- **Data Preprocessing:**  
  - Handling missing values and duplicates.  
  - Encoding categorical variables (`Geography`, `Gender`) using one-hot encoding.  
  - Standardizing numerical features with `StandardScaler`.  

- **Deep Learning Model (ANN):**  
  - Input Layer: 11 neurons (matching feature count).  
  - Hidden Layers: Two Dense layers with ReLU activation.  
  - Output Layer: A single neuron with Sigmoid activation for binary classification.  

- **Training & Evaluation:**  
  - Model compiled with Binary Crossentropy loss and Adam optimizer.  
  - Trained for 100 epochs with validation split (20%).  
  - Performance analyzed using accuracy and loss plots.  

## Dataset
The dataset used is `Churn_Modelling.csv`, which includes:
- Credit score  
- Age  
- Balance  
- Number of products  
- Tenure  
- Geography (encoded)  
- Gender (encoded)  
- Churn label (`Exited` - 1 or 0)  

## Dependencies
To run this notebook, install the required Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
