# Time Series Analysis on Tea Production

This project applies time series modeling to forecast the Nett Sale Average (Rs) of tea over time, using historical production and sales data. The core objective is to support strategic planning, revenue forecasting, and pricing decisions for tea-producing companies.

The SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors) model is used to capture trends, seasonality, and the influence of external market indicators.

📁 Dataset Description

The dataset contains historical records of tea production, processing, and pricing. Below is a brief explanation of each feature:

| Column                   | Description                                                                     |
| ------------------------ | ------------------------------------------------------------------------------- |
| `Date`                   | The date of each observation (Monthly).                                         |
| `GREEN LEAF (Kg)`        | Raw green leaf volume collected (input to processing).                          |
| `MADE TEA (Kg)`          | Final processed tea output in kilograms.                                        |
| `NETT OUT TURN`          | Conversion efficiency: Made Tea as a percentage of Green Leaf.                  |
| `NETT SALE AVERAGE (Rs)` | The average price per kg of made tea sold. **Target variable** for forecasting. |
| `LOW GROWN AVERAGE (Rs)` | Industry benchmark price for low-grown teas.                                    |
| `DIFFERENCE (Rs)`        | Difference between company price and market average.                            |
| `BOUGHT LEAF RATE (Rs)`  | Price paid per kg for externally purchased green leaf.                          |

📈 Forecasting Model: SARIMAX
The project uses the SARIMAX model to forecast the NETT SALE AVERAGE (Rs) based on:

Its own historical values.
Seasonality patterns (e.g., monthly cycles).
Exogenous variables: such as LOW GROWN AVERAGE (Rs) and BOUGHT LEAF RATE (Rs).

The model helps:

Anticipate market fluctuations.
Estimate future sales performance.
Improve decision-making on pricing and operational efficiency.

📦 Features

Time series decomposition and visualization.
Stationarity testing (ADF Test).
SARIMAX modeling with hyperparameter tuning.
Forecast generation with confidence intervals.
Forecast performance evaluation (MAE, RMSE).
Optional inclusion of exogenous variables.

