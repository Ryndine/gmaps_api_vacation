# Weather Travel Analysis

## Objective: 
Retrieve weather data using APIs, clean data with pandas, plot data onto a map, and create a travel itinerary for users.

## Tools used:
- Jupyter
- Pandas
- Citipy
- Open weather map API
- Google maps API

## Preparing data:

**City data:**  

For this dataset I want to create a random set of cities, and to do that I'm going to generate a list of corridinates first, then use citipy to find cities nearest to those coordinates.

Next I want the user to be able to select places based the on the weather conditions they prefer to have during their travels. So after creating a list of cities, I'm going to use the cities and run an API call to "openweathermap" in order to retrieve the weather data on each city as well as further information like the country the city is located.

After the data is collected form the API call, I'm storing everyhing in a pandas dataframe for use later.

**Hotel data:**

With the city data generated I next step is to take the list of cities and find nearby hotels based on user temperature preferences.

Using the inputs provided by the user, I filter the dataframe down to contain only what meets the criteria, then using that dataframe I'll do a gmaps API call to find hotels for those cities.

After I collect the hotel data, I save it to a csv, then create a google map with markers on it to give the user a visualization of the returned results.

**Itinerary data:**

After applying my hotel data to the map I chose a few destinations for my destinations map.

With my selection of cities I created variables which contained data for each city and coordinates, then made a new dataframe with the selected data.

Using google maps marker layer I added the detailed information for each stop, then using the destinations layer I applied the trip directions (via car) while making sure to hide the markers to prevent it from covering the marker layer information.

# Google Map API Results

