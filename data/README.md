# Data for Cryptocurrency Analysis

## Cryptocurrency price data

Data was originally downloaded from [www.cryptodatadownload.com](https://www.cryptodatadownload.com):

```bash
# First line needs to be removed; after that, the CSV files have the following header:
# unix,date,symbol,open,high,low,close,Volume BTC,Volume USD
curl https://www.cryptodatadownload.com/cdd/gemini_BTCUSD_2016_1min.csv > data/Gemini_BTCUSD_2016_minute.csv
...
curl https://www.cryptodatadownload.com/cdd/Bitstamp_BTCUSD_2017_minute.csv > data/Bitstamp_BTCUSD_2017_minute.csv
...
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2017_minute.csv > data/Bitstamp_ETHUSD_2017_minute.csv
...
curl https://www.cryptodatadownload.com/cdd/Bitstamp_ETHUSD_2017_minute.csv > data/Bitstamp_ETHUSD_2017_minute.csv
...
curl https://www.cryptodatadownload.com/cdd/Binance_XMRUSDT_1h.csv > Binance_XMRUSDT_1h.csv
curl https://www.cryptodatadownload.com/cdd/Binance_XMRUSDT_d.csv > Binance_XMRUSDT_d.csv
curl https://www.cryptodatadownload.com/cdd/Binance_XMRUSDT_minute.csv > Binance_XMRUSDT_minute.csv
```

Note that you can search for different exchange data in the menu `Historical Data`.

After doownloading the files, the first line needs to be removed! One way of solving that through the command line is:
```bash
tail -n +2 "$FILE" > "$FILE.tmp" && mv "$FILE.tmp" "$FILE"
# Or
tail -n +2 "Binance_XMRUSDT_1h.csv" > "Binance_XMRUSDT_1h.csv.tmp" && mv "Binance_XMRUSDT_1h.csv.tmp" "Binance_XMRUSDT_1h.csv"
```

Note that some datasets have missing values for given time perdiods.

## Google Trends data

These data needs to be downloaded manually by clicking on the GUI: [https://trends.google.com/trends/](https://trends.google.com/trends/).
Make sure that:
- The correct region is chosen (e.g., Worldwide)
- The datapoint frequency (e.g., every day) is correct for your selected period

For daily data, the periods I needed to take each year were: 20XX-01-01 - 20XX-08-31 and 20XX-08-31 - 20XY-01-01 (Y=X+1); note that the first and final dates need to overlap so that a bigger dataset is created by concatenating the files and scaling the interest values accordingly.