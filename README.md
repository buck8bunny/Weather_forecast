# Weather_forecast
The code retrieves the user's selected city and fetches weather data from the OpenWeatherMap API

<p align="center">
      <img src="[Project Logo Url](https://i.ibb.co/rMsZgHH/Screenshot-1.png)" width="726">
</p>


## About

The provided code is a JavaScript function that performs the following tasks:

1. The function `Complete()` is defined. It tries to retrieve the value entered in an input field with the id "city" from the HTML document. If the value is found, it is stored in the browser's local storage with the key "city". If there is an error (e.g., the input field does not exist), the default value "London,uk" is stored in the local storage.

2. The code then makes a fetch request to the OpenWeatherMap API to retrieve weather data for the city stored in the local storage. The API URL is constructed using the stored city value, an API key, and additional parameters for units (metric) and language (Ukrainian).

3. The fetch request returns a promise that, when resolved, converts the response to JSON format.

4. Another promise is chained to the previous one, which receives the JSON data as a parameter. It logs the data to the console and updates various elements in the HTML document with weather-related information. For example, it sets the current date, city name, temperature, weather description, and an image corresponding to the weather condition.

5. If any errors occur during the fetch request or promise chaining, the catch block is executed. In the provided code, it does not contain any specific error handling logic.

