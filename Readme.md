## Answer:

####Requirements:

- Python 3.7
- tbats(`pip install tbats`)
- statsmodels(`pip install tbats`)

#### Step1:

I inspected the data in three different aspects before we can explore it:

- Station_id and stationname matching
- Missing value
- Duplicates

####Step2:

- After visualizing the data, I found different stations' data had different time-series patterns. So I analyzed data and build model separately. For the rest of my work, I use station 'UIC-Halsted' as an example.
- After decompsing the data, I found that the data had both the weekly and yearly seasonality.

####Step3:

- Based on the data we have, the model we used should be able to deal with time series containing multiple seasonal effects. This is something TBATS was designed for.
- After fitting the model with data from 2002 to 2016, I further evaluated the model with data in 2017 with metrics MSE and RMSE.
- Based on all my results, TBATS seems to have done a pretty good job in modeling both of seasonal effects and therefore can help transportation department to improve service in the next few years.