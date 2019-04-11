# Latitude-vs-X
This is a python script that utilizes OpenWeatherMap API to get weather data from over 8,000 random cities across the globe.

First random latitude and longitude coordinates are randomly generated and saved to lists.  These are then run through citypy to get the nearest city name from the coordinates.  Unique cities are saved to another list.  That list is then used with the OpenWeatherMap API to get JSON data.  The JSON is loaded into a Pandas dataframe and exported to a CSV, then the various weather characteristics are plotted against the latitude with MatPlotLib.

I encountered a minor issue in my latest run of the script where three cities returned from OpenWeatherMap had a humidity value of 296%.  I removed these from the dataframe, rewrote the CSV, and replotted the data.
