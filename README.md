# Crytocurrency Analysis

This repository contains the analysis of price and network data related to Bitcoin and other cryptocurrencies. I made the repository just for fun; no investment purposes nor advice intended here.

:construction: This project is on-going, not finished.

## How to use the repository

First, install an environment manager, e.g., [conda](https://docs.conda.io/en/latest/), create an environment and install the required dependencies:

```bash
# Create your env
conda create --name crypto pip python=3.6
conda activate crypto

# Install all necessary packages
# FIXME: Many packages can be removed
pip install -r requirements.txt
```

Then, open the [notebooks](#notebooks), sequentially.

## Notebooks

The folder `data/` contains all the raw data used for the analysis. These data is not uploaded to the repository; you need to contact me if you would like access to it.

The repository contains the following notebooks:

- [`00_DataPreparation.ipynb`](00_DataPreparation.ipynb): raw datasets in `./data` are pre-processed; these are related to BTC, ETH, XMR, and the global crypto market. Also, several APIs are tested, but not really used yet: Quandl, Coinmarketcap, Google Trends Unofficial, Coingecko.
- [`01_BitcoinAnalysis.ipynb`](01_BitcoinAnalysis.ipynb): price level anaylsis of BTC in different halving cycles, support polynomial computation, comparisons of BTC to ETH and SPY (scatterplots, regressions, histograms, etc.).
- [`02_PortfolioAnalysis.ipynb`](02_PortfolioAnalysis.ipynb): Monte Carlo simulations are performed to compute the optimum portfolio allocation (BTC, ETH, XMR) following the Markowitz method. The optimum portfolio has the highest Sharpe ratio and it is on the efficient frontier. 
- [`03_CryptoCAPM.ipynb`](03_CryptoCAPM.ipynb): the `alpha` (intercept) and `beta` (slope) of BTC and ETH returns are computed with respect to the global crypto market returns performing simple linear regressions. According to CAPM, `alpha` should tend to `0`, but hedge funds try to choose assets with high `alpha` values and low `betas` to hedge their gains.


## Interesting links to get data from

- [https://1ml.com/statistics?json=true](https://1ml.com/statistics?json=true)
- [www.cryptodatadownload.com](https://www.cryptodatadownload.com/data/bitstamp/)
- [https://trends.google.com/trends/](https://trends.google.com/trends/)

## Authorship

Mikel Sagardia, 2020.  
No guarantees.

Check the [`LICENSE`](LICENSE).
