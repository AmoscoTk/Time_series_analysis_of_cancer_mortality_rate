## Time_series_analysis_of_cancer_mortality_rate


## Time Series Analysis & Forecasting of Cancer Mortality Rates in the USA

 # A project for analyzing historical trends in cancer mortality across U.S. states, applying time series methods, and forecasting future rates. 


# Overview

This repository implements a time series analysis of cancer mortality data across the U.S., using statistical and forecasting methods to:
	•	Identify trends, seasonality, and structural shifts in mortality rates
	•	Fit appropriate time series models (ARIMA, AR, MA)
	•	Evaluate model performance
	•	Forecast future mortality rates
	•	Visualize results (time plots, forecast bands, residual analysis)


# Repository Structure


├── Data/                   # Raw & cleaned data files (e.g. CSVs, preprocessed datasets)
├── Visuals/                # Plots, charts, model diagnostics, forecast plots
├── Project.gretl           # Example script / model file (if using Gretl)
├── Reference.pdf           # Background, literature, data documentation
├── Amos Tochukwu Ezeh.pdf  # (Author or report file)
├── LICENSE                 # MIT License
└── README.md               # This file



# Usage & Workflow

Here’s how someone can use or reproduce your analyses:
	1.	Get the data
Place the raw / cleaned cancer mortality data (e.g. CSV) into the Data/ folder.
	2.	Preprocess (if needed)
Run scripts (in R, Python, Gretl, etc.) to clean, transform, or aggregate the time series.
	3.	Explore trends & diagnostics
	•	Plot time series for overall USA and by state
	•	Check stationarity (e.g. ADF test, KPSS)
	•	Examine autocorrelation / partial autocorrelation
	4.	Fit models
	•	ARIMA, seasonal ARIMA
	•	Exponential smoothing (ETS)
	•	Other candidate models (e.g. vector autoregressive, structural time series)
	5.	Evaluate & compare
Use metrics such as RMSE, MAE, AIC, residual diagnostics, Ljung-Box test, etc.
	6.	Forecasting
Generate out-of-sample forecasts with confidence intervals.
Visualize the forecasted trajectories and compare with hold-out test sets.
	7.	Visualization & interpretation
Plot data + fits + forecasts, residual diagnostics, error distributions, etc.



# Example Highlights & Insights
	•	Long-term trend in cancer mortality rates: increasing, plateauing, or declining?
	•	Presence (or absence) of structural breaks (e.g. due to medical advances, policy changes)
	•	Forecasts with uncertainty bands — what range of mortality rates is plausible in the next 5–10 years
	•	Model diagnostics: residual checks, autocorrelation in residuals, overfitting avoidance
	
⸻

# Technical / Modeling Details

Here are some key modeling and design choices:
	•	Stationarity / differencing: whether to difference the series (and degree)
	•	AR / MA orders: selected via AIC / BIC / grid search
	•	Seasonality: if seasonal patterns are present (e.g. yearly cycles)
	•	Model selection criteria: AIC, BIC, cross-validation on hold-out sets
	•	Residual checks:
	•	Autocorrelation / partial autocorrelation
	•	Ljung-Box test
	•	Normality (e.g. QQ plots)
	•	Forecast horizon: how far ahead you forecast (e.g. 5, 10 years)
	•	Confidence intervals: how wide are your prediction bands


# Dependencies & Environment

List what software, 
	•	Gretl 
	•	Microsoft Excel



📃 License & Contributions

This repository is released under the MIT License, allowing reuse, modification, and distribution (with attribution).
Contributions, improvements, bug fixes, and extensions are warmly welcome — feel free to open issues or pull requests.
