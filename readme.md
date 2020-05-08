# Ford GoBike System Data Exploration

## by Michael F. H. Georgy


## Dataset

> This data set includes information about individual rides made in GoBike bike-sharing system (now called Baywheels) covering the greater San Francisco Bay area in the first 3 months of 2020.

> The dataset was downloaded from https://s3.amazonaws.com/baywheels-data/index.html and multiple data files needed to be joined together to get a single dataset that required some data wrangling in order to make it tidy for analysis.

> Data wrangling included the following:
	Data was gathered, assessed and cleaned as follows:

	I- Tidiness
		T1. Month column added  with the month name as value so that it is easy to distinguish the month after joining the datasets.

		T2. 3 separate dataframes joined into 1.

		T3. Unrequired columns for analysis (ex: start_station_latitude, start_station_longitude, end_station_longitude, end_station_longitude) were deleted.

		T4. Columns containing duration in minutes, hours, and days were added to improve perception of time.

		T5. 2 columns (start_day, end_day) containing day name obtained from start_time and end_time were added after converting data type to datetime.

	II- Quality
		Q1. Erroneous datatypes (start_time, end_time, start_station_id, end_station_id, bike_id) were converted to string since no operation will be performed on its values.

		Q2. Outlier in Jan dataset was deleted

## Summary of Findings

> Most important findinngs can be viewed in the accompanying slides. These are:
	1. An average ride duration lies in the 3-14 minute range.
	
	2. Most trips were taken in February, and trips started and ended on Wednesday.
	
	3. At durations less than or equal to 60 minutes, both customers (casual) and subscribers (members) have achieved similar duartions of use
	
	4. When viewed by Month, without setting a duration limit, the plot shows that some customers had longer trip durations than subscribers.
	
	5. The idea is succeeding since the average Trip duration has been increasing since Jan 2020 and reached it's peak in March which concludes that people are depending more on bikes to go to farther places.
