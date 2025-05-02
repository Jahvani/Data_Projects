# Shopify App Analysis

## Introduction

This project analyzes the landscape of apps on the Shopify platform using publicly available data scraped from Shopify websites. The goal is to identify key factors that contribute to the success of a Shopify app. The analysis is presented as a Power BI report with multiple pages, each addressing a specific aspect of the app ecosystem.

## Project Objective

The primary objectives of this project were to:

* Analyze the types of apps available on the Shopify platform.
* Investigate factors influencing app reviews and user opinions.
* Identify responsive and highly-rated app developers.

## Data Description

The analysis uses the `shopify.xlsx` dataset, which contains the following four tables:

* **apps:** Details of the apps on the Shopify app marketplace (app ID, developer, category, reviews count, rating, last modified date, etc.).
* **apps_categories:** A join table connecting apps with their respective categories.
* **categories:** Categories of the apps. Each app can belong to multiple categories.
* **reviews:** Individual user reviews for apps, including rating, comment, helpful count, and developer reply.

## Methodology

The project is structured into three parts, each corresponding to a page in the Power BI report. Each part involves creating specific visualizations to answer the posed questions. 

### Part 1: App Landscape

This part focuses on understanding the overall app ecosystem.

* **KPI Card (Unique App Count):** A KPI card displays the total number of unique apps in the dataset.
* **Line Chart (Review Count Over Time):** A line chart shows the trend of review counts over time, with the last modified date on the X-axis and the sum of review counts on the Y-axis. 
* **Scatterplot (Reviews vs. Rating):** A scatterplot visualizes the relationship between the number of reviews (X-axis) and the average rating (Y-axis) for each app. A text box annotates the interpretation of this relationship.

### Part 2: Reviews

This part delves into the characteristics of app reviews.

* **Helpful Reviews Column & Card:** A calculated column named `helpful_reviews` is created in the `Reviews` table using the DAX expression `rating * (1 + helpful_count)`. A card visual displays the average value of this new column.
* **Developer Answered vs. Rating Scatterplot:** A calculated column named `developer_answered` is created in the `Reviews` table using a DAX expression. This column is 1 (TRUE) if the `developer_reply` column is not blank and 0 (FALSE) otherwise.

### Part 3: App Reviews

This part analyzes app reviews in relation to app developers.

* **Relationship between Reviews and Apps Tables:** A many-to-one relationship is created in the data model between the `Reviews` table (many) and the `Apps` table (one) using the `app_id` and `id` columns.
* **Bar Chart (Sum of Rating by Developer):** A bar chart displays the sum of ratings for each developer.
* **Bar Chart (Helpful Review Average by Developer):** A new bar chart shows the average helpful review score (calculated in Part 2) for each developer, providing a more balanced view.
* **Bar Chart (Developer Responsiveness):** A bar chart displays the count of `developer_answered` (from Part 2) for each developer. A filter is applied to this visual to only include apps with more than 500 reviews. This identifies the most responsive developers.

## Results

The Power BI report provides insights into the Shopify app ecosystem, including:

* The total number of apps.
* Trends in app review counts over time.
* The relationship between app rating and the number of reviews.
* The impact of helpful reviews on overall app scores.
* The correlation between developer responsiveness and app ratings.
* Identification of top-rated and most responsive app developers.

