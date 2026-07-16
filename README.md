interpretable German Electricity Demand Forecasting
Overview

This project examines whether Elastic Net can provide competitive electricity-demand forecasts while keeping its predictive relationships understandable.

Data
German hourly electricity demand from 2015 to 2020
Weekly aggregation
Berlin temperature
German holidays and working days
195 training weeks and 104 testing weeks
Models
Seasonal Naive
Elastic Net
SARIMA
SARIMAX
Rolling hourly LSTM
Main Features
Load lags: 1, 2, 4, 13, 26 and 52 weeks
Shifted rolling means and standard deviations
Temperature, heating and cooling degree days
Holidays and working days
Seasonal sine and cosine terms
Time trend
Main Libraries
pandas
numpy
matplotlib
statsmodels
scikit-learn
tensorflow
requests
holidays
Installation
pip install pandas numpy matplotlib statsmodels scikit-learn tensorflow requests holidays
How to Run
Open the notebook in Jupyter or Google Colab.
Install the required libraries.
Run all cells in order.
Keep internet access enabled for demand and temperature retrieval.
Review the generated forecasts, coefficients, diagnostics and metric tables.
Main Result

Seasonal Naive achieved the best comparable weekly RMSE of 2,988.25 MW. Elastic Net achieved 3,575.28 MW, outperforming SARIMA and SARIMAX while providing ten interpretable non-zero coefficients.
