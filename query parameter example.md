# Represents the query parameters that returns list of bugs

| Parameter| 	Description| 	Type| 	Required|	Notes|
| ---      | ---         | ---  | ---       | ---  |
|startDate|	The start date for when the bug was created.|	date|	Optional|	Format for date is YYYY-MM-DD. Default is earliest recorded bug.|
|endDate|The end date for when the bug was created.	|date	|Optional|	Format for date is YYYY-MM-DD. Default is today’s date.|
|priority|	The priority value of how important the bug is.	|integer|	Optional|	Valid values are from 1 to 4, where 1 being the highest priority and 4 being the least priority. Default is all priorities.|
|severity	|The severity value	of how impactful the bug is.|integer|	Optional	|Valid values are from 1 to 4, where 1 being the highest severity and 4 being the least severity. Default is all severities.|
|status	|The status of the bug.	|string|	Optional|	Valid values are “open”, “closed”, “duplicate”, “notabug”. Default is all statuses.|
|start	|The starting index of bugs to return.|	integer|	Optional|	Zero is the first bug on the list. Default is Zero.|
|total|	The total number of bugs to return.|	integer|	Optional|	Default is total bugs minus the start value.|

## Sample Query (Not a real URL)

#### GET https://api.bugsquisher.com/bug?startDate=2020-01-01&endDate=2020-12-31&priority=1&severity=1&status=closed&start=0&total=100

The above query will return first 100 closed bugs in the year 2020 with both priority & severity of 1.
