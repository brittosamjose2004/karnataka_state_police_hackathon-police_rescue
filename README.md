# Crime Prediction and Forecasting Web Application

## Overview
This web application is developed for the KSP Hackathon, aimed at predicting and forecasting crime trends in various districts. The application utilizes machine learning models to predict the likelihood of crimes based on various inputs and provides visualizations for crime data. 

## Installation and Setup
To run the application, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Install required libraries**:
    Make sure you have `pip` installed, then run:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the application**:
    ```bash
    python app.py
    ```

4. **Access the application**:
    Open your browser and go to `http://0.0.0.0:5000/`.

5. **Login credentials**:
    - **Username**: `admin`
    - **Password**: `admin123`

## File Structure
- `app.py`: Main application script containing all routes and logic.
- `templates/`: Directory containing HTML templates for rendering web pages.
- `static/`: Directory for static files such as CSS and JavaScript.
- `models/`: Directory containing pre-trained models and data files.
- `requirements.txt`: File containing a list of Python dependencies.

## Functionality
### Web Pages
- **Login Page (`/`)**: User login with predefined credentials.
- **Index Page (`/index`)**: Dashboard overview after logging in.
- **District Pages**: Separate pages for each district, e.g., `/Bagalkot`, `/Bengaluru_City`.
- **Crime Distribution (`/crime_distribution_district`)**: Visualize crime distribution across districts.
- **Accused Age Distribution (`/Distribution_of_Accused_Ages`)**: Visualize age distribution of accused individuals.
- **Forecast Crime (`/forecast_crime`)**: Predict and forecast future crime trends.
- **Recent Crimes (`/Recent_Crimes`)**: Display recent crime data.
- **Heat Map (`/heat-map`)**: Heat map visualization of crime incidents.
- **Crime Marker (`/crime-marker`)**: Marker map visualization for crime locations.
- **Cluster Analysis (`/cluster`)**: Display clustering analysis of crime data.
- **Crime Prediction (`/predict`)**: Predict the likelihood of crime based on user inputs.
- **Future Crime Forecast (`/future-crime-forecast`)**: Forecast future crime trends using ARIMA model.

### Models and Data
- **Logistic Regression Model** (`logistic_regression_model.pkl`): Used for predicting crime likelihood.
- **Deployment Plan** (`deployment_plan.pkl`): Contains cluster information and deployment strategies.
- **Crime Data** (`predicted_crime.pkl`): Contains predicted crime data for future years.
- **ARIMA Model** (`arima_model.pkl`): Time series model for forecasting future crime trends.

## Usage
### Predict Crime
1. Navigate to `/predict`.
2. Enter the required details: age, sex, present city, and present state.
3. Submit the form to get the prediction result.

### Get Closest Cluster
1. Navigate to `/get-closest-cluster`.
2. Provide latitude and longitude to get the closest crime cluster details.

### Crime Prediction for Future Years
1. Navigate to `/crime-prediction`.
2. Select the year (2025 or 2026) to view predicted crime trends for each month.

### Future Crime Forecast
1. Navigate to `/future-crime-forecast`.
2. Enter the start date and the number of future steps to forecast.
3. View the forecasted crime trend plot and data.

## Prototype Link
For a live demo of the application, visit the prototype link: 
[Crime Prediction App](https://super-umbrella-pj7j4xpp49v9c6g4g-5000.app.github.dev/)

## Notes
- Ensure that all the necessary models and data files are present in the `models/` directory before running the application.
- The application runs on Flask and requires the necessary dependencies listed in `requirements.txt`.

## Contact
For any issues or inquiries, please contact [brittosamjosej@gmail.com].
