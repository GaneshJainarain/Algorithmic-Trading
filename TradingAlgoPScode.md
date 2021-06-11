# Trading Algo Pscode 

### Initialization
- Initialize tradeable stock list(S&P500 Stocks)
(By tradeable I mean the volume for the specific stock is above a certain constant value, volume is important for contracts with respect to Open Interests and Implied Volatility)
- Iterate through list of stocks:
    if stock is tradeable
    AND 

- For each Stock Ticker in our Tickerlist we observe Indicators:
    Calculate Simple Moving Average 20
    Calculate Simple Moving Average 50
    Calculate Simple Moving Average 200
    Calculate RSI Value:
        if RSI val >= 70(Overbought Value):
            Make a Put OR Add +1 to Put counter PutCounter()
        elif RSI val =< 30(Oversold Value):
            Make a Call OR Add +1 to Call counter CallCounter()
        elif 40 =< RSI val =< 60:
            Stock is nominal/stagnant
    Calculate MACD 12,26,9:
        if MACD was previously negative AND crosses SIGNAL:
            buy Call or Flag that this is more of a reason to make a Call
        else if MACD was positive AND crosses SIGNAL:
            buy Put or Flag that this is more of a reason to make a Put  








