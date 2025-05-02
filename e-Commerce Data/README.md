# BI Analyst Project: Turning Event Logs into Business Metrics

## Introduction

This project was undertaken as a junior analyst at an e-commerce company. The goal was to analyze raw transaction logs to understand user behavior and provide insights to the executive team. The project focused on building a conversion funnel and performing cohort analysis to assess website performance and customer retention.

## Project Objective

The primary objectives of this project were to:

* Create a conversion funnel to visualize and quantify the user journey from product page view to purchase.
* Prepare data for cohort analysis to track customer acquisition and retention over time.
* Calculate retention rates for different customer cohorts.
* Document the analysis process and results in a clear and concise manner.

## Data Description

The analysis was based on a dataset of raw user activity logs. The dataset included the following columns:

* **user_id:** Unique identifier for each customer.
* **event_type:** Type of user activity (e.g., page view, add to cart, purchase).
* **category_code:** Category of the product.
* **brand:** Brand of the product.
* **price:** Price of the product (USD).
* **event_date:** Date of the user activity (YYYY-MM-DD).

The raw data was located in the "raw\_user\_activity" tab of the Business Analytics Project Google spreadsheet.

## Methodology

The project was divided into the following parts:

### Part 1: Build a conversion funnel

1.  Extracted data from the "raw\_user\_activity" sheet to create a pivot table named "conversion\_funnel".
2.  Counted the unique users for each stage of the funnel (3 stages).
3.  Calculated total conversion rates and conversion rates to the next step using formulas.

### Part 2: Prepare data for cohort analysis

1.  Filtered the "raw\_user\_activity" data to include only purchase events and copied it to a new sheet called "purchase\_activity".
2.  Created a pivot table named "first\_purchase" to determine the first purchase date for each user.
3.  Used the `VLOOKUP()` function to add a "first\_purchase\_date" column to the "purchase\_activity" sheet.
4.  Added "event\_month", "first\_purchase\_month", and "cohort\_age" columns to the "purchase\_activity" sheet using the `TEXT()` and `DATEDIF()` functions, respectively.

### Part 3: Calculate retention rates

1.  Created a pivot table named "cohort\_analysis" to group users into cohorts based on their first purchase month.
2.  Calculated the count of unique users for each cohort at different cohort ages.
3.  Created a "retention\_rates" sheet and calculated retention rates for each cohort month by month.

### Part 4: Organize and document your spreadsheet

1.  Filled in the "Executive Summary" sheet with a results synopsis and analysis descriptions.
    * Summarized the findings from the "conversion\_funnel" and "retention\_rates" sheets.
    * Explained the raw data, the conversion rate calculations, and the cohort analysis decisions.
2.  Reordered the spreadsheet tabs for clarity.
3.  Formatted the spreadsheets for readability (e.g., number and date formats, borders, bold fonts, frozen rows).

## Results

The key results of the project are documented in the "Executive Summary" sheet of the provided spreadsheet. This includes:

* Conversion rates at each stage of the funnel.
* Retention rates for different customer cohorts over time.

## Conclusion

This project provided valuable insights into user behavior and website performance. The conversion funnel highlighted drop-off points in the purchase process, while the cohort analysis revealed customer retention patterns. These findings can be used to inform business decisions and improve the customer experience.
