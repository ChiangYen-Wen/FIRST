##About Bollinger Bands(English Version):

1. Import necessary libraries:
   
    yfinance: Used to download historical stock data from Yahoo Finance.
   
    pandas: Used for data manipulation and creating DataFrames.
   
    matplotlib.pyplot: Used for plotting charts.
   
2. Download historical stock data:
   
    Use the Ticker function from yfinance to download historical data of TSMC (stock symbol:    2330.TW) from January 1, 2000, to March 19, 2024.(You can change what you want.)

3. Calculate Bollinger Bands:
   
    Compute the 20-day moving average (sma) and standard deviation (std) using rolling functions.
   
    Calculate the upper band (upper_band) and lower band (lower_band) based on the moving average and standard deviation.
   
4. Initialize trading variables:
   
    Initialize initial capital, position status, trading points, and other variables.

5. Iterate through stock data and execute trading strategy:
    
    If the stock price is below the lower band, execute a buy operation.
   
    If the stock price is above the upper band, execute a sell operation.
   
    Execute buy and sell operations based on the trading strategy, while updating the capital status and trading records.
   
6. Plot cumulative profit/loss curve:

    Use matplotlib.pyplot to plot the cumulative profit/loss curve over time.

7. If there are trading records, save them as a CSV file:
    
    Save the trading records as a DataFrame.
    
    Use the to_csv method to write the DataFrame into a CSV file, resolving any issues related to Chinese characters' encoding.
   
    This code aims to calculate the Bollinger Bands of a stock and execute trading strategies based on these bands, while also providing visualization and trading record functionalities.
 
##關於布林通道(中文版):

1. 引入必要的庫：

    yfinance：用於從 Yahoo Finance 下載股票歷史數據。
   
    pandas：用於處理數據和創建 DataFrame。
   
    matplotlib.pyplot：用於繪製圖表。

2. 下載股票歷史數據：
 
    使用 yfinance 中的 Ticker 函數下載台積電（股票代號：2330.TW）的歷史數據，時間從 2000 年 1 月 1 日到 2024 年 3 月 19 日。

3. 計算布林通道指標：

    使用滾動函數計算 20 天的移動平均線（sma）和標準差（std）。
   
    根據移動平均線和標準差計算上軌（upper_band）和下軌（lower_band）。

4. 初始化交易變數：

    初始化初始資金、持倉狀態、交易點等變數。
   
    遍歷股票數據，執行交易策略：

    如果股價低於下軌，則進行買入操作。
   
    如果股價高於上軌，則進行賣出操作。
   
    根據交易策略執行買入和賣出操作，同時更新資金狀態和交易記錄。

5. 繪製累計損益曲線圖：

    使用 matplotlib.pyplot 繪製隨時間的累計損益曲線圖。

6. 如果有交易記錄，將交易記錄保存為 CSV 文件：

    將交易記錄保存為 DataFrame。
   
    使用 to_csv 方法將 DataFrame 寫入 CSV 文件中，並解決中文亂碼問題。
   
    這段程式碼旨在計算股票的布林通道指標並基於此指標執行交易策略，同時提供可視化和交易記錄的功能。



