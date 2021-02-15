# World_Weather_Analysis
## Overview
We created a beta program to provide real-time suggestions to our clients for hotels within 5,000 meters of a desired-temperature location. Upon finishing that project, beta testers recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data, and provide input statements to filter the data for their weather preferences. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary, and we'll provide a recommended hotel for each city along their route.

## Development
### 1. Retrieve Weather Data
We generated a set of 2,000 random latitudes and longitudes, retrieved the nearest city, and performed an API call with the OpenWeatherMap to retrieve the current weather description for each city, and stored all of the information into a DataFrame.

### 2. Create a Customer Travel Destinations Map
We then created and used input statements to retrieve customer weather preferences; in this case, between 75-90 degrees. We then used those preferences to identify potential travel destinations and nearby hotels, showing those destinations on a marker layer map with pop-up markers.
![Ideal Weather Locations](https://github.com/andeevosters/World_Weather_Analysis/blob/main/Vacation_Search/Vacation_search.png)


### 3. Create a Travel Itinerary Map 
Lastly, we used the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations, with a marker layer map with a pop-up marker for each city on the itinerary for optimal travel experience.
![Brazil Travel Itinerary](https://github.com/andeevosters/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
![Brazil Hotel Recommendations](https://github.com/andeevosters/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

## Resources
Jupyter Notebook 6.1.4
Pandas Library 
CityPi 
Python Requests Library 2.24 
OpenWeatherMap API
Google Map Platform API
JSON Traversals
