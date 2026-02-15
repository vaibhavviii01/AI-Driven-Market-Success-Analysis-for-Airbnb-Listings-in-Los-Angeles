
# Analyzing the Los Angeles Airbnb Market (Post-COVID)

## Project Overview
This project provides a data-driven analysis of the home-sharing economy in Los Angeles between 2022 and 2023.This project analyzes the post-COVID landscape of the Airbnb market in Los Angeles, focusing on price forecasting and identifying the "Success DNA" of top-performing listings. Based on the data from October 2022 to September 2023, the analysis combines linear trend modeling with geospatial insights to predict future market shifts. It addresses two primary objectives:

**Market Forecasting:** Predicting the future of nightly prices and supply trends in LA.

**Success Optimization:** Identifying the characteristics that distinguish "winner" listings (top 7.8%) from the rest of the market.

## Key Insights

### 1. Market Trends & Forecasting

**Price Momentum:** Average nightly prices rose from $196 in Q4 2022 to $213 in Q3 2023.

**Future Projections:** Using a linear trend model, prices are forecasted to reach approximately **$234 by Q3 2024**, growing at a rate of ~$5.42 per quarter.

**Supply Growth:** Total listings increased by **10.28%** annually, though the growth is unevenly distributed across room types.

### 2. The "Success DNA" of LA Listings
The analysis identified a massive revenue gap: the top 7.8% of performers generate **$110k more annually** than standard listings, a 442% premium.

**Location:** Success is heavily tied to affluent coastal zones. Avalon (28.7% win rate) and Pacific Palisades (21.3%) significantly outperform the city average of 7.8%.

**Privacy Preference:** Entire homes are **7x more likely to succeed** than private rooms, reflecting a strong post-COVID preference for private spaces.

**Host Strategy:** "Focused Owners" (Single-listing hosts) actually earn higher average revenue ($42,779) than "Enterprise" hosts with 5+ listings ($30,386), suggesting quality beats quantity[cite: 490, 495].

## Methodology

**Data Cleaning:** Handled missing values, converted data types, and removed outliers from the 2022-2023 LA Listings dataset.

**Modeling:** Fit a linear trend model for forecasting and validated it against ARIMA/SARIMA time-series models.

**Geospatial Analysis:** Utilized LA's GeoJSON files to map price premiums and host activation scores by neighborhood.

## Model

The project includes 6 forecasting models:

**SARIMA:** Classical time series model

**Prophet:** Meta's forecasting framework

**LSTM:** Deep learning neural network

**XGBoost:** Gradient boosting for price/occupancy

**VAR/VECM**: Multi-variable time series

**Ensemble:** Combined model (best performance)

**Best Model:** Ensemble achieves 2.87% MAPE on 4-quarter forecasts.

## Tools Used
* Python (Pandas, Matplotlib, Seaborn)
* Time-Series Forecasting (Linear Regression, ARIMA)
* Geospatial Mapping

## Confidentiality & Data Privacy
Due to the sensitive nature of the underlying data and project requirements, the full source code for data processing and modeling is not publicly disclosed in this repository.
