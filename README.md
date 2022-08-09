For this project, a Python script was created to visualize the weather of 500+ cities of varying distance from the equator. This was done using simple Python libraries & the OpenWeatherMap API,  to create a representative model of weather across cities.

1. The WeatherPy file used matplotlib, pandas, numpy, requests, time, json, citipy, scipy.stats. 

First, a list of cities was generated using the citipy library. This library returns the name of the cities using its geolocation. Next, the OpenWeatherMap api was used to perform a weather check on each city in the list. This data was then put into a dataframe and exported to a CSV file. 

Next, a series of scatter plots were created to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

After this, the linear regression for each relationship was computed, and these were plotted (the plots were separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude)). The plots made were:

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

2. In the VacationPy file, matplotlib, pandas, numpy, requests, gmaps and os libraries were used. 

The CSV file from the previous script was loaded into a DataFrame again, and then used to create a heatmap. 
Next, the cities with a humidity of less than 15% were selected, and the Google Places API was used to locate hotels near that location, and places on top of the heatmap. 

All plots and heatmaps are saved as PNG files in the 'Images' folder. Observable trends are added in the Jupyter notebooks. 
