# Customer Lifetime Value Analysis and Future Spending Prediction

## Project Overview

This project focuses on Customer Lifetime Value (CLV) analysis and future spending prediction using customer behavior data.

The objective of the project is to help businesses:
- understand customer value
- identify high-value customers
- predict future spending
- improve customer retention
- optimize marketing strategies
- increase long-term profitability

The project includes:
- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Customer Segmentation
- Regression Modeling
- Future Spending Prediction
- Business Recommendations


# Business Problem

Customer acquisition is expensive, so businesses aim to maximize revenue from existing customers.

Customer Lifetime Value (CLV) measures the long-term value a customer brings to the company.

Understanding customer value helps businesses:
- improve retention
- personalize offers
- optimize marketing spending
- increase repeat purchases

Future spending prediction allows businesses to:
- identify customers likely to spend more
- prioritize valuable customers
- improve upselling strategies
- reduce customer churn risk


# Dataset Description

The dataset contains customer demographic, behavioral, and spending information.

Each row represents one customer.

## Dataset Columns

| Column | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Age | Customer age |
| AnnualIncome | Customer yearly income |
| WebsiteVisits | Number of website visits |
| AppSessions | Number of app sessions |
| PreviousOrders | Total previous orders |
| AverageOrderValue | Average order value |
| DaysSinceLastPurchase | Number of days since last purchase |
| ReturnRate | Product return rate |
| CancellationRate | Order cancellation rate |
| LoyaltyTier | Customer loyalty category |
| DiscountUsedLastCampaign | Whether discount was used |
| Year1Spending | Previous customer spending |
| FutureSpending | Target variable |


# Business Understanding

## What is Customer Lifetime Value (CLV)?

Customer Lifetime Value represents the total expected value a customer generates throughout their relationship with the business.

## Why CLV is Important

Increasing CLV helps businesses:
- increase profitability
- improve retention
- reduce acquisition costs
- improve long-term growth

## Why Existing Customers Matter

Retaining existing customers is usually more cost-effective than acquiring new customers.

Existing customers:
- already trust the brand
- purchase more frequently
- are easier to upsell

## Why Future Spending Prediction is Useful

Predicting future spending helps businesses:
- identify valuable customers early
- personalize offers
- improve customer engagement
- optimize marketing campaigns


# Data Cleaning Summary

The dataset was checked for:
- missing values
- duplicates
- data type issues
- outliers

## Cleaning Steps Performed

- Removed duplicate rows
- Filled missing values in AnnualIncome using median
- Filled missing values in AverageOrderValue using median
- Verified numerical and categorical data types

The dataset was relatively clean and suitable for machine learning analysis.


# Feature Engineering Summary

Several business-focused features were created:

| Feature | Purpose |
|---|---|
| TotalEngagement | Measures total digital engagement |
| SpendingGrowth | Difference between future and previous spending |
| SpendingGrowthRate | Relative growth in spending |
| OrderIntensity | Purchase frequency measure |
| NetEngagementScore | Overall engagement score |

These features helped improve customer understanding and prediction performance.


# Exploratory Data Analysis (EDA)

EDA was performed to analyze:
- customer spending patterns
- customer engagement
- relationships between features
- customer value distribution
- future spending behavior


# Key EDA Insights

## Spending Distribution

- Most customers fall within moderate spending ranges.
- A smaller group of customers contributes very high revenue.
- Spending distributions are positively skewed.

## Previous Spending vs Future Spending

The analysis showed a very strong positive relationship between Year1Spending and FutureSpending.

Customers who spent more previously are highly likely to spend more in the future.

## Orders vs Future Spending

Customers with higher order counts generally showed higher future spending.

This suggests that repeat purchase behavior strongly influences customer value.

## Engagement Analysis

Website visits and app sessions showed moderate relationships with future spending.

Highly engaged customers tend to spend more over time.

## Loyalty Tier Analysis

Platinum and Gold customers generally showed higher future spending compared to lower loyalty tiers.

## Correlation Heatmap Insights

The heatmap showed:

- Strong positive correlation between Year1Spending and FutureSpending
- Strong relationship between PreviousOrders and FutureSpending
- Strong relationship between TotalEngagement and NetEngagementScore

These features are highly important for future spending prediction.


# Customer Segmentation Summary

Customers were segmented into meaningful business groups using spending, engagement, and recency behavior.

## Segments Created

| Segment | Description |
|---|---|
| High-Value Customer | High spending and loyal customers |
| Medium-Value Customer | Moderate spending customers |
| Low-Value Customer | Low spending customers |
| High-Potential Customer | Highly engaged customers with growth potential |
| Low-Engagement Customer | Low activity customers |
| At-Risk Valuable Customer | Valuable customers with declining activity |


# Segment Insights

## High-Value Customers
- generate the highest revenue
- show strong spending consistency
- should receive premium treatment

## High-Potential Customers
- highly engaged
- strong growth opportunities
- suitable for upselling

## At-Risk Valuable Customers
- historically valuable
- reduced recent activity
- require re-engagement campaigns

## Low-Engagement Customers
- low activity and low spending
- less suitable for expensive campaigns


# Regression Model Summary

Two regression models were built:

- Linear Regression
- Decision Tree Regressor

The models were trained using customer behavior and spending features to predict FutureSpending.


# Model Evaluation Results

The models were evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

## Key Findings

- Both models achieved very high R² scores.
- Linear Regression performed extremely well due to the strong relationship between Year1Spending and FutureSpending.
- The Actual vs Predicted plot showed predictions closely aligned with actual values.


# Feature Importance Analysis

The most important predictive features were:

1. Year1Spending
2. SpendingGrowth
3. SpendingGrowthRate
4. WebsiteVisits

This indicates that historical spending behavior is the strongest predictor of future customer value.


# Business Recommendations

## Premium Offers

High-Value Customers should receive:
- exclusive rewards
- VIP membership benefits
- personalized premium offers

## Upselling Opportunities

High-Potential Customers should receive:
- personalized recommendations
- upselling campaigns
- loyalty upgrade incentives

## Re-Engagement Strategies

At-Risk Valuable Customers should receive:
- retention campaigns
- targeted discounts
- personalized communication

## Discount Strategies

Low-Value Customers can receive:
- limited discounts
- entry-level promotional offers

## Avoid Expensive Campaigns

Low-Engagement Customers should not receive expensive acquisition or premium campaigns unless engagement improves.


# LTV Growth Strategy

The company can improve overall Customer Lifetime Value by:

- increasing repeat purchases
- improving customer engagement
- reducing return and cancellation rates
- rewarding loyal customers
- targeting customers based on behavior
- improving personalized marketing


# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

# Conclusion

This project successfully analyzed Customer Lifetime Value and predicted future customer spending using regression models.

The analysis demonstrated that:

historical spending
order frequency
engagement behavior

are strong indicators of future customer value.
The project provides practical strategies for customer retention, upselling, engagement improvement, and long-term revenue growth through data-driven customer analytics.