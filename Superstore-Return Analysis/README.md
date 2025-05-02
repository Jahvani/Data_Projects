# BI Analyst Project: Understanding and Reducing Returned Orders at Superstore

## Introduction

This project was undertaken as a **TripleTen student** to analyze the high volume of returned orders at the Superstore. The goal was to identify the root causes of these returns and provide actionable insights to the CEO on how to reduce them, ultimately improving profitability. This analysis involved data preparation, visualization, dashboard creation, and the development of a data story for presentation.

## Project Objective

The primary objectives of this project were to:

* Investigate various factors to understand what is driving customer order returns at the Superstore.
* Determine the most effective metrics for measuring returns (return rate, total cost, total number).
* Identify key root causes of returned orders through data analysis and visualization.
* Design and build an interactive dashboard to monitor and analyze returns.
* Develop a data story to present the findings and recommendations to the CEO.

## Data Description

The analysis was based on the Superstore dataset, which includes information on orders, customers, products, shipping, and a separate table for returned items. The "Returns" table was **left-joined** with the "Orders" table to identify returned orders effectively. A **calculated field** named "Returned" was created, where "Yes" values were converted to `1` and "null" values to `0`. The average of this field represents the **return rate**.

## Methodology & Visualizations

The project followed a structured approach involving exploratory data analysis and visualization in Tableau:

### 1. What is Causing Returns?

The following worksheets were created to analyze different aspects of return rates:

* **Sales vs. Returns Scatterplot (by Product Subcategory):** A scatterplot visualizing the relationship between total sales and total returns for each product subcategory to identify any correlation patterns. *
* **Return Rate by Product Category Bar Chart:** A bar chart showing the average return rate for each product category to identify categories with higher propensity for returns. 
* **Return Rate by Customer (Filtered):** A bar chart displaying the return rate for individual customers, with a filter applied to exclude customers with only one order to focus on repeat returners. 
* **Return Rate by Geographic Measure (Map):** A map visualizing the return rate by state or city to identify any geographic concentrations of returned orders. 
* **Return Rate by Time Measure (Line Chart):** A line chart showing the return rate over time (e.g., by month or week) to identify any seasonal trends in returns. 
* **Composite Charts (Multiple Factors):** Two different composite charts combining factors like date/geography/product category to explore the interplay of multiple dimensions on return rates. 

### 2. Building a Dashboard for Monitoring Returns

* **Low-Fidelity Mock-ups:** Pen-and-paper sketches of at least three different dashboard layouts were created to plan the structure and flow of information. 
* **Dashboard Template:** A template was created in Tableau using empty containers, mirroring the chosen mock-up design. 
* **Final Dashboard:** The previously created worksheets were integrated into the dashboard template. Relevant markers, images, and titles were added to finalize the dashboard for effective monitoring and analysis of returns. 

### 3. Presenting Your Analysis and Dashboard

* **Story Arc (Captions Only):** A draft of the presentation story arc was developed using only captions for each Story Point, outlining the flow of the analysis and key findings.
* **Tableau Story:** A Tableau Story was constructed using the created worksheets and dashboards to build presentation-style slides. 
* **Presentation:** A 3 to 5-minute presentation of the Tableau Story was prepared (either as a screen recording or in PDF format) to deliver the analysis and recommendations. 

## Results & Recommendations

The analysis conducted in this project aimed to identify the key drivers of returned orders at the Superstore. The findings, presented through visualizations and the interactive dashboard, provide insights into which product categories, customer segments, geographic locations, and time periods experience higher return rates.

Based on these insights, the presentation outlines potential root causes for the returns and proposes actionable steps the Superstore can take to mitigate these issues and reduce the overall volume of returned orders. This includes recommendations on how to measure returns effectively and how to utilize the developed dashboard for ongoing monitoring and identification of problem areas.

---
