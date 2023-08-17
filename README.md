# Predicting a DND Character Race using Machine Learning Classifier Models

This project involves using Scikit-learn and Pandas to create a machine learning model for a multiple classification problem aimed at predicting the race of a Dungeons & Dragons character based on their ability scores and general features.

## Problem Definition

Given a set of character ability scores and general features, the goal is to predict the race of the character.

## Data

The original dataset was obtained from Kaggle, provided by Andrew Abeles: [DND Character Stats Dataset](https://www.kaggle.com/datasets/andrewabeles/dnd-stats).

## Evaluation

**Aim**
To achieve a classification accuracy that matches or exceeds 51.8%, the model accuracy from Andrew Abeles's project (KNN tuned model).

## Features

The dataset contains 10,000 samples, each with 9 input features and 1 target feature.

**Input Features:**
- Height (inches)
- Weight (lbs)
- Speed (ft.)
- Strength
- Dexterity
- Constitution
- Wisdom
- Intelligence
- Charisma

**Target Variable:**
- Race (dragonborn, dwarf, elf, gnome, half-elf, half-orc, halfling, human, tiefling)

## Modelling

1. Data Preprocessing: The dataset was loaded into a Pandas DataFrame. There were no missing values.

2. Exploratory Data Analysis (EDA): Data visualization was performed to understand feature correlations and distributions.

3. Model Selection: Several machine learning models were evaluated, including Support Vector Classifier (SVC), K-Nearest Neighbors (KNN), Random Forest Classifier, AdaBoost Classifier, and Logistic Regression.

4. Model Evaluation: Initial model scores were computed and compared. Random Forest, Logistic Regression and SVC performed similarly.

5. Hyperparameter Tuning:
   - Random Forest: Randomized and Grid Search CV were used to optimize hyperparameters.
   - Logistic Regression: Randomized and Grid Search CV were used to optimize hyperparameters.

6. Model Comparison: The best Random Forest model was selected based on the hyperparameters obtained from Grid Search CV.

7. Cross-Validation: The final Random Forest model's performance was evaluated using cross-validation for accuracy, precision, recall, and F1-score.

## Conclusion

The project involved building and tuning a machine learning model to predict the race of a DND character based on their ability scores and general features. The Random Forest model achieved an accuracy of around 67.25% after hyperparameter tuning and cross-validation. This model can serve as a baseline for predicting character races and can be further improved with more data and feature engineering.
