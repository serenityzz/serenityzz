---
title: "GetWeather API"
date: 2025-09-25
tag: API 
---

Use the **GetWeather API** to get current weather conditions and seven-day forecasts for a specified city or location. Authentication with an API key is required.

## Base URL

`https://api.weather.com/v1/weather`

## Authentication

All requests require an API key. You can provide your API key in either of the following ways:

- **Query parameter**
  
  `?apikey=your_api_key`

- **HTTP header**
  
  `Authorization: Bearer your_api_key`

## Common request parameters

The following request parameters apply to all GetWeather API operations.

|Parameter  |Type   |Required |Description                                                                                                                                                                                                   |
|:---------- |:------ |:-------- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `location` | string | Yes      | The location for which you want to get weather information. You can specify a city name (for example, `London`) or coordinates in the format `lat,lon` (for example, `51.50,-0.12`).                          |
| `units`    | string | No       | The units for weather values. <br>Valid values: <br>- `metric` (default): Celsius(°C) and meters/second. <br> - `imperial`: Fahrenheti (°F) and miles/hour.<br>- `standard`: Kevin (K) and meters/second.<br> |
| `apikey`   | string | Yes      | Your API key for authentication.                                                                                                                                                                              |

## Endpoints

### Get current weather

`GET /current`

Retrieves the current weather for a specified city or location.

#### Request example

`GET https://api.weather.com/v1/weather/current?location=London&units=metric&apikey=your_api_key`

#### Response syntax

```
{
  "city": "string",
  "country": "string",
  "latitude": number,
  "longitude": number,
  "temperature_celsius": number,
  "humidity_percent": number,
  "condition": "string",
  "wind_speed_kph": number,
  "observation_time": "string (ISO 8601)"
}
```

#### Response example

```
{
  "city": "London",
  "country": "United Kingdom",
  "latitude": 51.5074,
  "longitude": -0.1278,
  "temperature_celsius": 18,
  "humidity_percent": 72,
  "condition": "Partly cloudy",
  "wind_speed_kph": 14,
  "observation_time": "2025-04-29T10:00:00Z"
}
```

#### Response elements

|Element               |Type   |Description                                                         |
|:--------------------- |:------ |:------------------------------------------------------------------- |
| `city`                | string | Name of the city.                                                   |
| `country`             | string | Country of the specified city.                                      |
| `latitude`            | number | Latitude coordinate of the location.                                |
| `longitude`           | number | Longitude coordinate of the location.                               |
| `temperature_celsius` | number | Current temperature in degrees Celsius.                             |
| `humidity_percent`    | number | Current humidity level (percentage).                                |
| `condition`           | string | Current weather condition (for example, *Partly cloudy*).           |
| `wind_speed_kph`      | number | Current wind speed in kilometers per hour.                          |
| `observation_time`    | string | Time when the weather information was observed, in ISO 8601 format. |

### Get seven-day weather forecast

`GET /forecast`

Retrieves a seven-day weather forecast for a specified city or location.

#### Request example

`GET https://api.weather.com/v1/weather/forecast?location=London&units=metric&apikey=your_api_key`

#### Response syntax

```
{
"location": {
    "city": "string",
    "country": "string",
    "latitude": number,
    "longitude": number
  },
  "forecast": [
    {
      "date": "string (YYYY-MM-DD)",
      "temperature_celsius": {
        "min": number,
        "max": number
      },
      "condition": "string",
      "humidity_percent": number,
      "wind_speed_kph": number
    }
  ]
}

```

#### Response example

```
{
"location": {
    "city": "London",
    "country": "United Kingdom",
    "latitude": 51.5074,
    "longitude": -0.1278
  },
  "forecast": [
    {
      "date": "2025-09-24",
      "temperature_celsius": {
        "min": 12,
        "max": 19
      },
      "condition": "Partly cloudy",
      "humidity_percent": 70,
      "wind_speed_kph": 4.5
    },
    {
      "date": "2025-09-25",
      "temperature_celsius": {
        "min": 11,
        "max": 18
      },
      "condition": "Rain",
      "humidity_percent": 80,
      "wind_speed_kph": 6.3
    }
  ]
}
```

#### Response elements

|Element                              |Type   |Description                                   |
|:------------------------------------ |:------ |:--------------------------------------------- |
| `location.city`                      | string | Name of the city.                             |
| `location.country`                   | string | Country of the specified city.                |
| `location.latitude`                  | number | Latitude coordinate of the location.          |
| `location.longitude`                 | number | Longitude coordinate of the location.         |
| `forecast[]`                         | array  | List of forecast objects, one for each day.   |
| `forecast[].date`                    | string | Date of the forecast in YYYY-MM-DD format.    |
| `forecast[].temperature_celsius.min` | number | Minimum temperature in degrees Celsius.       |
| `forecast[].temperature_celsius.max` | number | Maximum temperature in degrees Celsius.       |
| `forecast[].condition`               | string | Forecasted weather condition.                 |
| `forecast[].humidity_percent`        | number | Forecasted humidity level (percentage).       |
| `forecast[].wind_speed_kph`          | number | Forecasted wind speed in kilometers per hour. |

---

## Errors

If an error occurs, the service returns a standard error response in JSON format.

|Error                      |HTTP Status Code |Description                                                                                               |
|:-------------------------- |:---------------- |:--------------------------------------------------------------------------------------------------------- |
| `InvalidRequestException`  | 400              | The request is invalid. For example, a required parameter is missing or has an incorrect value.           |
| `UnauthorizedException`    | 401              | The request is not authorized. Verify that you provided a valid API key.                                  |
| `TooManyRequestsException` | 429              | The request exceeded the rate limit. Retry after the time specified in the `Retry-After` response header. |
