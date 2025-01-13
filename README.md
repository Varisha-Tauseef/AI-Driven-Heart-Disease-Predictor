# AI-Driven Heart Disease Predictor
This project demonstrates the development of a machine learning model to predict whether an individual has heart disease based on clinical parameters. It leverages Python's powerful data science and machine learning libraries.

Problem Definition
Can we predict the presence of heart disease in a patient using their medical data?

Dataset
The dataset used is the Cleveland Heart Disease dataset from the UCI Machine Learning Repository:

## Original Source
Alternative Source on Kaggle

Project Goals
Achieve at least 95% accuracy for heart disease prediction during the proof of concept.
Identify the most important clinical features contributing to predictions.

## Steps Followed
Exploratory Data Analysis (EDA):
  * Visualized distributions and correlations.
  * Analyzed key relationships (e.g., gender vs. target).

Preprocessing:
  * Checked for missing values (none found in this dataset).
  * Split data into training and testing sets.

Baseline Model Comparison:
  * Tested multiple models:
    * Logistic Regression
    * K-Nearest Neighbors (KNN)
    * Random Forest
    * Decision Tree
  * Evaluated models using accuracy, precision, recall, and F1 score.

Hyperparameter Tuning:
  * Used RandomizedSearchCV to tune Logistic Regression, Random Forest, and Decision Tree.

Evaluation:
Plotted ROC-AUC curves.
Visualized the confusion matrix.
Generated cross-validated classification metrics.
Feature Importance:
Determined key predictors using coefficients from Logistic Regression.
Key Findings
The Logistic Regression model performed the best after tuning.
Most important features: Sex, Cp, Oldpeak, Ca, and Thal.
The KNN model underperformed and was discarded.
Technologies Used
Python Libraries:
Data Manipulation: pandas, numpy
Visualization: matplotlib, seaborn
Machine Learning: scikit-learn
How to Run
Clone this repository or download the .ipynb file.
Upload the notebook to Google Colab.
Download the dataset and adjust file paths as needed.
Future Improvements
Experiment with other advanced algorithms like XGBoost or LightGBM.
Perform more feature engineering for better results.
Address potential class imbalances if larger datasets are used.
Acknowledgements
This project is inspired by the publicly available Cleveland Heart Disease dataset. Special thanks to the UCI Machine Learning Repository and Kaggle.
