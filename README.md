# NYC Taxi Demand and Pricing Forecasting

This project uses historical New York City taxi data to forecast demand and pricing patterns, helping drivers make more informed decisions about where and when to position themselves for the next ride. Developed as part of a University of Chicago Applied Data Science Time Series Analysis and Forecasting course.

## Overview

Taxi and for-hire vehicle drivers face significant uncertainty when deciding where to operate throughout the day. Poor positioning can lead to:

* Longer idle times
* Reduced earnings
* Increased fuel consumption

At a system level, inefficient driver movement contributes to:

* Traffic congestion
* Higher emissions in dense urban areas

**Goal:**
Use historical hourly New York City trip data to forecast:

* Average trip prices
* Pickup demand
* Airport-specific pickup demand

These forecasts can help drivers position themselves more strategically, improving efficiency and earnings.

## Data

### Taxi Trip Data

* **Source:** NYC Yellow Taxi data
* **Time Period:** January 2024 – November 2025

### Aggregation Level

* Hourly

### Key Variables

* Total number of trips
* Total airport trips
* Average trip charge

### Weather Data

Hourly weather conditions were incorporated to capture their impact on rider demand:

* Temperature (°C)
* Precipitation (mm)
* Wind speed (km/h)
* Rain (mm)
* Snowfall (cm)

Weather plays a key role in influencing both rider behavior and taxi demand.

### Gas Price Data

* **Source:** Daily NYC gasoline prices (DGASNY)

Gas prices serve as an external economic indicator that may affect:

* Driver supply decisions
* Operating costs
* Overall taxi availability

## Methodology

* Aggregated trip-level data into hourly time series
* Merged external datasets (weather and gas prices)
* Engineered features to capture temporal and environmental patterns
* Built forecasting models for:

  * Demand (total and airport trips)
  * Pricing (average fare)

## Use Case

The outputs of this project can be used to:

* Identify high-demand time periods
* Anticipate airport demand spikes
* Adjust driving strategies based on weather and cost conditions

## Impact

* Reduced idle time for drivers
* Improved earnings potential
* Lower fuel consumption
* Reduced congestion and environmental impact

## Future Work

* Incorporate real-time data streams
* Add spatial modeling (e.g., borough or zone-level forecasts)
* Explore advanced time series models (e.g., LSTM, Prophet)
* Build a driver-facing dashboard for live recommendations
