# World Weather Analysis

## Overview

This analysis offers insights to travelers who want to book a trip based on weather patterns. Users can provide filter criteria based on temparature and get suggestions to create a travel itinerary. This analysis uses the Google gmaps API to plot heatmap based on temperatures, and markers to indicate hotel locations around selected destinations. There are three folders here that offer different levels of analysis: weather database, vacation search, and vacation itinerary.

### Weather Database

This folder uses Open Weather Map API to pull weather information on selected cities around the world. That information consists of:

1. Maximum Temperature
2. Cloudiness
3. Wind Speed
4. Humidity
5. Current Weather Description

The temperature information is used to plot a heatmap while the remaining information is used to populate markers.

### Vacation Search

This module uses the data curated in the weather database and uses Google Maps API to plot different travel destinations with a hotel at each location. For example, the image below shows the locations of all the places in the database that have an daily maximum temperature between 75 and 88 degrees farinheit.

![weatherpy_vacation_map](https://github.com/tarini-mi7/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### Vacation Itinerary

This module takes a search criteria and uses Google Maps directions API to create a vacation itinerary. For example, the image below shows a 4 stop itinerary across the continental United States.

![WeatherPy_travel_map](https://github.com/tarini-mi7/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

Also, as with the vacation search folder, there is a hotel at each location.

![WeatherPy_travel_map_markers](https://github.com/tarini-mi7/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)

### Correlation of weather attributes with latitude

I have included valuable linear regression models looking at the correlation between different weather attributes and latitude in the WeatherPy.ipynb notebook.
