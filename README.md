# abhishekmishra_2511066_part3_regression_insights

# Regression-Based Business Insights & Model Interpretation

## Business Problem Summary

The leadership team wants to understand which factors are most strongly associated with monthly sales performance across retail stores. The objective is to identify key drivers of sales and support business decision-making related to marketing, inventory management, staffing, and store operations.

## Dataset Description

The dataset contains monthly store-level information including:

* Region
* Store Type
* Marketing Spend
* Footfall
* Average Discount Percentage
* Staff Count
* Inventory Availability Percentage
* Competitor Distance
* Holiday Flag
* Customer Rating
* Monthly Sales
* Monthly Profit

Total Records: 320

## Dependent Variable

* Monthly Sales

## Independent Variables

* Marketing Spend
* Footfall
* Inventory Availability Percentage
* Customer Rating
* Average Discount Percentage
* Staff Count
* Competitor Distance
* Holiday Flag
* Region
* Store Type

## Data Preparation

Missing values in Customer Rating and Competitor Distance were replaced using median imputation.

Dummy variables were created for the Region variable.

Reference Category: East

Dummy Variables:

* Region North
* Region South
* Region West

## Regression Approach

Three models were developed:

1. Simple Regression using Marketing Spend
2. Simple Regression using Footfall
3. Multiple Regression using Marketing Spend, Footfall, Inventory Availability Percentage, and Region North

## Model Comparison Summary

| Model               | R-Squared |
| ------------------- | --------- |
| Marketing Spend     | 0.167     |
| Footfall            | 0.736     |
| Multiple Regression | 0.805     |

The multiple regression model achieved the highest explanatory power.

## Final Model Selected

Multiple Regression Model

Variables:

* Marketing Spend
* Footfall
* Inventory Availability Percentage
* Region North

## Business Recommendation

Footfall, marketing spend, and inventory availability are the strongest predictors of monthly sales. Leadership should prioritize actions that increase store traffic, maintain inventory availability, and optimize marketing investments.

## Assumptions and Limitations

* Regression identifies association, not causation.
* Important business factors may not be included in the dataset.
* Results are based on historical data.
* Regional effects may be influenced by other unobserved factors.

## Screenshots Included

* simple_regression_output.png
* multiple_regression_output.png
* residuals_preview.png
* model_comparison_preview.png
