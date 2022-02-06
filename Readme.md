# Weather Retrieval, Travel Destinations and Travel Itinerary Map

### **Overview**
This project was created to demonstrate use of the Google Maps and Openweather APIs
	

The project is arranged into 3 scripts, each within their respective folder:

1) Weather_Database: Generates a a range of random longitudes, latitudes and assigns these against nearest cities from the citypy module. For these cities, an API call is amde to OpenWeatherMap to rereive longitude, latitude, Max Temp, Humidity, Cloudiness, Wind Speed and Current Weather Description. This data is output as a csv file WeatherPy_Database.csv which is used in step 2

2) Vacation Search: The user inputs a desired temperature range. The WeatherPy_Database.csv is into a dataframe and filtered based upon the required temperature range. Using the Googlemaps API the hotel field is populated and filtered and cleaned. Additionally, the info box for each city is populated and plotted agains the google maps figure. Results are output as WeatherPy_vacation.csv

3) Vacation Itinerary: Basedupon the results from 2, a route is plotted between 4 selected locations using the Google Maps Directions API. Result is output as WeatherPy_travel_maps_markers.png. Additionally the location infoboxes are shown, this detail is output as WeatherPy_travcel_map.png


