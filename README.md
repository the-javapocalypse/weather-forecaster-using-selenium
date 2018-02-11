# WEATHER FORECAST

A simple python web crawler to fetch three days [weather forecast](http://www.weather-forecast.com)

## Getting Started

### Installation

After downloading or cloning the repo, Download [chrome webdriver](https://sites.google.com/a/chromium.org/chromedriver/downloads) or (firefox webdriver)[https://github.com/mozilla/geckodriver/releases] and extract the folder in the root folder of project. AFter that you'll need to install selenium. You can get it through pip.

```pip isntall selenium```


### HOW IT WORKS

It prompts to enter a city name to get the forecast for and requests the forecast for the city's name that is taken as input and replaces 'city' in url with the one entered
http://www.weather-forecast.com/locations/<city_name_entered>/forecasts/latest

The HTML ```div``` containing the the content of forecast is fetched through it's class. Since there are more elements associated with the same class, an array of elements is returned. The forecast for the first three days is at the index 0. We use ```.text``` to get the text of the div, which is the forecast.

## Built With

1. Python 3.6
2. Selenium

## Contributing

1. Fork it
2. Create your feature branch: git checkout -b my-new-feature
3. Commit your changes: git commit -am 'Add some feature'
4. Push to the branch: git push origin my-new-feature
5. Submit a pull request

## Authors

+ Muhammad Ali Zia

## License

This project is licensed under the MIT License
