# Project Requirements: Manhattan Vacation Rental Market Analysis

This project analyzes Airbnb data for Manhattan to provide insights into which property types are most attractive for vacation rentals. The analysis aims to guide investment decisions.

## Key Requirements

1.  **Neighborhood and Property Size Analysis:**

    * Analyze data to determine which neighborhoods are most attractive for vacation rentals.
    * Analyze data to determine which property sizes (i.e., number of bedrooms) are most popular for vacation rentals.
    * Investigate if different neighborhoods have different preferences for property sizes.
    * Use `number_of_reviews_ltm` to assess listing attractiveness.
    * Clean the neighborhood column and store cleaned values in a new column named `neighborhood_clean`.
    * Create a pivot table to identify the top 10 most attractive neighborhoods.
    * Include a bar chart displaying the number of reviews for the top 10 listings.
    * Clean the bedrooms column to handle empty cells (representing studio apartments) and store cleaned values in a new column named `bedrooms_clean`.
    * Create a pivot table to determine the most popular property sizes for rentals.
    * Update the pivot table to recommend specific property sizes for each of the top 10 neighborhoods.

2.  **Revenue Analysis:**

    * Identify "top listings" based on the most popular property size for each of the top 10 neighborhoods.
    * Create a new column in the listings data called `top_listing` (1 if a listing matches the criteria, 0 otherwise).
    * Calculate potential revenue for top listings using the calendar sheet.
    * Add a new column to the calendar data called `revenue_earned`. If `available` is "f", set `revenue_earned` to `adjusted_price`; otherwise, set it to $0.
    * Create a new column in the listings data called `revenue_earned` using the `SUMIF()` function to bring over the total `revenue_earned` from the 30-day calendar data.
    * Create a pivot table that orders all top listings according to revenue, using `top_listing` as a filter.
    * Estimate annual revenue for recommended listings by multiplying the 30-day revenue by 12.

3.  **Formatting and Documentation:**

    * Hide unnecessary columns.
    * Include an executive summary and table of contents in the analysis.
    * Document data cleaning steps in a change log.
    * Clearly document assumptions.
    * Ensure consistent formatting, borders, cell background colors, font styles, and sizes across the analysis.
