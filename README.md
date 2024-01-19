# Bright Night MT5

This is a fully automated advisor designed for trading during quiet hours in the forex market. It uses various patterns and spread analysis to determine trading opportunities. The code provided here is a sample implementation of the Bright Night MT5 strategy and is not the official product developed by ForexRobotEasy. To find the official developer of this product, please use MQL5.

## Description

The Bright Night MT5 advisor is designed to trade during periods of low market volatility, also known as quiet hours. It analyzes the spread and price patterns to identify potential trading pairs and executes trades based on a set of predefined rules.

The advisor works by monitoring the spread of the current symbol and checking if it exceeds a certain threshold. If the spread is widening, the advisor analyzes the Ask and Bid patterns to predict price movements. It then matches these patterns with the predefined trading pairs and calculates the lot size based on a trading strategy.

The trading pairs are predefined and can be customized by adding or removing pairs in the `OnInit` function. The minimum and maximum lot sizes are also defined as constants in the code.

The advisor uses the `Trade` library to execute trades. It sets various trade parameters such as slippage, stop loss, and take profit levels. These parameters can be adjusted in the `OnInit` function.

## Usage

To use the Bright Night MT5 advisor, follow these steps:

1. Include the necessary libraries `Trade.mqh` and `ArrayObj.mqh`.
2. Define the maximum number of trading pairs and the minimum and maximum lot sizes.
3. Create a `CTrade` object for executing trades and a `CArrayObj` object for storing the trading pairs.
4. Implement the `OnTick` function to monitor the spread, calculate patterns, and execute trades.
5. Implement the `CalculateAskPattern` and `CalculateBidPattern` functions to calculate the Ask and Bid patterns.
6. Implement the `CalculateLotSize` function to calculate the lot size based on the trading strategy.
7. Implement the `AverageSpread` function to calculate the average spread over a specified period.
8. Implement the `OnInit` function to initialize the trading pairs and trade settings.
9. Implement the `OnDeinit` function to free up resources and clean up.
10. Define the `CPair` class to represent a trading pair with pattern matching.

## Product Review

For detailed reviews and trading results of this product, please visit [ForexRobotEasy](https://forexroboteasy.com/forex-robot-review/bright-night-mt5-review-efficient-forex-trading-during-quiet-hours/). Please note that ForexRobotEasy is not the official developer of this product. The provided code is a sample implementation and may not reflect the exact functionality of the official product. To find the official developer of this product, please use MQL5.
