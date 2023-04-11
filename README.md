# Python Weather API
Using Python, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

It may seem obvious that it gets hotter but, if pressed for more information, how would you prove that?

## Background
### Part 1: WeatherPy
Create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python library, the OpenWeatherMap API, and your problem-solving skills to create a representative model of weather across cities.

#### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
Use the OpenWeatherMap API to retrieve weather data from the cities list. Next, you'll create a series of scatter plots to showcase the following relationships:

- Latitude vs. Temperature

- Latitude vs. Humidity

- Latitude vs. Cloudiness

- Latitude vs. Wind Speed

#### Requirement 2: Compute Linear Regression for Each Relationship
Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).

Next, create a series of scatter plots (like the following image) showing the relationship between the variable pairs below:

![Python API example](https://user-images.githubusercontent.com/111451303/231047229-b22e5371-82f3-4a2a-bce2-999c82ce0475.png)

- Northern Hemisphere: Temperature vs. Latitude

- Southern Hemisphere: Temperature vs. Latitude

- Northern Hemisphere: Humidity vs. Latitude

- Southern Hemisphere: Humidity vs. Latitude

- Northern Hemisphere: Cloudiness vs. Latitude

- Southern Hemisphere: Cloudiness vs. Latitude

- Northern Hemisphere: Wind Speed vs. Latitude

- Southern Hemisphere: Wind Speed vs. Latitude

### Part 2: VacationPy
Use your weather data skills to plan future vacations. You'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

Create a map that displays a point for every city in the ```city_data_df``` DataFrame as shown in the following image. The size of the point should be the humidity in each city.

Narrow down the ```city_data_df``` DataFrame to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21

Wind speed less than 4.5 m/s

Zero cloudiness

Create a new DataFrame called ```hotel_df``` to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:
