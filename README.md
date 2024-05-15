# Predictive Analysis on Revenue Per Available Room (RevPAR)

## Overview

This project aims to develop a predictive model to forecast the Revenue per Available Room (RevPAR) for Airbnb listings in Dallas, Texas. By leveraging historical data and machine learning techniques, we aim to empower hosts with actionable insights to optimize their pricing strategies and improve their overall performance.

## Problem Statement

The core of our project is to develop a predictive model using the Airbnb Dallas dataset. Our objective is clear: to empower hosts with actionable insights for informed decisions and proactive adjustments. By accurately predicting the Revenue per Available Room (RevPAR), we aim to enable hosts to fine-tune their strategies for maximum efficiency and profitability.

## Objectives

- **Empower hosts**: Provide hosts with actionable insights for informed decisions.
- **Optimize strategies**: Enable hosts to optimize their pricing and availability strategies.
- **Predict RevPAR**: Accurately predict Revenue per Available Room to enhance profitability.

## Dataset Description

The dataset contains comprehensive information on Airbnb listings, hosts, and their performance metrics. Key attributes include:

- **Host and Property Identifiers**: Unique IDs for Airbnb hosts and properties.
- **Location Details**: City, neighborhood, census tract details, and geographic coordinates (latitude and longitude).
- **Listing Characteristics**: Property type (e.g., apartment, house), listing type (e.g., entire home, private room), number of bedrooms and bathrooms, maximum guest capacity, and amenities like pet allowance and instant booking.
- **Pricing and Availability**: Nightly rates, cleaning fees, minimum stay requirements, and booking details for current and previous periods.
- **Superhost Status**: Tracks the Superhost status of hosts across different periods.
- **Performance Metrics**: Reviews, ratings, occupancy rates, and revenue generated, both current and historical.
- **Demographic Context**: Census tract data offering racial composition and total population.

## Key Attributes

- **Airbnb Host ID**: Unique identifier for the host.
- **Airbnb Property ID**: Unique identifier for the property/listing.
- **City_x**: City where the property is located.
- **superhost_period_all**: Evaluation period of this sample.
- **Scraped Date**: Date when the information was scraped.
- **host_is_superhost_in_period**: Indicator if the host was a superhost during this period.
- **prev_host_is_superhost_in_period**: Indicator if the host was a superhost in the previous period.
- **rating_ave_pastYear**: Average rating of the listing over the past year.
- **numReviews_pastYear**: Number of reviews for the host over the past year.
- **numCancel_pastYear**: Number of cancellations for the host over the past year.
- **num_5_star_Rev_pastYear**: Number of 5-star reviews received in the past year.
- **prop_5_StarReviews_pastYear**: Proportion of reviews that were 5 stars in the past year.
- **available_days**: Number of days the listing is available for booking.
- **booked_days**: Number of days the listing is booked in the evaluation period.
- **available_days_aveListedPrice**: Average listed price for available days.
- **booked_days_avePrice**: Average booking price for booked days.
- **Property Type**: Type of property (e.g., apartment, house).
- **Listing Type**: Type of listing (e.g., entire home, private room).
- **Zipcode**: Postal code of the property's location.
- **Bedrooms**: Number of bedrooms in the property.
- **Bathrooms**: Number of bathrooms in the property.
- **Max Guests**: Maximum number of guests the property can accommodate.
- **Cleaning Fee (USD)**: Fee charged for cleaning services in US dollars.
- **Minimum Stay**: Minimum number of nights a guest must book.
- **Number of Photos**: Total number of photos associated with the property listing.
- **Latitude**: Geographical latitude coordinate of the property.
- **Longitude**: Geographical longitude coordinate of the property.
- **Pets Allowed**: Indicator if pets are allowed in the property.
- **Instantbook Enabled**: Indicator if instant booking is enabled for the property.

## Methodology

1. **Data Collection and Cleaning**:
   - Aggregated data at host level for each evaluation period.
   - Handled missing values using imputation techniques based on median values.
   - Removed outliers based on statistical methods (e.g., boxplot, standard deviation).

2. **Data Preprocessing**:
   - Feature selection to identify primary and secondary features.
   - Data transformation including log transformation to normalize data.

3. **Model Training**:
   - Applied linear and polynomial regression models.
   - Validated models using train/test split and evaluated their performance.

4. **Model Validation**:
   - Assessed models based on R-squared value and other performance metrics.
   - Selected the best-performing model for prediction.

## Results

- The final model achieved an R-squared value of 79.43%, indicating a strong predictive power.
- Key features influencing RevPAR include average nightly rate, number of reviews, and overall rating.

## Implications

- **Operational Efficiency**: Hosts can identify peak and off-peak periods to optimize resource allocation.
- **Pricing Strategy Optimization**: Insights into demand patterns enable dynamic pricing adjustments.
- **Occupancy Rate Insights**: Understanding property utilization helps maintain high occupancy rates.
- **Predictive Maintenance**: Accurate revenue predictions allow better planning for maintenance and upgrades.
- **Competitive Analysis**: Benchmarking performance against market trends aids in strategic decision-making.

