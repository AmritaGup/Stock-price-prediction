# Stock-price-prediction
Forecasting Stock Prices of a selected company/organisation using ARIMA.

#ARIMA.py can be imported as pd by following instruction:
from ARIMA import Predict as pd
obj = pd(stock = <stock_name>, st=<starting date>)

#using different methods of 'Predict' class via an object:
ts_data = obj.get_data()
cp_fig = obj.visualize_data(ts_data)
obj.stationarize_data(ts_data)
fc, datelist = obj.forecast(period=<period for forecasting>)
path = obj.save_fig()
