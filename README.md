# Latitude and Weather Trends Comparison

This repo showcases weather trends (cloudiness, humidity, maximum temperature and wind speed) compared with latitude.  The results of this analysis can be viewed [here](https://makeller234.github.io/Web-Design-Challenge/WebVisualizations/). The repository for that website can be found [here](https://github.com/makeller234/Web-Design-Challenge).

### WeahterPy.ipynb
This jupyter notebook uses citipy to find the actual cities that are closest to the randomly generated latitude and longitude locations.  Then the API from [OpenWeather](https://openweathermap.org/) was used to access their JSON to get the weather trends from each city. Information pulled from the JSON was put into a dataframe so that it could be graphed and plotted with linear regression to highlight correlation.

### VacationPy.ipynb
This jupyter notebook uses the same cities that were collected in WeatherPy.ipynb.  Gmaps was used to create a heatmap of the humidity of those cities. The dataframe was narrowed down to cities that had weather that I preferred, which is cool and cloudy. These cities where then used with the Google Places API to gather a Hotel name in that city. The hotels were plotted on the humidity heat map.


### Built With
* Python
* Pandas
* APIs
* Matplotlib

### Installing
* Git Clone the repository to your local machine
* You will need an API key from [OpenWeather](https://openweathermap.org/) and a [Google Places API key](developers.google.com)
* After the repo is cloned and the API keys are ready, create a file called "api_keys.py" and save the API keys with the variables "weather_api_key" for the Open Weather API key and "g_key" for the Google Places API