# World_Weather_Analysis

## Overview of the analysis: 

The project has the goal to help PlanMyTrip collect and present data that shows the relation between latitude and a variety of weather parameters for over 500 cities around the world. The analysis will help clients to better plan the trips by filtering and showing targeted results. 

“Background: Jack loves the PlanMyTrip app. Beta testers love it too. And, as with any new product, they’ve recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data you’ve already retrieved in this module. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map.”

### Software:

Pandas, Jupyter Notebook, Python (Numpy), CitiPy, OpenWeatherMap API  and JavaScript Object Notation (JSON Traversals). 

### Outline of the analysis

Basic Project Plan

Here's an outline of project plan:
- Task: Collect and analyze weather data across cities worldwide.
- Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
- Method: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This  process will entail collecting, analyzing, and visualizing the data.

The analysis of the data was split into three main parts, or stages.
  1. Collect the Data
    1. Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
    2. Use the citipy module to list the nearest city to the latitudes and longitudes
    3. Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
    4. Parse the JSON data from the API request.
    5. Collect the following data from the JSON file and add it to a DataFrame:
        - City, country, and date
        - Latitude and longitude
        - Maximum temperature
        - Humidity
        - Cloudiness
        - Wind speed
  2. Exploratory Analysis with Visualization
    1. Create scatter plots of the weather data for the following comparisons:
       - Latitude versus temperature
       - Latitude versus humidity
       - Latitude versus cloudiness
       - Latitude versus wind speed
    2. Determine the correlations for the following weather data:
       - Latitude and temperature
       - Latitude and humidity
       - Latitude and cloudiness
       - Latitude and wind speed
    3. Create a series of heatmaps using the Google Maps and Places API that showcases the following:
       - Latitude and temperature
       - Latitude and humidity
       - Latitude and cloudiness
       - Latitude and wind speed
  3. Visualize Travel Data. Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:
    1. Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
    2. Create a heatmap for the new DataFrame.
    3. Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
    4. Store the name of the first hotel in the DataFrame.
    5. Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.

### Results:

Deliverable 1: Retrieve Weather Data. Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

![DataFrame](https://github.com/chocoplace/World_Weather_Analysis/blob/main/Resources/D1.png)

Deliverable 2: Create a Customer Travel Destinations Map. Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

![Destination Map](https://github.com/chocoplace/World_Weather_Analysis/blob/main/vacation_search/WeatherPy_vacation_map.png)

Deliverable 3: Create a Travel Itinerary Map. Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

Travel Itinerary Map

![Travel Itinerary Map](https://github.com/chocoplace/World_Weather_Analysis/blob/main/vacation_itinerary/WeatherPy_travel_map.png)

Marker Layer Map of the Travel Itinerary Map

![Marker Layer Map](https://github.com/chocoplace/World_Weather_Analysis/blob/main/vacation_itinerary/WeatherPy_travel_map_markers.png)

-- 
End 
