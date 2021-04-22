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


 #### Represents a request for a meeting in a calendar.

| Element | Description | Type | Required | Notes |
|---- | --- | --- | --- | --- |
| meeting | Top level | meeting data object | Required | |
| &nbsp; &nbsp; time | When meeting starts.  | string | Required | Format is YYYY-MM-DD HH:MM:SS. Timezone is GMT. |
| &nbsp; &nbsp; duration | How long meeting lasts | number | Required | In minutes |
| &nbsp; &nbsp; description | Description of the meeting | string | Required | |
| &nbsp; &nbsp; location | Location of the meeting | number | Optional | Default is an empty string |
| &nbsp; &nbsp; reminder | How many minutes before the meeting a reminder event should take place | number | Optional | Default is 10 minutes |
| &nbsp; &nbsp; invitees | List of email address of people to invite to the meeting | array of string | Optional | The strings should be valid email addresses. Default is an empty array. |


#### Represents a menu.

| Element | Description | Type | Notes |
|---- | --- | --- | --- |
| Top level | Menu columns | array of menu column objects | |
| &nbsp; &nbsp; header | Name of the column | string | |
| &nbsp; &nbsp; items | List of menu items under the column | array of menu items | |
| &nbsp; &nbsp; id | ID of the menu | string | |
| &nbsp; &nbsp; label | Label that is displayed in the user interface | string | |

#### Represents a song.

| Element | Description | Type | Notes |
|---- | --- | --- | --- |
| song | Top level | song data object | |
| &nbsp; &nbsp; title | Song title | string | |
| &nbsp; &nbsp; artist | Song artist | string | |
| &nbsp; &nbsp; musicians | A list of musicians who play on the song | array of string | |


---
---

Click [here](https://dbvamsi.github.io/markdown/) to get back to index.
