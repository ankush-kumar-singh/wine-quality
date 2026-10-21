
# Wine Quality Analysis 🍷

## Project Overview

What makes a wine good? In this project, I explored the Wine Quality Dataset to understand how different physicochemical properties are related to wine quality ratings.

The main goal was to use Exploratory Data Analysis (EDA) to identify patterns in the data and understand how these insights can guide machine learning model selection.

## Objectives

- Explore the dataset and understand its features.
- Analyze relationships between chemical properties and wine quality.
- Identify patterns using statistical analysis and visualizations.
- Understand class distribution and feature scaling.
- Explore suitable machine learning approaches for predicting wine quality.

## Dataset

The Wine Quality Dataset contains physicochemical measurements of wine samples along with quality ratings assigned by sensory evaluations.

Some important features include:

- `alcohol`
- `volatile acidity`
- `citric acid`
- `residual sugar`
- `chlorides`
- `pH`
- `density`
- `total sulfur dioxide`
- `sulphates`
- `quality` (target variable)

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Key Findings

### 1. Alcohol Content and Quality

Alcohol content showed a positive correlation with wine quality in my analysis (approximately +0.48).

Higher-rated wines generally had higher alcohol content, making alcohol an interesting feature to investigate during model development.

### 2. Volatile Acidity and Quality

Volatile acidity showed a negative correlation with quality (approximately -0.40).

Higher volatile acidity can contribute to unpleasant, vinegar-like flavours, which may influence sensory evaluations.

### 3. Distribution of Quality Ratings

Most wine samples were concentrated around quality ratings of 5 and 6, while extreme ratings were less common.

This uneven distribution is important to consider when selecting evaluation metrics and developing classification models.

### 4. Differences in Feature Scales

The dataset contains features with very different numerical ranges. For example, pH values are much smaller in magnitude than total sulfur dioxide values.

Feature scaling may be useful for algorithms such as K-Nearest Neighbors (KNN) and Support Vector Machines (SVM).

## Machine Learning Approach

Model selection depends on the prediction objective and the patterns present in the dataset.

### Regression

If the objective is to predict a numerical wine quality score, possible models include:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

### Classification

If the objective is to predict a discrete quality rating, possible models include:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier

These are candidate models, not a claim that every model has already been trained or evaluated.

## Model Evaluation

For regression, suitable evaluation metrics include:

- **MAE:** Measures the average absolute prediction error.
- **RMSE:** Gives more weight to larger prediction errors.
- **R² Score:** Measures the proportion of target variance explained by the model.

For classification, useful metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The final model should be selected based on validation performance and the project's objective, rather than accuracy alone.

## Project Workflow

1. Load and inspect the dataset.
2. Check data types, missing values, and duplicates.
3. Perform Exploratory Data Analysis.
4. Visualize feature distributions and correlations.
5. Identify potential relationships with wine quality.
6. Define the prediction objective: regression or classification.
7. Split the data into training and testing sets.
8. Apply preprocessing where required.
9. Train and compare suitable baseline models.
10. Evaluate the models and interpret the results.

## Key Learning

This project helped me understand how EDA can guide machine learning decisions.

Rather than choosing an algorithm randomly, the aim is to understand the data, establish a baseline, compare suitable models, and select an approach supported by evaluation results.

## Future Improvements

- Perform deeper statistical analysis.
- Compare regression and classification approaches.
- Experiment with feature engineering.
- Evaluate feature importance.
- Tune model hyperparameters.
- Investigate ordinal classification methods for ordered quality ratings.

## Conclusion

The Wine Quality Analysis project is an exploration of how data analysis can reveal useful patterns in physicochemical properties and help guide predictive modeling.

It is an ongoing learning exercise focused on understanding the data and making evidence-based decisions throughout the machine learning workflow.
