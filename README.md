# Air Quality Prediction Model

This repository contains a random forest model for predicting air quality based on AQI (Air Quality Index) values of various pollutants. The model is trained on a dataset sourced from Kaggle's Global Air Pollution Dataset.

## Dataset

- **Dataset Name**: Global Air Pollution Dataset
- **Dataset Source**: [Kaggle](https://www.kaggle.com/datasets/hasibalmuzdadid/global-air-pollution-dataset/)
- **Dataset Size**: 23,463 rows, 12 columns

## Model Performance

- **Model Name**: hackathonrf.joblib
- **Accuracy**: 99.91%
- **Classification Report**:

          precision    recall  f1-score   support

       0       1.00      1.00      1.00      1926
       1       1.00      0.91      0.95        45
       2       1.00      1.00      1.00      1841
       3       1.00      1.00      1.00       405
       4       1.00      1.00      1.00       333
       5       0.93      1.00      0.97        57

accuracy                           1.00      4607
