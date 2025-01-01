# A Comparative Study of Machine Learning Algorithms for Veterinary and Speculative Scenarios

## Overview
This project investigates the application of machine learning models to two distinct prediction tasks:
1. Forecasting health outcomes in horses
2. Predicting passenger transportation in the hypothetical Spaceship Titanic scenario

The study implements and compares four primary machine learning algorithms to analyze these diverse datasets, providing insights into model performance and optimization techniques.

## Key Features
- Implementation of multiple machine learning algorithms:
  - CatBoost
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Naive Bayes
- Comprehensive data preprocessing pipeline
- Hyperparameter tuning optimization
- Ensemble methods implementation
- Cross-validation techniques for robust evaluation

## Key Steps

### Data Preprocessing
1. Data cleaning and missing value handling
   - Numeric columns: Mean value imputation
   - Non-numeric columns: Mode value imputation
2. Label encoding for categorical variables
3. Feature engineering and dimensionality reduction
4. Dataset augmentation using random value generation within attribute ranges

### Model Implementation
1. Dataset splitting into training and validation sets
2. 10-fold Cross Validation implementation
3. Stratified sampling for balanced class distributions
4. Model training with hyperparameter optimization
5. Performance evaluation using F1-Score metric

## Results (F1-Score)

### Spaceship Titanic Dataset Performance
- CatBoost: 80.64
- KNN: 79.23
- SVM: 75.55
- Naive Bayes: 76.6

### Horse Health Dataset Performance
- CatBoost: 78.65
- KNN: 67.07
- SVM: 46.95
- Naive Bayes: 39.63

CatBoost consistently demonstrated the most robust performance across both datasets, achieving the highest scores in all scenarios.

## Project Limitations
1. Dataset Size
   - Initial dataset size was insufficient
   - Required artificial data augmentation
   - May impact model generalization

2. Feature Independence
   - Naive Bayes assumption of feature independence may not hold true
   - Could affect model accuracy in real-world scenarios

3. Computational Resources
   - SVM implementation may be computationally intensive
   - Could limit scalability for larger datasets

4. Model Complexity
   - Advanced models like CatBoost may require more tuning
   - Could increase implementation complexity
