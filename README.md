# Realtime Weather Monitoring 


## Project Overview
The **Realtime Weather Monitoring App** is designed to provide users with real-time weather data for various cities, including current weather conditions, temperature, and forecasts. It features an intuitive interface that allows users to set temperature thresholds for alerts and visualize data through graphs.

## Features
- **Real-time Weather Data**: Fetch current weather conditions from the Weatherstack API.
- **Daily Summaries**: Display daily weather aggregates such as average, maximum, and minimum temperatures.
- **Temperature Unit Toggle**: Users can switch between Celsius and Fahrenheit for temperature readings.
- **Forecast Modal**: Provides detailed forecast data for each city.
- **Temperature Alert Thresholds**: Users can set customizable thresholds for temperature alerts.
- **Responsive Charts**: Visualize temperature changes throughout the day using Chart.js.

## Technologies Used
- **Backend**: Python with Flask for the server-side application.
- **Database**: MongoDB for storing weather data and user configurations.
- **Frontend**: HTML, CSS, and JavaScript (with Chart.js) for the user interface.
- **API Integration**: Weatherstack API for fetching real-time weather data.

## Project Setup
To set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd weather-monitoring-app
   ```

2. **Create a Virtual Environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up MongoDB**: Make sure you have MongoDB running and configure the connection in the `database/__init__.py` file.

5. **Run the Flask Application**:
   ```bash
   python app.py
   ```

6. **Access the Application**: Open your web browser and go to `http://127.0.0.1:5000` to access the application.

## Design Choices

- **Modular Architecture**: The application is organized into modules (weather, database, etc.) for better maintainability and separation of concerns.
- **RESTful API Design**: The backend exposes RESTful endpoints for retrieving weather data and settings, promoting a clear and intuitive interface.
- **Responsive Design**: The frontend is designed to be responsive, ensuring usability across different devices and screen sizes.
