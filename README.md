# Energy Demand Forecasting using ARIMA

This project provides a comprehensive analysis and forecasting solution for energy demand and solar energy generation using the ARIMA (AutoRegressive Integrated Moving Average) model. The workflow is implemented in a Jupyter Notebook, utilizing real-world time series data.

## Project Overview

The notebook walks through:
- Loading, visualizing, and preprocessing energy demand and solar generation data
- Handling missing values
- Testing for stationarity using the Augmented Dickey-Fuller test
- Building and evaluating ARIMA models for both energy demand and solar generation time series
- Comparing actual values with predicted values through plots and RMSE calculations

## Key Features

- **Data Cleaning:** Handles missing values using forward fill.
- **Visualization:** Multiple plots for exploratory data analysis.
- **Stationarity Check:** Uses ADF statistical test to assess stationarity before modeling.
- **ARIMA Modeling:** 
  - Parameter selection using ACF and PACF.
  - Model fitting and evaluation for both load and solar generation series.
  - Train/test split for robust performance estimation.
  - RMSE metric for quantitative evaluation.
- **Result Visualization:** Plots show actual vs. predicted values for intuitive comparison.

## Data

The notebook expects a CSV file named `TimeSeries_TotalSolarGen_and_Load_IT_2016.csv` with the following columns:
- `utc_timestamp`: Timestamps in ISO format
- `IT_load_new`: Energy load values
- `IT_solar_generation`: Solar generation values

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook

### Main Dependencies

Install requirements with:

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn
```

### Running the Notebook

1. Place your data file (`TimeSeries_TotalSolarGen_and_Load_IT_2016.csv`) in the repository directory.
2. Open and run the notebook:  
   `Energy Demand Forecasting using ARIMA.ipynb`

## Usage

The notebook is self-contained. Execute each cell sequentially to reproduce the analysis and results. The ARIMA model parameters (p, d, q) were determined based on the ACF/PACF plots and stationarity tests.

Typical workflow:
1. Load the data and handle missing values.
2. Visualize the time series.
3. Check for stationarity.
4. Plot ACF/PACF to select ARIMA parameters.
5. Train/test split and model fitting.
6. Evaluate predictions using RMSE and plots.

## Results

- The ARIMA models provide forecasts for both energy demand and solar generation.
- Performance is evaluated using Root Mean Squared Error (RMSE) and visual inspection of prediction plots.

## License

This project is for educational and research purposes. No license specified.

## Author

[Excalibuurr](https://github.com/Excalibuurr)
