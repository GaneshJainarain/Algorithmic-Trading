# Trading Algo Pscode 

### Initialization
- Initialize tradeable stock list(S&P500 Stocks)
(By tradeable I mean the volume for the specific stock is above a certain constant value, volume is important for contracts with respect to Open Interests and Implied Volatility)
- Iterate through list of stocks:
    if stock is tradeable
    AND 

- For each Stock Ticker in our Tickerlist:
    Calculate Simple Moving Average 20
    Calculate Simple Moving Average 50
    Calculate Simple Moving Average 200
    Calculate RSI Value
        ''' if RSI val >= 70:
            Make a Put
        elif RSI val =< 30:
            Make a Call
        elif 30 =< RSI val =< 70:
            SendToInDepthAnalysis(StockTicker)
    Calculate MACD 
    '''






