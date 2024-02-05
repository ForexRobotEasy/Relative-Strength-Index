# Relative Strength Index (RSI) Expert Advisor

This Expert Advisor (EA) is designed to trade based on the Relative Strength Index (RSI) indicator. The RSI is a momentum oscillator that measures the speed and change of price movements. It oscillates between 0 and 100 and is typically used to identify overbought and oversold conditions.

## Input Parameters

- RSI_Period: The period for RSI calculation (default: 14)
- RSI_Level_Overbought: The overbought level for RSI (default: 70)
- RSI_Level_Oversold: The oversold level for RSI (default: 30)
- Trade_Start_Hour: The hour to start trading (default: 8)
- Trade_End_Hour: The hour to end trading (default: 16)
- Take_Profit: The take profit level in pips (default: 100)
- Stop_Loss: The stop loss level in pips (default: 50)

## Usage

1. Include the necessary libraries `Trade.mqh` and `Indicators.mqh`.
2. Create an instance of the RSI indicator using `CRSI rsi`.
3. Create an instance of the trading class using `CTrade trade`.
4. In the `OnTick()` function, check if it's time to trade based on the specified trading hours.
5. Retrieve the RSI value using `rsi.iRSI()` function.
6. Compare the RSI value with the overbought and oversold levels.
7. If the RSI is above the overbought level, execute a sell order using `trade.Sell()` function.
8. If the RSI is below the oversold level, execute a buy order using `trade.Buy()` function.
9. In the `OnDeinit()` function, close any open positions when the EA is removed from the chart.

## Product Description

The RSI Expert Advisor is an advanced forex trading tool developed by the Forex Robot Easy Team. This EA is designed to automate trading decisions based on the popular Relative Strength Index (RSI) indicator.

The RSI is a widely used momentum oscillator that helps identify overbought and oversold conditions in the market. This EA takes advantage of the RSI indicator to execute buy and sell orders automatically.

With customizable input parameters, traders can adjust the RSI period, overbought and oversold levels, trading hours, take profit, and stop loss levels according to their trading preferences.

The RSI Expert Advisor is suitable for both beginner and experienced traders who want to incorporate the power of the RSI indicator into their trading strategy. It eliminates the need for manual analysis and execution, saving time and effort.

Please note that Forex Robot Easy is not the official developer of this product. We have provided a sample code that demonstrates how this product works. To find the official developer and access detailed reviews and trading results, please visit [this link](https://forexroboteasy.com/forex-robot-review/rsi-expert-advisor-review-advanced-forex-tool-for-mt5/). For further information and support, we recommend referring to the MQL5 platform.
