# Air Quality Prediction Model

This repository contains a random forest model for predicting air quality based on AQI (Air Quality Index) values of various pollutants. The model is trained on a dataset sourced from Kaggle's Global Air Pollution Dataset.

## How It Works

The `app.py` file receives a location input from the user, converts it to coordinates, retrieves the AQI using OpenWeatherMap, and prints the location's AQI along with the current air quality condition.

## Instructions

### Setup

1. **Create an OpenWeather Account**:
    - Create an account on [OpenWeather](https://home.openweathermap.org/users/sign_up).
    - Obtain your API key from OpenWeather.

2. **Clone the Repository**:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set Up OpenWeather API Key**:
    - **On Unix-based systems (Linux, macOS)**:
        ```bash
        export OPENWEATHER_API_KEY='your_api_key_here'
        ```
    - **On Windows (Command Prompt)**:
        ```cmd
        set OPENWEATHER_API_KEY=your_api_key_here
        ```
    - **On Windows (PowerShell)**:
        ```powershell
        $env:OPENWEATHER_API_KEY = "your_api_key_here"
        ```

5. **Run the Application**:
    ```bash
    python app.py
    ```

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

            accuracy               1.00      4607



- **Class Labels**:
  - 0: Good
  - 1: Moderate
  - 2: Unhealthy for Sensitive Groups
  - 3: Unhealthy
  - 4: Very Unhealthy
  - 5: Hazardous

## USA Air Quality Index Levels

Below is a description of USA Air Quality Index levels:

| AQI        | Level of Health Concern               | Color  |
|------------|---------------------------------------|--------|
| 0 to 50    | Good                                  | Green  |
| 51 to 100  | Moderate                              | Yellow |
| 101 to 150 | Unhealthy for Sensitive Groups        | Orange |
| 151 to 200 | Unhealthy                             | Red    |
| 201 to 300 | Very Unhealthy                        | Purple |
| 301 to 500 | Hazardous                             | Maroon |
| 501 to 1000| Very Hazardous                        | Brown  |

## License

This project is licensed under the Apache 2.0 - see the [LICENSE](https://github.com/TLeonidas/TLeonidas-HCC-CSA-April24-Hackathon/blob/main/LICENSE) file for details.


