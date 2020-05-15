# tickrtape
Github for pypi package tickrtape

**Website** [tickrtape](http://www.tickrtape.co)

# Usage and Installation
Installation
```bash
pip install tickrtape
```

Pulling data
```bash
import tickrtape as tt

start = '2020-04-06 9:45:00'
end = '2020-04-06 10:45:00'
key = #personal api key
ticker = 'AAPL'

prices = tt.pull(key, ticker, start, end)
[
[date, time, open, high, low, close, volume],
[date, time, open, high, low, close, volume],
.
.
.
]
```

Stock Availability
```bash
import tickrtape as tt

cov = tt.coverage('AAPL')
print(cov) #'minutely data exceeding 30 days'
```