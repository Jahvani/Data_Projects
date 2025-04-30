# Manhattan Vacation Rental Market Analysis

This project analyzes Airbnb data for Manhattan to provide insights into which property types are most attractive for vacation rentals. The analysis aims to guide investment decisions by identifying popular neighborhoods and property sizes, and by estimating potential revenue.

## Project Description

The analysis addresses the following questions from the provided data from TripleTen:

* Which neighborhoods and property sizes (i.e., number of bedrooms) are most attractive for vacation rentals?
* How much money did these listings generate?

## Data

* NYC Airbnb Data

## Analysis

1.  **Which neighborhoods and property sizes are most attractive for vacation rentals?**

    * Cleaned the neighborhood column to remove inconsistencies.
    * Used `number_of_reviews_ltm` as a proxy for attractiveness.
    * Created pivot tables to identify:
        * Top 10 most attractive neighborhoods.
        * Most popular property sizes (number of bedrooms).
        * Neighborhood preferences for property sizes.
    * Cleaned the bedrooms column to handle empty cells (representing studio apartments).
    * Visualized the number of reviews for the top 10 listings using a bar chart.

2.  **How much money did the most attractive listings generate?**

    * Defined "top listings" based on the most popular property size for each of the top 10 neighborhoods.
    * Calculated `revenue_earned` for each listing using the calendar sheet.
    * Used the `SUMIF()` function to calculate the total `revenue_earned` for each top listing over a 30-day period.
    * Created a pivot table to rank top listings by revenue.
    * Estimated annual revenue by multiplying the 30-day revenue by 12.

## Key Findings

* Identified the top 10 most attractive neighborhoods for vacation rentals in Manhattan.
* Determined the most popular property sizes for rentals.
* Analyzed neighborhood preferences for property sizes.
* Estimated the potential revenue of top-performing listings.

## Recommendations

The report provides insights to help the client identify the most promising neighborhoods and property types for investment in the Manhattan vacation rental market.

