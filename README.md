# Ydata
Download stock symbol historical data from yahoo finance in a json format (dictionary) beginners friendly.

``` python
from ydata import Ydata
# The first parameter is the stock symbol TSLA
yd = Ydata('TSLA')

Get historical data using yd.historical(initialDate,endDate)
historicalResp = yd.historical('2020-01-01','2020-02-01')
print(historicalResp)
