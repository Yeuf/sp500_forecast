# S&P 500 Index Forecasting
This Python script uses the Prophet library to forecast the S&P 500 index.

## Requirements
- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- ydata_profiling
- prophet

## Installation
To install the required libraries, run the following command:
```bash
pip install pandas numpy matplotlib seaborn ydata_profiling prophet
```
## Description
The script retrieves data on the S&P 500 index from a csv file and generates a profiling report for the data frame. It then uses the Prophet library to forecast the S&P 500 index and generates several visualizations of the data using matplotlib.

The script fits several Prophet models with different parameters and generates visualizations for each model:

A basic Prophet model with specified parameters:

- A line plot of the S&P 500 index over time
- A line plot of the forecasted values
- A plot of the components of the forecast (trend, holidays and yearly seasonality)
- A cross-validation metric (MAPE) over time horizon

A Prophet model with best parameters from grid search:

- A line plot of the forecasted values using best parameters
- A plot of the components of the forecast using best parameters (trend, holidays and yearly seasonality)
- A cross-validation metric (MAPE) over time horizon using best parameters

A Prophet model with best parameters from grid search and custom seasonality:

- A line plot of the forecasted values using best parameters and custom seasonality
- A plot of the components of the forecast using best parameters and custom seasonality (trend, holidays and yearly seasonality)
- A cross-validation metric (MAPE) over time horizon using best parameters and custom seasonality

A Prophet model with best parameters from grid search, custom seasonality and including covid lockdown as one time holidays:

- A line plot of the forecasted values using best parameters, custom seasonality and including lockdown information as holidays
- A plot of the components of the forecast using best parameters, custom seasonality and including lockdown information as holidays (trend, holidays and yearly seasonality)
- A cross-validation metric (MAPE) over time horizon using best parameters, custom seasonality and including lockdown information as holidays.
