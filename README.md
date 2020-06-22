# World_Weather_Analysis

## Project Overview
Incoporate the following: 

	1. A weather description to the pop-up markers for customers so that they know what the weather is as they are traveling
	2. A notation in the search criteria to indicate if it is raining or snowing for customers who are making travel decisions in real-time
	3. A map that shows the directions for customers’ travel itinerary
	
## Resources
Data Source: OpenWeather, Google Maps
Software: Python 3.8.3, Jupyter Notebook

## Get the Weather Description and Amount of Precipitation for Each City
Below is a description of the process to collect Weather data for a list of latitude/longitude coordinates:
  * Generate a list of 1,500 random latitude/longitude coordinates using the Random library
  * Use the citipy module to take a latitude/longitude coordinate pair and find the closest city
  * Perform API calls to get real-time OpenWeatherMap weather data for each city
  * Data dumped to CSV file WeatherPy_database.csv
  
## Have Customers Narrow Their Travel Searches Based on Temperature and Precipitation
Below is a description of the process to allow user inputs for desired vacation spots matching using user inputs:
  * Imported and used the data from the 1,500 cities with real-time weather data
  * Allowed user input of min/max, rain, or snow
  * Looked up hotel(s) in the vicinity of a found town, and collected the hotel name using Google Search API
  * Overlayed real-time weather data, and closest hotel on Google Maps. 
![Weather Data Visualization for 1,500 random latitude/longitude coordinate pairs](https://github.com/n-toy/World_Weather_Analysis/blob/master/weather_data/WeatherPy_vacation_map.png)


## Create a Travel Itinerary with a Corresponding Map
Below is a description of the process to allow a user to create an itinerary using this module:
  * Enabled Google Cloud API for direction layer
  * Selected 4 cities that can be driven back and forth to (Same continent and area)
  * Overlayed current weather and hotels in current itinerary
![Custom Itinerary for identified cities](https://github.com/n-toy/World_Weather_Analysis/blob/master/weather_data/WeatherPy_travel_map_markers.PNG)
  
















