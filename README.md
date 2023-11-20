# WeatherPy and VacationPy: Analysis of Weather and Vacation Destinations

## Introduction
This repository contains the code and analysis for WeatherPy and VacationPy, two Python scripts designed for weather data retrieval and vacation destination identification based on specified weather conditions. The WeatherPy script generates random geographic coordinates, retrieves weather data from OpenWeatherMap, and analyzes the relationships between weather variables and latitude. The VacationPy script utilizes the weather data from WeatherPy to identify ideal vacation destinations and find nearby hotels using the Geoapify API.

## Background
### WeatherPy
WeatherPy is a Python script that leverages the OpenWeatherMap API to retrieve current weather data for randomly generated cities worldwide. The script uses the citipy library to determine the nearest city for given latitude and longitude coordinates. The retrieved data includes information such as maximum temperature, humidity, cloudiness, wind speed, and more.

### VacationPy
VacationPy is an extension of WeatherPy, focusing on identifying ideal vacation destinations based on specific weather conditions. The script filters cities from the WeatherPy output to find locations with favorable weather, considering criteria like temperature and wind speed. Additionally, VacationPy utilizes the Geoapify API to search for nearby hotels within a specified radius of the selected cities.

## Instructions

### WeatherPy
1. **Dependencies and Setup**: Ensure you have the required libraries installed. If not, run the following commands in your terminal or command prompt:
    ```bash
    pip install matplotlib pandas numpy requests scipy
    ```

2. **OpenWeatherMap API Key**: Obtain a free API key from [OpenWeatherMap](https://openweathermap.org/api) and replace `weather_api_key` in the `api_keys.py` file with your key.

3. **Run WeatherPy Script**: Execute the WeatherPy script by running the `WeatherPy.ipynb` Jupyter Notebook. This script generates random geographic coordinates, retrieves weather data from OpenWeatherMap, creates scatter plots, and performs linear regression on various weather variables.

4. **Output**: The script generates scatter plots and linear regression plots in the `output_data` folder and outputs weather data to `cities.csv`.

### VacationPy
1. **Dependencies and Setup**: Ensure you have the required libraries installed. If not, run the following commands in your terminal or command prompt:
    ```bash
    pip install hvplot pandas requests
    ```

2. **Geoapify API Key**: Obtain a free API key from [Geoapify](https://www.geoapify.com/) and replace `geoapify_key` in the `api_keys.py` file with your key.

3. **Run VacationPy Script**: Execute the VacationPy script by running the `VacationPy.ipynb` Jupyter Notebook. This script uses the weather data from WeatherPy to identify ideal vacation destinations and find nearby hotels using the Geoapify API.

4. **Output**: The script generates a map with vacation destinations marked, including information about hotels and weather conditions.

## Code References
- [WeatherPy Starter Code](#) - Initial code for generating random coordinates, retrieving weather data, and creating plots.
- [VacationPy Starter Code](#) - Initial code for identifying ideal vacation destinations, filtering data, and finding hotels using Geoapify API.

Feel free to explore the Jupyter Notebooks for a detailed walkthrough of the code and analysis. Enjoy your exploration of weather patterns and vacation destinations!
