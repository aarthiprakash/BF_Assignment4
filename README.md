# BF_Assignment4 - Answers

- The time series used is quarterly values of the total net patient revenue at Alameda Hospital in California.

1) You will try the different models we ran in class today on your dataset.  (2 points)
- ACF plot, Mean Forecase, Naive Forecast, Random Walk Forecast, Seasonal Naive Forecast, Moving Average Forecast for 4 and 8 window, Exponential Smoothing, HOlts-Winters have been run on my dataset. 

2) Understand and Explain your model output (4 points)
- ACF plot shows that there is no seasonality or trend. None of the data points are statistically significant.
- The mean forecast takes mean of all history and plots a forecast of 1 value at around $19,000,000. MAPE was 8.590105 as baseline
- The naive forecast shows the same value as the mean forecast but with expanded confidence intervals. MAPE was 9.257945 and not better than mean forecast.
- The random walk forecast adds some drift/noise to what the naive forecast is showing. MAPE was 9.592681 and not better than the mean forecast.
- The seasonal naive forecast is showing a slight curve for 3 quarters and a large drop. MAPE was 11.94603 and not better than the mean forecast.
- The moving average forecasts (4 and 8 quarter intervals) shows a smoother curve forming of the total net patient revenue values. 
- The ETS forecast shows that the patient revenue for the next 4 quarters will be the same, similar to the mean forecast but it shows that the value is a little less at around $185,000,000. MAPE was 9.049191 and not better than the mean forecast.
- The Holt-Winters forecast shows similar forecasted values as the ets forecast but this is expected because the data does not have trend or seasonality to it. MAPE was 7.210746 and better than the mean forecast.

3) Plot the time series and different model forecasts in one chart (2 points).
- Time series data and different model forecasts are in 1 plot. Please see the html rendering.
  
4) Pick an accuracy measure, compare your models, and state the best model based on the accuracy comparison (2 points)
- I chose MAPE = Mean Absolute Percentage Error
- MAPE for Mean Forecast was 8.590105 as baseline.
- MAPE for Naive Forecast was 9.257945 and not better than mean forecast.
- MAPE for Random Walk Forecase was 9.592681 and not better than the mean forecast.
- MAPE for Seasonal Naive Forecast was 11.94603 and not better than the mean forecast.
- MAPE for ETS Forecast was 9.049191 and not better than the mean forecast.
- MAPE for Holt-Winters Forecast was 7.210746 and better than all of the other forecast methods. Based on the accuracy comparison, the Holt-Winters forecast is the best model for this data.
  
