# 📈 Fibonacci Martingale Strategy

The Fibonacci Martingale Strategy is a trading strategy implemented in Pine Script for the TradingView platform. It combines the concepts of Fibonacci levels and the martingale betting system to manage trades and risk.

## 📝 Strategy Overview

The strategy operates by placing a base order and a series of safety orders at predetermined Fibonacci levels. If the price moves against the initial position, the strategy will open additional safety orders to average down the entry price. The goal is to recover losses from the initial trade and potentially generate profits.

Key features of the strategy:

- 📊 Customizable base order size and safety order size
- 🔄 Adjustable safety order step scale and volume scale
- 💰 Configurable take profit percentage
- ⛔ Maximum number of safety orders limit
- 🛑 Optional stop-loss functionality to limit potential losses

## ⚙️ Parameters

The strategy includes the following adjustable parameters:

- `Base Order Size (%)`: The size of the initial base order as a percentage of the available capital.
- `Safety Order Size (%)`: The size of each safety order as a percentage of the available capital.
- `Safety Order Step Scale`: The scale factor used to determine the price levels for placing safety orders.
- `Safety Order Volume Scale`: The scale factor used to increase the volume of each subsequent safety order.
- `Price Deviation to Open Safety Orders (%)`: The percentage deviation from the initial entry price at which safety orders will be placed.
- `Take Profit (%)`: The percentage above the average entry price at which the strategy will close all positions and take profit.
- `Max Safety Orders Count`: The maximum number of safety orders allowed (up to 8).
- `Use Stop Loss`: A boolean option to enable or disable the stop-loss feature.
- `Stop Loss Deviation (%)`: The percentage deviation from the initial order price at which the stop-loss will be triggered.

## ⚠️ Risk Management

Please note that the Fibonacci Martingale Strategy involves a high level of risk. The martingale approach can lead to significant losses if the price continues to move against the position and the maximum number of safety orders is reached. The newly added stop-loss feature can mitigate some of these risks by closing the position at a predefined loss level, thereby limiting potential losses. However, it is crucial to understand the risks involved and use the strategy with caution.

## 🛠️ Installation

To use the Fibonacci Martingale Strategy, follow these steps:

1. Open the Pine Editor on TradingView.
2. Copy the provided code and paste it into the Pine Editor.
3. Customize the input parameters according to your preferences.
4. Save the script and add it to your chart.

## 🛡️ Disclaimer

The Fibonacci Martingale Strategy is provided "as is" without any warranty. The author shall not be liable for any damages or losses arising from the use of this strategy. It is important to thoroughly backtest and understand the risks before using the strategy with real funds.

## 📜 License

This work is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to provide any feedback or suggestions for improvement.
