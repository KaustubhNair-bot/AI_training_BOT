# Tree-Based Models - Adult Income Classification

## Overview
This notebook demonstrates the implementation and comparison of tree-based machine learning models for predicting adult income levels (>50K or ≤50K) using the UCI Adult dataset.

## Dataset
- **Source**: UCI Adult Income Dataset
- **Features**: Demographics, education, occupation, and employment information
- **Target**: Binary classification of income (>50K / ≤50K)

## Models Implemented
1. **Decision Tree Classifier**
   - Baseline tree-based model
   - Easy to interpret and visualize

2. **Random Forest Classifier**
   - Ensemble method with multiple decision trees
   - Reduces overfitting through bagging

3. **Gradient Boosting Classifier**
   - Sequential ensemble method
   - Optimizes for better predictive performance

## Key Steps
1. **Data Preprocessing**
   - Handling missing values
   - Encoding categorical variables
   - Feature scaling

2. **Model Training**
   - Training baseline models
   - Cross-validation for performance estimation

3. **Hyperparameter Tuning**
   - GridSearchCV for optimal parameter selection
   - Systematic exploration of parameter space

4. **Model Evaluation**
   - Accuracy, precision, recall metrics
   - Confusion matrix analysis
   - ROC curves and AUC scores

5. **Feature Importance Analysis**
   - Identifying key predictors
   - Visualizing feature contributions

## Results
- Comparison of model performance metrics
- Top features: capital-gain, relationship, education-num, marital-status, age
- Insights into income prediction factors

## Requirements
- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

## Usage
Run the notebook cells sequentially to:
- Load and explore the dataset
- Train and compare different models
- Tune hyperparameters
- Analyze feature importance
- Generate visualizations

## Author
Kaustubh Nair
