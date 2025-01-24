# Sampling-Assignment

## Overview
This repository contains the implementation of various sampling techniques applied to a credit card fraud detection dataset. The goal is to balance the dataset, apply five different sampling techniques, and evaluate the performance of five different machine learning models. The results of each sampling technique are evaluated based on accuracy scores, and the best performing sampling technique for each model is determined.

## Dataset
The dataset used in this project is the [Creditcard_data.csv](https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv), which contains information about credit card transactions. The 'Class' column represents whether a transaction is fraudulent (`1`) or not (`0`).

## Steps
1. **Data Loading**: The dataset is loaded from the provided GitHub URL.
2. **Data Preprocessing**: 
   - The dataset is cleaned and preprocessed.
   - Missing values are handled, if any.
   - The dataset is balanced using various sampling techniques:
     - **Sampling1**: Random Sampling 
     - **Sampling2**: Stratified Sampling
     - **Sampling3**: Cluster Sampling
     - **Sampling4**: Systematic Sampling
3. **Model Training**: The following machine learning models are applied:
   - **Model 1**: Random Forest Classifier
   - **Model 2**: Support Vector Classifier (SVC)
   - **Model 3**: Logistic Regression 
   - **Model 4**: Gaussian Naive Bayes
   - **Model 5**: Decision Tree Classifier
4. **Evaluation**: The models are evaluated based on accuracy for each sampling technique, and the best sampling method is identified for each model.

## Results
The accuracy scores for each model and sampling technique are summarized as follows:

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 |
|-------|-----------|-----------|-----------|-----------|
| M1    | 0.974     | 0.984     | 0.951     | 1.000     |
| M2    | 0.623     | 0.721     | 0.754     | 0.735     |
| M3    | 0.844     | 0.902     | 0.951     | 0.873     |
| M4    | 0.857     | 0.902     | 0.902     | 0.882     |
| M5    | 0.961     | 0.934     | 0.885     | 0.980     |



## Setup and Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/tanisha0016/Sampling-Assignment.git
    cd Sampling-Assignment
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the main Python script to execute the sampling and model evaluation:
    ```bash
    python Sampling_assignment.py
    ```

## Files
- **sampling_assignment.py**: Main Python script that implements data processing, sampling techniques, model training, and evaluation.
- **requirements.txt**: List of Python packages required to run the code.

## Conclusion
This project demonstrates the application of various sampling techniques to handle class imbalance in a dataset, and evaluates the performance of different machine learning models on the balanced data. The results help identify which sampling method is most effective for each model, and contribute to improving the predictive accuracy of fraud detection models.

## License
This project is licensed under the MIT License.
