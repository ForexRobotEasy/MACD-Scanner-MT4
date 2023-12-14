# MACD Scanner MT4

**Developer**: Forex Robot Easy Team
**Website**: [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/macd-scanner-mt4-a-review-of-the-forex-software-for-professional-traders/)

This code represents a custom indicator for MetaTrader 4 (MT4) called MACD Scanner MT4. It allows traders to scan for MACD trend conditions on multiple timeframes and receive alert notifications when these conditions are met.

## How it Works

The indicator utilizes the following libraries and global variables:

- `Trade.mqh` - A library for trading operations
- `MA.mqh` - A library for calculating moving averages
- `ExpMA.mqh` - A library for calculating exponential moving averages
- `MACD.mqh` - A library for calculating MACD values
- `Button.mqh` - A library for creating buttons on the interface
- `Label.mqh` - A library for creating labels on the interface
- `Edit.mqh` - A library for creating text input fields on the interface

The input parameters for the indicator are as follows:

- `FastEMA` - The period for the fast exponential moving average (default: 12)
- `SlowEMA` - The period for the slow exponential moving average (default: 26)
- `SignalSMA` - The period for the signal simple moving average (default: 9)
- `Timeframe` - The timeframe for MACD calculation (default: H1)

The `OnInit` function is responsible for initializing the indicator by creating a user-friendly interface with a start button, a label, and a text input field. The `OnDeinit` function is called when the indicator is being deinitialized, and it cleans up and releases any resources used by the interface elements.

The `OnCalculate` function is the main iteration function of the indicator. It checks if the start button is clicked and retrieves the symbol entered by the user. It then sets the symbol and timeframe for MACD calculation and calculates the MACD values using the `MACD.Calculate` method. After that, it retrieves the MACD trend values for multiple timeframes using the `MACD.GetMainValue` and `MACD.GetSignalValue` methods. If the MACD trend condition is met (i.e., the main MACD value is greater than the signal MACD value), it sends an alert notification using the `SendNotification` function.

The `start` function is responsible for displaying the user-friendly interface by calling the `Draw` method for each interface element.

## Product Description

[MACD Scanner MT4](https://forexroboteasy.com/forex-robot-review/macd-scanner-mt4-a-review-of-the-forex-software-for-professional-traders/) is a custom indicator developed by Forex Robot Easy Team. It is designed for professional traders who want to scan for MACD trend conditions on multiple timeframes and receive alert notifications when these conditions are met.

Key Features:
- Easy-to-use interface with a start button, label, and text input field
- Customizable input parameters for fast and slow exponential moving averages, signal simple moving average, and timeframe
- Calculates MACD values and retrieves MACD trend values for multiple timeframes
- Sends alert notifications when MACD trend conditions are met
- Compatible with MetaTrader 4 (MT4)

Please note that Forex Robot Easy is not the official developer of this product. We only provide sample code that can work as described in the product. To find the official developer of this product and access detailed reviews and trading results, please visit the [official website](https://forexroboteasy.com/forex-robot-review/macd-scanner-mt4-a-review-of-the-forex-software-for-professional-traders/) or use MQL5.
