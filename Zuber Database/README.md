# Zuber Ride-Sharing Analysis Project

## Project Description

As a student analyst for Zuber, a new ride-sharing company launching in Chicago, I used a cleaned dataset provided by Tripleten's data analysis team to identify patterns in the available data through SQL. The goal was to understand passenger preferences and the impact of external factors on rides. This involved analyzing competitor data and testing a hypothesis about how weather conditions affect ride frequency.

## Data

The analysis uses a database with information on taxi rides in Chicago, including the following tables:

* **neighborhoods:**
    * `name`: Name of the neighborhood
    * `neighborhood_id`: Neighborhood code
* **cabs:**
    * `cab_id`: Vehicle code
    * `vehicle_id`: The vehicle's technical ID
    * `company_name`: The company that owns the vehicle
* **trips:**
    * `trip_id`: Ride code
    * `cab_id`: Code of the vehicle operating the ride
    * `start_ts`: Date and time of the beginning of the ride (time rounded to the hour)
    * `end_ts`: Date and time of the end of the ride (time rounded to the hour)
    * `duration_seconds`: Ride duration in seconds
    * `distance_miles`: Ride distance in miles
    * `pickup_location_id`: Pickup neighborhood code
    * `dropoff_location_id`: Dropoff neighborhood code
* **weather_records:**
    * `record_id`: Weather record code
    * `ts`: Record date and time (time rounded to the hour)
    * `temperature`: Temperature when the record was taken
    * `description`: Brief description of weather conditions (e.g., "light rain," "scattered clouds")

## Analysis Steps

1. Exploratory Data Analysis:

Conduct exploratory data analysis using SQL queries.


2. Customer Impact of Weather Conditions:

Identify the impact of weather conditions on customers.
