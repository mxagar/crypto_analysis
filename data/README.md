# Data for Cryptocurrency Analysis

Minute data was originally downloaded from [www.cryptodatadownload.com](https://www.cryptodatadownload.com/data/bitstamp/):

```bash
# First line needs to be removed; after that, the CSV files have the following header:
# unix,date,symbol,open,high,low,close,Volume BTC,Volume USD
curl https://www.cryptodatadownload.com/cdd/Bitstamp_BTCUSD_2017_minute.csv > data/Bitstamp_BTCUSD_2017_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_BTCUSD_2018_minute.csv > data/Bitstamp_BTCUSD_2018_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_BTCUSD_2019_minute.csv > data/Bitstamp_BTCUSD_2019_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_BTCUSD_2020_minute.csv > data/Bitstamp_BTCUSD_2020_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_BTCUSD_2021_minute.csv > data/Bitstamp_BTCUSD_2021_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2017_minute.csv > data/Bitstamp_ETHUSD_2017_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2018_minute.csv > data/Bitstamp_ETHUSD_2018_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2019_minute.csv > data/Bitstamp_ETHUSD_2019_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2020_minute.csv > data/Bitstamp_ETHUSD_2020_minute.csv
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2021_minute.csv > data/Bitstamp_ETHUSD_2021_minute.csv
```
