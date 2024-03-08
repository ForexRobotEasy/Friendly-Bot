# Friendly Bot - ReadMe

## Description
Friendly Bot is a multi-currency Forex software solution developed by Forex Robot Easy. It aims to provide an automated trading experience for users with a risk appetite of their choice. The bot uses a grid trading strategy to open positions on pullbacks in the market, taking into consideration the user-defined parameters such as risk, maximum number of open positions, grid step size, and pullback threshold.

For detailed reviews and trading results of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/friendly-bot-review-a-multi-currency-forex-software-solution/). Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5.

## Input Parameters
- Risk: The risk appetite of the user. It determines the lot size of the positions opened by the bot. Default: 1.0.
- EnableTrading: Enable or disable trading. If set to false, the bot will not open any positions. Default: true.
- MaxPositions: The maximum number of open positions allowed by the bot. If the number of open positions reaches this limit, no new positions will be opened. Default: 5.
- GridStep: The size of the grid steps used by the bot for opening positions. Default: 0.01.
- PullbackThreshold: The threshold for considering a pullback in the market. If the price retraces by this percentage or more, a position will be opened. Default: 0.02.

## Global Variables
- accountBalance: The current balance of the trading account.
- accountEquity: The current equity of the trading account.
- totalPositions: The total number of open positions.

## Initialization Function (OnInit)
The OnInit function is called when the expert advisor is initialized. It initializes the global variables by retrieving the current account balance and equity. It also sets the totalPositions variable to 0.

## Deinitialization Function (OnDeinit)
The OnDeinit function is called when the expert advisor is being deinitialized. It can be used to perform any necessary cleanup tasks.

## Tick Function (OnTick)
The OnTick function is called on every tick of the market. It first checks if trading is enabled and if the maximum number of positions is already reached. Then, it checks if the market conditions and time frame are suitable for trading. If all conditions are met, it checks if there is a clear market trend and if there is a pullback. If both conditions are satisfied, a new position is opened.

## Market Conditions Suitability Function (IsMarketConditionsSuitable)
The IsMarketConditionsSuitable function is used to check if the current market conditions are suitable for trading. This is a placeholder function and needs to be implemented based on the specific logic and indicators used by the bot.

## Time Frame Suitability Function (IsTimeFrameSuitable)
The IsTimeFrameSuitable function is used to check if the current time frame is suitable for trading. This is a placeholder function and needs to be implemented based on the specific logic and time frame requirements of the bot.

## Market Trend Clarity Function (IsMarketTrendClear)
The IsMarketTrendClear function is used to check if the current market trend is clear for trading. This is a placeholder function and needs to be implemented based on the specific logic and indicators used by the bot.

## Pullback Detection Function (IsPullback)
The IsPullback function is used to check if there is a pullback in the market. This is a placeholder function and needs to be implemented based on the specific logic and indicators used by the bot.

## Position Opening Function (OpenPosition)
The OpenPosition function is called when there is a pullback in the market and all conditions for opening a position are satisfied. This is a placeholder function and needs to be implemented based on the specific logic and parameters of the bot. After opening a position, the totalPositions variable is increased.

## Execution Function (OnTimer)
The OnTimer function is called periodically and can be used for 24/7 operation logic. This function is not implemented in the provided code and needs to be implemented based on the specific requirements of the bot.

Please note that the provided code is a basic framework and does not contain the complete logic for trading. It serves as a starting point for implementing the desired trading strategy.

For more information and detailed reviews of the Friendly Bot product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/friendly-bot-review-a-multi-currency-forex-software-solution/).
