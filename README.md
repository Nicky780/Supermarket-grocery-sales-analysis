# Supermarket Grocery Sales Analysis

**Question:** Do discounts make the supermarket more money, and where should it focus?

## Data
9,994 grocery orders from Tamil Nadu, India (2015-2018): category, city, date,
sales, discount and profit. Source: <add link>. The data appears synthetic.

## Methods
- Data cleaning (two mixed date formats, constant column, quality checks)
- Feature engineering (margin, discount amount, time features)
- Group analysis by category, city and year
- OLS regression (Profit ~ Discount + Sales), implemented in matrix form
- Customer segmentation (K-Means) and a Random Forest profit model

## Key findings
- Overall margin: 25.05%
- Discount has no significant effect on profit (coefficient 10.78, p = 0.67)
- Margin is flat (~25%) across all discount bands (10-35%)
- Profit is driven by order size (correlation with Sales = 0.605)
- Sales grew 5%, 24% and 29% in 2016-2018

## Limitations
- `Region` labels are inconsistent (North has 1 order)
- Day-first order assumed for dash-format dates
- Data looks synthetic, so results may not reflect real retail behavior

## How to run
pip install -r requirements.txt
jupyter lab