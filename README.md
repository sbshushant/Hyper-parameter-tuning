# Hyper-parameter-tuning

Introduction
This project focuses on hyper-parameter tuning for machine learning models to improve their performance. The dataset used is the Titanic dataset, which contains information about passengers on the Titanic and their survival status.

Table of Contents
Introduction About the Dataset Data Preprocessing Feature Engineering Chi-Square Test for Feature Selection Feature Scaling Modeling Hyper-Parameter Tuning Model Performance Evaluation Conclusion

About the Dataset
The Titanic dataset includes the following features:

Survived: Survival status (0 = No, 1 = Yes) Pclass: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) Sex: Gender of the passenger Age: Age of the passenger SibSp: Number of siblings/spouses aboard the Titanic Parch: Number of parents/children aboard the Titanic Fare: Fare paid for the ticket Embarked: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

Data Preprocessing
Loading Data:
The dataset was loaded into a pandas DataFrame for inspection.

Handling Missing Values:
Dropped rows with missing values.

Encoding Categorical Variables:
Converted categorical variables (Sex and Embarked) into numerical format using label encoding.

Feature Engineering
Chi-Square Test for Feature Selection:
Applied the Chi-Square test to select the most important categorical features. Selected features: Pclass, Parch, sex_encoded, and embarked_enc.

Feature Scaling:
Standardized numerical features (Age and Fare) using StandardScaler.

Modeling
Data Splitting:
Split the dataset into training and testing sets using an 80-20 split.

Hyper-Parameter Tuning:
Used GridSearchCV to perform hyper-parameter tuning on a Decision Tree classifier. Tuned parameters: criterion, max_depth, and min_samples_leaf. Selected the best model based on grid search results. Model Performance Evaluation

Training the Final Model:
Trained the final Decision Tree model with the best hyper-parameters.

Evaluation:
Evaluated the model's performance using accuracy score and classification report.

Conclusion
The analysis demonstrated the application of hyper-parameter tuning to improve the performance of a Decision Tree classifier on the Titanic dataset. Key findings include:

Hyper-parameter tuning significantly improved the model's accuracy. The selected features and scaled numerical values contributed to better model performance. These insights highlight the importance of hyper-parameter tuning and feature engineering in building efficient and effective machine learning models.
