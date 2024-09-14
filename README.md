# Customer Churn Prediction Using Machine Learning and Neural Networks

## Overview
This project focuses on predicting customer churn using a telecom dataset. A major part of the project involved extensive data preprocessing, including data cleaning, feature selection, and transformation to ensure the models performed optimally.

## Data Preprocessing Steps
**1. Data Cleaning**
- Converted the 'HandsetPrice' column from an object to numeric data type to handle it properly in the model.
- Imputed missing values using the KNN Imputer for continuous variables, ensuring that missing data did not skew the model results.
- Dropped unnecessary columns such as 'CustomerID' and weakly correlated features after performing correlation analysis.

**2. Encoding Categorical Variables**
- Used `LabelEncoder` to transform categorical variables into numerical format to make the data suitable for machine learning models.
  
**3. Handling Imbalanced Data**
- The target variable, `Churn`, had class imbalance, so the NearMiss undersampling technique was applied to balance the dataset and avoid model bias.

**4. Feature Scaling**
- Applied `StandardScaler` to normalize the features, improving model convergence and performance.

## Modeling
After preprocessing the data, two machine learning models were implemented and optimized:
- **Artificial Neural Network (ANN)** using Keras, with Early Stopping and ModelCheckpoint callbacks for optimization.
- **Random Forest Classifier** with hyperparameter tuning using RandomizedSearchCV.

## Key Preprocessing Techniques:
- **KNN Imputation**: Efficiently filled missing values based on the nearest neighbors.
- **Label Encoding**: Converted all categorical variables to a numeric format.
- **Correlation Matrix Analysis**: Dropped features with weak correlations to the target variable.
- **Undersampling with NearMiss**: Balanced the target class distribution.
- **Standardization**: Scaled features to standardize the input data.

## Technologies Used
- **Python**: pandas, numpy, scikit-learn, keras
- **Data Preprocessing**: KNN Imputer, LabelEncoder, StandardScaler
- **Machine Learning Models**: ANN, Random Forest
- **Model Evaluation**: Accuracy, Precision, Recall, F1-score, ROC-AUC
- **Hyperparameter Tuning**: RandomizedSearchCV

## Conclusion
This project demonstrates the importance of thorough data preprocessing in machine learning pipelines. By using advanced preprocessing techniques, the final models were able to achieve high performance in predicting customer churn.

