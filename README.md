# java-script-datatype
Created with CodeSandbox
# Weather App

A simple weather application built with JavaScript that allows users to check the current temperature and humidity of various cities.

## JavaScript Features

- **Weather Data**: Uses a JavaScript object to store weather information for different cities.
- **User Input**: Prompts the user to input a city name to fetch the weather data.
- **Temperature Conversion**: Converts the temperature from Celsius to Fahrenheit.
- **Alerts**: Displays the weather information using alert dialogs.

## JavaScript Data Structure

The weather data is stored in a JavaScript object named `weather` with the following structure:

```javascript
let weather = {
  city_name: {
    temp: temperature_value,
    humidity: humidity_value,
  },
  // ... more cities
};
How It Works
User Input: Prompts the user to enter a city name using prompt().
Data Retrieval: Checks if the entered city exists in the weather object.
Temperature Conversion: Converts the temperature to Fahrenheit using the formula (temperature * 9) / 5 + 32.
Display Information: Displays the weather information using alert dialogs.
JavaScript Code Snippet
Here's a snippet of the JavaScript code responsible for fetching and displaying the weather data:

let city = prompt("Enter a city?");
city = city.toLowerCase();

if (weather[city] !== undefined) {
  let temperature = weather[city].temp;
  let humidity = weather[city].humidity;
  let celsiusTemperature = Math.round(temperature);
  let fahrenheitTemperature = Math.round((temperature * 9) / 5 + 32);

  alert(
    `It is currently ${celsiusTemperature}°C (${fahrenheitTemperature}°F) in ${city} with a humidity of ${humidity}%`
  );
} else {
  alert(
    `Sorry we don't know the weather for this city, try going to https://www.google.com/search?q=weather+${city}`
  );
}
Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

License
This project is licensed under the MIT License. See the LICENSE file for details.

This README.md file focuses on explaining the JavaScript functionalities and structure of your Weather App.

