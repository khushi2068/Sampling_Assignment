# Sampling Techniques in Machine Learning

This Python script demonstrates various sampling techniques commonly used in machine learning for handling imbalanced datasets. It includes implementations of simple random sampling, systematic sampling, cluster sampling, stratified sampling, and bootstrap sampling.

## Dataset
The dataset used in this script is [Creditcard_data.csv](https://raw.githubusercontent.com/AnjulaMehto/Sampling_Assignment/main/Creditcard_data.csv), containing credit card transaction data with a highly imbalanced target variable ('Class').

## Sampling Techniques

### 1. Simple Random Sampling
- The script performs simple random sampling on the dataset and evaluates the performance of several machine learning models.
- Models include Random Forest, Logistic Regression, Naive Bayes, Decision Trees, and KNN.

### 2. Systematic Sampling
- Systematic sampling is applied to the dataset, and machine learning models are trained and evaluated similarly.

### 3. Cluster Sampling
- KMeans clustering is used to perform cluster sampling.
- Three clusters are selected randomly, and the script evaluates the models on the sampled data.

### 4. Stratified Sampling
- Stratified sampling is conducted based on the target variable ('Class').
- The script calculates the required sample size using the formula for stratified sampling and evaluates model performance.

### 5. Bootstrap Sampling
- Bootstrap sampling is performed by resampling with replacement.
- The script generates 100 bootstrap samples and evaluates model performance.

## Evaluation
For each sampling technique, the script trains several machine learning models and reports the accuracy score for each model.

## Usage
1. **Data Loading**: The script loads the dataset from the provided URL.
2. **Data Preprocessing**: It normalizes the 'Amount' column and removes the 'Class' column.
3. **Sampling Techniques**: Various sampling techniques are applied to the dataset.
4. **Model Training and Evaluation**: Machine learning models are trained and evaluated on the sampled data.

## Requirements
- Python 3.x
- pandas
- scikit-learn
- imbalanced-learn

You can install the required dependencies using pip:

```bash
pip install pandas scikit-learn imbalanced-learn
