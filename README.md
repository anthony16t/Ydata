Download stock symbol historical data from yahoo finance in a json format (dictionary) beginners friendly.

When initialize the module it will create the cache folder inside the module if it do not exists.
The cache folder it's use to cache data if that data was fetched on current day, it will make the script run faster since the data is already downloaded.

# Usage

``` python
from ydata import Ydata
# The first parameter is the stock symbol TSLA
yd = Ydata('TSLA')
```

# Get historical data
``` python
historicalResp = yd.historical('2020-01-01','2020-02-01')
print(historicalResp)
```

# Get current price
``` python
price = yd.currentPrice()
print(price)
```

# Get one week data
``` python
data = yd.oneWeek()
print(data)
```

# Get two weeks data
``` python
data = yd.twoWeeks()
print(data)
```

# Get two months data
``` python
data = yd.twoMonths()
print(data)
```