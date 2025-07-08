# Time Series Analysis

### Characteristics
- collected at chronological order with timestamps (date and time)<br>
- shows trend over a long period of time <br>
- random variation (noise) is not explained <br>
- statistical properties (mean, variance) are constant over time - Test for Stationarity: Augmented Dickey-Fuller (ADF) test.<br><br>

examples: stock prices, temperature reading, website traffic, monthly sales, IoT sensor data analysis 

### COMPONENTS
- trend and seasonality
- repeating pattern
- irregular frequency (rise and fall)
- Random variation/noise

### Uses of Time Series Analysis

- forcasting:  predicting future temperature values
- classification:  predict if stock will go up/down (not exact value)
- anomaly detection:  detect unusual spikes (fraud / machine failure)

### Time Series Forecasting approach

0. Data Collection📥

1. Data Preprocessing ⚙️<br>
&nbsp;&nbsp;&nbsp;&nbsp;1.0 Sort Data chronologically<br>
    &nbsp;&nbsp;&nbsp;&nbsp;1.1 Handle Missings & duplicates<br>
    &nbsp;&nbsp;&nbsp;&nbsp;1.2 Smoothing data / Resampling<br>
    
2. Data visualization 📊
3. Feature engineering 🔧<br>
    &nbsp;&nbsp;&nbsp;&nbsp;3.0 Lag<br>
     &nbsp;&nbsp;&nbsp;&nbsp;3.1 Drop irrelevelant features<br>
4. Exploratory Data Analysis 📊<br>
    &nbsp;&nbsp;&nbsp;&nbsp;4.0 Autocorrelation Analysis<br>
    &nbsp;&nbsp;&nbsp;&nbsp;4.1 Encoding Cyclical Features<br>
    &nbsp;&nbsp;&nbsp;&nbsp;4.2 TimeSeries Decomposition<br>
    &nbsp;&nbsp;&nbsp;&nbsp;4.3 Stationarity<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.3.0 Augmented Dickey-Fuller (ADF)<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.3.1 Transforming<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.3.2 Differencing<br>
5. Train-Test Split: based on time
6. Modeling<br>
    &nbsp;&nbsp;&nbsp;&nbsp;6.0 Models for Univariate Time Series<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > MA, AR, ARIMA, SARIMA...ETC<br>
    &nbsp;&nbsp;&nbsp;&nbsp;6.2 Models for Multivariate Time Series<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > SARIMAX, VAR, VARMA, PROPHET...ETC<br>
7. Model Training🛠️<br>
&nbsp;&nbsp;&nbsp;&nbsp;7.0 Fit model with training dataset<br>
&nbsp;&nbsp;&nbsp;&nbsp;7.1 Predict/Forecast using testing data<br>
8. Model Evaluation📈<br>
&nbsp;&nbsp;&nbsp;&nbsp;8.0 Use various performance matrics to evaluate model accuracy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > mean absolute error (mae) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > mean squared error (mse)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > root mse (rmse)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > mean absolute percentage error (mape)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > AIC/BIC - EVALUATION: lowest == best<br>

9. Post-processing & Interpretation📦<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > Plot predicted vs actual sales<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > Apply business constraints (e.g., inventory caps)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > Convert predictions into actionable insights <br>
