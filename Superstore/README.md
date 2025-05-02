# Data Visualization Project: Saving SuperStore

## Introduction

This project was undertaken to analyze the operations of a struggling superstore and identify strategies to increase its profitability and avoid bankruptcy. As a Tripleten Student, I used data visualization techniques to uncover key insights related to profits, losses, advertising opportunities, and product returns. The goal was to provide actionable recommendations based on visual evidence.

## Project Objective

The primary objectives of this project were to:

* Identify the biggest profit centers and loss-makers based on different dimensions.
* Determine which products and product subcategories the superstore should stop selling or focus on.
* Pinpoint the best combinations of states and months for advertising based on profit potential.
* Analyze product return rates to identify problematic items and customers.
* Explore the relationship between average profit and average return rate across different dimensions.

## Data Description

The analysis was based on the SuperStore dataset, which included information on sales, profits, shipping details, product categories, customer information, and return data. The "Returns" table was joined with the "Orders" table to analyze return rates effectively. A calculated field was created to represent returns numerically (1 for "Yes", 0 for "null").

## Methodology & Visualizations

This project was structured into three main parts, each addressing a specific business question through data visualization:

### Part 1: Profits & Losses

* **Biggest Profit Centers and Loss-Makers:** Visualizations (e.g., heatmaps, bar charts) were created to identify the top two profit-generating and the top two loss-generating pairs of dimensions (e.g., subcategory + region, shipping mode + product ID). 
* **Products to Stop Selling:** A visualization (e.g., scatter plot, bar chart) was used to identify products with consistently low or negative profitability. 
* **Product Subcategories to Focus On and Stop Selling:** Visualizations (e.g., bar charts) highlighted the top 3 most profitable and the bottom 3 least profitable product subcategories. 

### Part 2: Advertising

* **Best Advertising Combinations:** A visualization (e.g., heatmap, line chart) displayed the average profit for each month of the year for the top 3 identified states, helping to determine the most promising advertising periods. 
* **Advertising Budget Justification:** Based on the return on ad spend ratio (willingness to spend 1/5 of profits), an argument was made, supported by the profit visualizations, for the potential advertising budget for the identified state-month combinations.

### Part 3: Returned Items

* **Products with Highest Return Rate:** A visualization (e.g., bar chart) showcased the products with the highest percentage of returns. 
* **Customers with Highest Return Rate:** A visualization (e.g., bar chart) identified the customers with the highest number or rate of returned items. 
* **Profit vs. Return Rate Analysis:** A scatter plot or similar visualization displayed the average profit against the average return rate for a chosen dimension (e.g., state, shipping mode, product type), providing a visual basis for decisions on whether to continue or discontinue business based on that dimension. 

## Results & Recommendations

The visualizations generated in this project led to specific recommendations for the SuperStore, including:

* Focusing on the most profitable product and dimension combinations.
* Discontinuing the sale of consistently unprofitable products and potentially underperforming subcategories.
* Strategically allocating advertising budgets to the most promising state-month combinations based on profit potential.
* Investigating the reasons behind high return rates for specific products and customers.
* Evaluating business decisions based on the relationship between profit and return rates across different dimensions.




