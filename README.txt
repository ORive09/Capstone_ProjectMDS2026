----------------
Project Overview
----------------

-Traffic accidents remain one of the leading causes of injury and death in the United States. Understanding the conditions that lead to severe crashes can help transportation agencies and planners improve roadway safety.
-This project uses machine learning techniques to predict the severity of traffic accidents using the publicly available U.S. Accidents dataset. By analyzing environmental, temporal, and roadway-related features, the goal is to identify patterns that contribute to severe crashes and evaluate the effectiveness of different predictive models.
-This project was completed as part of a Data Science Capstone Project.

----------
Objectives
----------

-The main goals of this project are:
-Predict accident severity using machine learning models
-Identify the most important factors contributing to severe crashes
-Compare multiple classification models
-Evaluate model performance using standard machine learning metrics

----------------
Project Workflow
----------------

1. Data Preprocessing
   - Load the dataset
   - Clean missing or inconsistent values
   - Select relevant features

2. Feature Engineering
   - Encode categorical variables
   - Prepare data for machine learning models

3. Model Training
   - Train multiple classification models:
     - Logistic Regression
     - Random Forest
     - XGBoost
     - Deep Neural Network
     - Stacking Ensemble

4. Model Evaluation
   - Evaluate models using standard metrics
   - Compare performance across models

5. Model improvement Experirments
   - Threshold Tuning
   - SMOTE on Losistic Regression
   - 2x scale_pos_weight on XGBoost

-----------
How to run:
-----------

The code in this repository expects the dataset to be located in a folder named:

/datasets

This folder must exist in the same directory where the code is being executed.

If the dataset is not placed inside the /datasets folder, the code may fail to locate the file and will produce a file path error.

Repository Structure

repo/

│
├── code files
│ (data cleaning, feature engineering, and model training scripts)
│
└── datasets/
        └── dataset file used for training and analysis

------------
Dependencies
------------

This project requires the following Python libraries:

- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost
- tensorflow
- imbalanced-learn


Authors

Osvaldo Rivera
Master's Student in Data Science

Nitin Nellisserry
Data Science Graduate Student
