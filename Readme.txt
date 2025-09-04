Feature Selection Methods and High Accuracy ML Model In this task, I worked on the Breast Cancer Dataset (from Kaggle) to apply three feature selection techniques and then train a Machine Learning model that achieves more than 90% accuracy.

The goal of this project is to: Understand and apply different feature selection methods. Compare which features are most important for predicting breast-cancer. Build a classification model that can accurately predict whether a tumor is benign or malignant.

#Dataset Used Source: Breast Cancer Dataset on Kaggle Rows: 570 Columns: 32 The target column is 2, Benign&Malignant.

Data Cleaning
Before modeling, I cleaned the dataset in MSExcel: Checked for missing/blank values. Replaced invalid 0 values with the median of the respective column. Ensured that all columns had the correct numeric data type.

#Feature Selection Methods I applied three feature selection techniques: #Filter Method (Correlation / Chi-Square Test) Removed less informative features. Kept features that showed higher correlation with the target variable. #Wrapper Method (Recursive Feature Elimination – RFE) Used Logistic Regression as the base model. Iteratively removed weaker features until the most important ones were left. #Embedded Method (Feature Importance from Random Forest)

##Trained a Random Forest Classifier. Ranked features by importance (Gini Index). After comparing results, the dataset was reduced to a smaller set of important features, improving accuracy and reducing overfitting.

##Machine Learning Model Model chosen: Random Forest Classifier Reason: Works well with tabular data, handles noisy features, and provides feature importance scores. Random state was fixed (RANDOM_STATE = 42) for reproducibility. ##Results Accuracy of Random Forest Classifier (after feature selection): 94% Model successfully crossed the 90% accuracy requirement.

##Steps to repeat the model Download the dataset from Kaggle and clean it in Excel (fill missing/0 values with median). Open the Jupyter Notebook. Run the cells step by step: Data Loading (import the cleaned dataset). Feature Selection Methods (Filter, Wrapper, Embedded). Model Training (Random Forest). Evaluation (Accuracy Score, Confusion Matrix).

##Requirements To run this project, install: numpy
pandas
matplotlib
seaborn

scikit-learn
