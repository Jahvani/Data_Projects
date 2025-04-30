# Zuber Ride-Sharing Analysis Project

## Project Description

As an analyst for Zuber, a new ride-sharing company launching in Chicago, the goal of this project is to identify patterns in available data to understand passenger preferences and the impact of external factors on rides. This involves analyzing competitor data and testing a hypothesis about how weather conditions affect ride frequency.

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

1.  **Exploratory Data Analysis:**
    * Find the number of taxi rides for each taxi company for November 15-16, 2017.
    * Find the number of rides for taxi companies with "Yellow" or "Blue" in their names for November 1-7, 2017.
    * Find the number of rides for "Flash Cab" and "Taxi Affiliation Services" in November 2017, and group the rides of all other companies into "Other".

2.  **Impact of Weather on Ride Duration:**
    * Retrieve the identifiers for the O'Hare and Loop neighborhoods.
    * Categorize weather conditions from the `weather_records` table into "Bad" (rain or storm) and "Good".
    * Retrieve all Saturday rides from the Loop to O'Hare, their weather conditions, and ride durations.
    * Exclude rides with missing weather data.
