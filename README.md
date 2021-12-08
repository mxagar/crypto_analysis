# Crytocurrency Analysis

This respository contains the analysis of price and network data related to Bitcoin and other cryptocurrencies. I made the repository just for fun; no investment purposes nor advice intended here.

This project is on-going, not finished.

## How to use the repository

First, install [Anaconda](https://anaconda.org) and get required dependencies:
```bash
# Create your env, if you require a new one
# Install all necessary packages
# TBD
```
## Contents

The folder `data/` contains all the raw data used for the anaylsis.
These data is not uploaded to the repository;
you need to contact me if you would like access to it.

The repository contains the following notebooks:

- `00_DataPreparation.ipnb`: raw datasets in `./data` are pre-processed; these are related to BTC, ETH, XMR, and the global crypto market. Also, several **APIs are tested, but not really used yet: Quandl, Coinmarketcap, Google Trends Unofficial, Coingecko.**
- `01_BitcoinAnalysis.ipnb`: price level anaylsis of BTC in different halving cycles, support polynomial computation, comparisons of BTC to ETH and SPY (scatterplots, regressions, histograms, etc.).
- `02_PortfolioAnalysis.ipnb`: Monte Carlo simulations are performed to compute the optimum portfolio allocation (BTC, ETH, XMR) following the Markowitz method. The optimum portfolio has the highest Sharpe ratio and it is on the efficient frontier. 
- `03_CryptoCAPM.ipnb`: the `alpha` (intercept) and `beta` (slope) of BTC and ETH returns are computed with respect to the global crypto market returns performing simple linear regressions. According to CAPM, `alpha` should tend to `0`, but hedge funds try to choose assets with high `alpha` values and low `betas` to hedge their gains.


## Interesting links to get data from

- [https://1ml.com/statistics?json=true](https://1ml.com/statistics?json=true)
- [www.cryptodatadownload.com](https://www.cryptodatadownload.com/data/bitstamp/)
- [https://trends.google.com/trends/](https://trends.google.com/trends/)