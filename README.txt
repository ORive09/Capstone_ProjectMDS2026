----------------
Project Overview
----------------

This project predicts high-severity traffic accidents using machine learning
models trained on the US Accidents dataset, comparing Logistic Regression,
Random Forest, XGBoost, a Deep Neural Network, and a stacking ensemble.

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

--------------------
Repository Structure
--------------------

repo/
├── README.txt
├── notebooks/
|        └──(01_data_preprocessing.ipynb, 02_model_training.ipynb, 03_model_evaluation.ipynb)
|        └── artifacts/
|                 └── .joblib files used to store intermediate objects (models, results, etc.)
|                       so they can be reused by later notebooks. These files are ignored by git
|                       and will be generated when the notebooks are executed.
└── datasets/
        └── US_Accidents_March23.csv
        └── cleaned_accidents.csv(after running 01_data_preprocessing, this will be saved off in here)
        └── .gitkeep file just to track the folder, since it is currently empty.

-----------
How to run:
-----------

1. Ensure the dataset is in the correct directory, can be found here: https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents/data

repo/
└── datasets/
    └── US_Accidents_March23.csv
         |  - Note: The dataset is not included in this repository due to its large size.
         |     Download it from Kaggle and place it in the `/datasets` directory.
         └── cleaned_accidents.csv (generated after running 01_data_preprocessing.ipynb)
         └── .gitkeep file just to track the folder, since it is currently empty.
The code in this repository expects the dataset to be located in a folder named:
 -/datasets

If the dataset is not placed inside the /datasets folder, the code will fail to locate the file and will produce a file path error.

2. Run notebooks **in the following order**: 
      - 01_data_preprocessing.ipynb
         -Loads the raw accident dataset
         -Cleans and preprocesses the data
         -Performs feature engineering and dataset preparation
         -saves artifacts for notebook 2 to use
      - 02_model_training.ipynb
         - Trains machine learning models including:
            - Logistic Regression
            - Random Forest
            - XGBoost
            - Deep Neural Network
            - Stacking Ensemble
      - 03_model_evaluation.ipynb
         - Compares model performance
         - Generates evaluation metrics and visualizations
         - Analyzes feature importance and model improvements

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
- pathlib
- joblib


Authors

Osvaldo Rivera
Master's Student in Data Science

Nitin Nellisserry
Data Science Graduate Student
