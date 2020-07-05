# Crypto Analyzer 
Check out the [link](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/CryptoAnalysis_1.0_D.ipynb )  for code. (Code will not work because [cryptocompare](cryptocompare.com) bas changed the free-API endpoints since the code's implementation.)


I [**formulated and prioritised requirements**](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/CryptoAnalysis_1.0_D.ipynb#TO-DO:), built a low-frequency cryptocurrency trading system using the [CCXT API](https://github.com/ccxt/ccxt) and [cryptocompare API](https://min-api.cryptocompare.com/). 
A **single interface** was created to [download market data from different cryptocurrency exchanges](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/CryptoAnalysis_1.0_D.ipynb#TO-DO:), thereby avoiding duplication of code.)

Level-1 order book data and multiple time-frame data
(1-hour,4-hour,12-hour and 24-hour data) were analysed together to spot trending and high volume cryptocurrencies. 

Used Technical Analysis libraries such as [Ta-Lib](https://mrjbq7.github.io/ta-lib/doc_index.html) and [Pyti](https://github.com/kylejusticemagnuson/pyti/tree/master/pyti). 
Added Cron-Jobs which would periodically download market data from the exchange API. 

[**Re-sampled data**](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/CryptoAnalysis_1.0_D.ipynb#Resample-high-frequency-data(1m,15m,etc)-to-low-frequncy-data(1day,1week,1month,etc)) to generate weekly and monthly price trends. 

[Automated the data download and the technical analysis parts.](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/CryptoAnalysis_1.0_D.ipynb#Since-Crypto-Markets-are-24-hours,-the-current-candle-may-be-incomplete,until-the-candle-is-closed.-So-delete-the-last-row-for-each-coin-exchange-time_period-combination-and-download-OHLCV-data-from-the-last-row-in-the-CSV/table-after-deletion-to-the-current-timestamp.)

Formed trading rules using [technical indicators,past trades and order book](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/Order_Book_and_Past_Trade_Analysis_D.ipynb) such as Moving Averages(Moving Averages Cross-Over technique), Relative Strength Index(RSI) to spot trending patterns and Bollinger Bands to spot mean-reverting patterns.

I also experimented with intra-day trading (wrote code to spot mean-reverting prices) using [Bollinger Bands and WebSocket Real Time Code](https://nbviewer.jupyter.org/github/ankit-a-aggarwal/crypto-analysis/blob/master/notebooks/BTC_USD_Streaming_D.ipynb?flush_cache=true)

