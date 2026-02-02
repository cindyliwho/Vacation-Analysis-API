# Weather & Vacation Analysis (APIs, Data Visualization, Geospatial Mapping)

## Overview
This project explores the relationship between **latitude and weather patterns** and uses real-time weather data to identify **ideal vacation destinations**. It combines API data retrieval, exploratory data analysis, visualization, and geospatial mapping.

The project is split into two parts:
1. **WeatherPy** – Analyze global weather trends using OpenWeather API data  
2. **VacationPy** – Identify and map potential vacation cities based on preferred weather conditions

---

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **SciPy**
- **OpenWeather API**
- **Geoapify API**
- **Jupyter Notebook**

Key libraries:
- `requests`
- `matplotlib`
- `scipy.stats`
- `hvplot`
- `geoviews`

---
## Part 1: WeatherPy – Global Weather Analysis

### What It Does
- Generates a list of random cities using latitude and longitude coordinates
- Fetches current weather data from the **OpenWeather API**
- Builds a structured DataFrame with:
  - Latitude & longitude
  - Temperature
  - Humidity
  - Cloudiness
  - Wind speed

### Analysis & Visualizations
Scatter plots are created to examine relationships between latitude and:
- Temperature
- Humidity
- Cloudiness
- Wind speed

Linear regression is performed separately for:
- **Northern Hemisphere**
- **Southern Hemisphere**

This highlights how latitude influences temperature differently across hemispheres.

---

## Part 2: VacationPy – Vacation Destination Finder

### What It Does
- Filters cities based on **ideal weather conditions**, such as:
  - Moderate temperatures
  - Low wind speed
  - Minimal cloud cover
- Uses the **Geoapify API** to locate nearby hotels for each qualifying city
- Plots the results on an interactive **map visualization**

### Output
- A map displaying potential vacation destinations
- Markers include:
  - City name
  - Country
  - Nearby hotel name
  - Weather conditions
