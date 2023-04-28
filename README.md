## Script 5

- Script for a simple trading strategy that uses moving averages, Bollinger Bands, chart patterns, and support/resistance levels. Here's how it works:
- Moving averages: The script calculates two simple moving averages (SMA) based on the close price of the asset over different time frames. The first is a 20-period SMA (ma1), and the second is a 50-period SMA (ma2).
- Bollinger Bands: The script calculates Bollinger Bands using the same 20-period SMA as the basis, with an upper band that is two standard deviations away from the basis (upper) and a lower band that is two standard deviations below the basis (lower).
- Greedy Strategy: The script uses the moving averages to create a basic greedy trading strategy. When the 20-period SMA (ma1) crosses above the 50-period SMA (ma2), the script generates a buy signal (longCondition), and when ma1 crosses below ma2, the script generates a sell signal (shortCondition).
- Edge Patterns: The script uses the TA-Lib library to look for "rising edge" and "falling edge" patterns in the price data. When a rising edge pattern is detected (edgeUp), a green triangle is plotted below the price bars, and when a falling edge pattern is detected (edgeDown), a red triangle is plotted above the price bars.
- Triangle Patterns: The script also uses the TA-Lib library to look for "triangle up" and "triangle down" patterns in the price data. When a triangle up pattern is detected (triangleUp), a green triangle is plotted below the price bars, and when a triangle down pattern is detected (triangleDown), a red triangle is plotted above the price bars.
- Support and Resistance: The script uses the TA-Lib library to calculate support and resistance levels based on pivot highs and lows in the price data. When a pivot low is detected (supp), a green line is plotted, and when a pivot high is detected (res), a red line is plotted.
- Plotting: The script plots all of the indicators and patterns on the price chart, including the moving averages, Bollinger Bands, support/resistance levels, and chart patterns.
- Buy and Sell Points: The script generates actual buy and sell signals using the strategy.entry() function. When a buy signal is generated (longCondition), the script enters a long position using strategy.entry("Buy", strategy.long). When a sell signal is generated (shortCondition), the script enters a short position using strategy.entry("Sell", strategy.short).

## Script 4
- The script then defines buy and sell signals based on the **greedy** strategy and both **edge** and **triangle** patterns. 
- The buy signal is triggered when the close price crosses above the upper Bollinger Band and the close price is either falling or rising for 5 consecutive periods, or when a triangle up pattern is detected. 
- The sell signal is triggered when the close price crosses below the lower Bollinger Band or when a triangle down pattern is detected.


## Script 3

- Calculates the moving average and Bollinger Bands based on user-defined lengths and standard deviation. 
- The script then plots the **moving** **average** and upper and lower **Bollinger** Bands on the chart.
- The script then defines buy and sell signals based on the **greedy** strategy and both **falling** and **rising** edge patterns. 
- The buy signal is triggered when the close price crosses above the upper Bollinger Band and the close price is either falling or rising for 5 consecutive periods, indicating a falling or rising edge pattern.
- The sell signal is triggered when the close price crosses below the lower Bollinger Band.

## Script 2

- The script calculates the moving average and Bollinger Bands based on user-defined lengths and standard deviation. 
- The script then plots the moving average and upper and lower Bollinger Bands on the chart.
- The script then defines buy and sell signals based on the **greedy** strategy. 
- The buy signal is triggered when the close price crosses above the upper Bollinger Band, and the sell signal is triggered when the close price crosses below the lower Bollinger Band.

## Script 1

- The script calculates the moving average and Bollinger Bands based on user-defined lengths and standard deviation. 
- The script then plots the **moving** **average** and upper and lower **Bollinger** Bands on the chart.
- The script then defines buy and sell signals based on the **greedy** strategy and **falling** edge pattern. 
- The buy signal is triggered when the close price crosses above the upper Bollinger Band and the close price is falling for **5** consecutive periods, indicating a falling edge pattern. 
- The sell signal is triggered when the close price crosses below the lower Bollinger Band.
