# World_Weather_Analysis
## Project Overview
Compiling weather data and using it to help clients select travel destinations. Steps included:
  - Genereating random latitude and longitude coordinates for world cities.
  - Retrieving weather data using the OpenWeatherMap API.
  - Cleaning the data and placing it into a pandas DataFrame.
  - Plotting weather data using matplotlib.
  - Determining correlations between latitude and various weather patterns using linear regressions.
  - Using Google API to create heatmaps of certain weather conditions, as well as pop-up markers showing hotels and weather information     for destinations meeting certain criteria.

## Challenge
The challenge for this module involved adding features to the already created maps and DataFrames. These new features include:
  - Adding a weather description to the pop-up markers so customers know what the weather is when they are travelling.
  - A notation in the search criteria to indicate if it is raining or snowing for customers who are making travel decisions in real-         time.
  - A map that shows the directions for customers' travel itinerary.
  
## Challenge Overview
The steps for each feature are as follows.
  - Weather description: For the weather description pop-up, I performed my work in the Weather_Database.ipynb file. In this file, I      generated a list of random latitude and longitude coordinates. I then used the citipy dependency to locate the closest city for each coordinate pair. I then used the OpenWeatherMap API to extract the weather data for each city. I then compiled this information into a    pandas DataFrame, which is saved in the "data" folder as "WeatherPy_database.csv".
  - Notation in the search criteria to indicate if it is raining or snowing: For the search notation portion of this project, I performed my work in the Vacation_Search.ipynb file. I first imported hte "WeatherPy_database.csv" DataFrame. I then added several input() functions to allow the customer to add their desired weather criteria--temperature, rain, and snow--for their vacation. I then used an if-elif-else statement to create a new DataFrame with destinations that fit the client's criteria. I then used the Google Maps API to locate the nearest hotels in each of the cities meeting the client's weather criteria. I then exported this DataFrame to the "WeatherPy_vacation.csv" file in the "data" folder. I then used the Google Maps API to createa map of the selected destinations. I then saved this image as "Weather_Py_vacation_map.png" in the "image" folder.
  - Map that shows the directions for the customers' travel itinerary: For the map showing the travel itinerary, I first imported the "WeatherPy_vacation.csv" file as a pandas DataFrame. I then selected four locations that were all within the same continent for the client's travel itinerary. I then used the Google Maps API to create a map with a marker designating the route for the clients to take. I then saved this map as "WeatherPy_travel_map.PNG" in the "image" folder. I then created a map with markers for each of the selected cities in the itinerary. I saved this map as "WeatherPy_travel_map_markers.png" in the "image" folder.
  
  
