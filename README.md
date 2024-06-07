# Air Quality Prediction Model

This repository contains a random forest model for predicting air quality based on AQI (Air Quality Index) values of various pollutants. The model is trained on a dataset sourced from Kaggle's Global Air Pollution Dataset.

The `app.py` file is used on Hugging Face for inference with Gradio. The program receives the location input by the user, converts it to coordinates, retrieves the AQI using Open Meteo, and prints the location's AQI along with the current air quality condition.

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

accuracy                         1.00      4607


- **Class Labels**:
  - 0: Good
  - 1: Moderate
  - 2: Unhealthy for Sensitive Groups
  - 3: Unhealthy
  - 4: Very Unhealthy
  - 5: Hazardous

## How to Use

1. **Clone the Repository**:
  ```bash
  git clone <repository-url>
  cd <repository-directory>
  ```

2. **Install Dependencies**:
  ```bash
  pip install -r requirements.txt
  ```

3. **Run the Application**:
  ```bash
  python app.py
  ```

## License

This project is licensed under the Apache 2.0 - see the [LICENSE](https://github.com/TLeonidas/TLeonidas-HCC-CSA-April24-Hackathon/blob/main/LICENSE) file for details.


