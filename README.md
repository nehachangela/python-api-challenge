# python-api-challenge

This challenge is divided into two parts

Part one was analysing weather data from OpenWeatherMap. 
I have created Python script to visualize the weather of over 500 cities randomized geographic cooridate(using citipy) to show relationships between weather variables and Latitude(using OpenWeatherMaps API).
Creating DataFrame with retrival information for City, Country, Latitude, Longitude, Maximum Temperature, Humidity, Cloudiness, Wind Speed and Date.
Using this DataFrame scatter plots were requested for below categories:
City Latitude vs. Temperature
City Latitude vs. Humidity
City Latitude vs. Cloudiness
City Latitude vs. Wind Speed 
To further analysis, I created scatter plots for Northern and Southern Hemisphere for above categories:
linear regression line, and r values were drawn for each of the plots to observe the relationship in each category.

Part two was analysing ideal city for Vacation and find nearby Hotel
Using weather data from Part one, First, I mapped all the cities in the DataFrame using geoViews Python library.
Then, I set parameters for a new DataFrame with ideal weather to collect cities with ideal weather.
Using Geoapify API. Parameters where set to collect nearest Hotel Names within 10000 meters of the city coordinates.
try except was set to No Hotel Found with there were no hotel in 10000 meter radius.
Finally, using geoView again cities with ideal weather plotted on the map and using hover_cols, Hotel Name and County were appended.
