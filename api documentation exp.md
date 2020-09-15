#### Represents a daily temperature data.

dailydata: Daily temperature data received
| Element |Description | Type | Notes |
|---|---|---|---|
|dailyData|Daily data received by the computer||Data is received Hourly|

hourlyData: Hourly temperature data received
| Element |Description | Type | Notes |
|---|---|---|---|
|hourlyData|Holds the information of device and time|||
|&nbsp; time|Time at which the device reported the information|number| time is localtime|
|&nbsp; device| Device that reported the information||devices have unique IDs|


device: Contains the id & temperature parameters of device
| Element |Description | Type | Notes |
|---|---|---|---|
|device| Holds the information of device ID,temperature & humidity reported|||
|&nbsp; id| Unique ID of the device|number||
|&nbsp; temperature|Temperature details that were reported|number|format is degree F
|&nbsp; humidity| Humidity details that were reported|number|is reported in percentage (%)|


#### Represents a one day weather forecast.

| Element | Description | Type | Notes |
|----|----|----|----|
| date | Date of the forecast | string | format is YYYY-MM-DD |
| description | Description of the forecast | string | "description" can have these values: "sunny", "overcast", "partly cloudy", "raining", and "snowing" |
| maxTemp | forecast Maximum Temperature | integer | "maxTemp" is in degrees Celsius |
| minTemp | forecast Minimum Temperature | integer | "minTemp" is in degrees Celsius |
| windSpeed | forecast Wind Speed | integer | "windSpeed" is in kilometres per hour |
| danger | Level of danger | boolean | |



#### Represents a one day weather forecast.

| Element | Description | Type | Notes |
|----|----|----|----|
| longitude | longitude where the forecast takes place | number | |
| lattitude | latitude where the forecast takes place | number | |
| forecasts | dates for which forecasts take place | an array of forecasts objects| |
|&nbsp;&nbsp; date | Date of the forecast | string | format is YYYY-MM-DD |
|&nbsp; &nbsp; description | Description of the forecast | string | "description" can have these values: "sunny", "overcast", "partly cloudy", "raining", and "snowing" |
|&nbsp;&nbsp; maxTemp | High Temperature | number | "maxTemp" is in degrees Celsius |
|&nbsp;&nbsp; minTemp | Low Temperature | number | "minTemp" is in degrees Celsius |
|&nbsp;&nbsp; windSpeed | forecast Wind Speed | number | "windSpeed" is in kilometres per hour |
|&nbsp;&nbsp; danger | true if the whether conditions are dangerous; otherwise false | boolean | |
