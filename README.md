# sqlalchemy-challenge
SQLAlchemy Homework - Surfs Up!

## Step 1 - Climate Analysis and Exploration Assignment 
 
 The ReadMe file and the startercode had some differences so I'm including below the step by step instructions as listed in the Read me File. 
 
Congratulations! You've decided to treat yourself to a long holiday vacation in Honolulu, Hawaii! To help with your trip planning, you need to do some climate analysis on the area. The following outlines what you need to do.
 
Using Python and SQLAlchemy to do basic climate analysis and data exploration of climate database. All of the following analysis will be done using SQLAlchemy ORM queries, Pandas, and Matplotlib.  Use the provided starter notebook and hawaii.sqlite files to complete your climate analysis and data exploration. 


1. Use SQLAlchemy create_engine to connect to your sqlite database.
2. Use SQLAlchemy automap_base() to reflect your tables into classes and 
3. Save a reference to those classes called Station and Measurement.
 
- The vacation range is approximately 3-15 days total. 

4. Choose a start date and end date for your trip. 
-- Precipitation analysis * Retrieving the last 12 months of precipitation data.

5. Select only the date and prcp values 
6. Load the query results into a Pandas DataFrame setting the index to date
7. Sort the DataFrame values by date
8. Plot using the DataFrame plot method 

-- Calculating the total number of stations.

9. List stations and obserbation counts in descending order
10. Identify the station with the highest number of observations (Use func.min, func.max, func.avg and func.count)

Calculating the last 12 months of temperature data 

11. filter by the station with the highest number of observations 
12. plot the results using histogram using bins=12

-- Use FLASK to create your routes. 
#use jasonify to convert API data into valid JSON response object. 
#Join the station and measurement tables for analysis. 

13. use / for Homepage - Listing all routes available 
14. use /api/v1.0/precipitation
15. convert querie results into a dictionary using date as the key and prcp as the value 
16. return the JSON representation of the dictionary. 
17. use /api/v1.0/stations
18. return a JSON list of stations from the data 
19. use /api/v1.0/tobs 
20. query for dates and temperature observations from a year from the last data point.
21. use api/v1.0/<start> and /api/v1.0/<start>/<end> 
22. return a JSON list of the min temperature, average temperature and max temperature given a start or end range *This is where you pick a vacation range from 3-15 days. 
 23. when given the start only, calculate TMIN, TAVG and TMAX for all dates greater than and equal to the start date. 
24. When given the start and end date, calculate the TMIN, TAVG, and TMAX for the start and end date inclusive. 
    

* Optional challenge queries. Recommended but not required for the homework.

##### Temperature Analysis I

 Is there a meaningful difference between the temperature in, for example, June and December?
 
##### Temperature Analysis II

* Use the `calc_temps` function to calculate the min, avg, and max temperatures for your trip using the matching dates from the previous year (i.e., use "2017-01-01" if your trip start date was "2018-01-01").
* Plot the min, avg, and max temperature from your previous query as a bar chart

##### Daily Rainfall Average

* Calculate the rainfall per weather station using the previous year's matching dates.
* Calculate the daily normals. Normals are the averages for the min, avg, and max temperatures.

