# Trade Assist Pro

Trade Assist Pro is an advanced risk management expert advisor designed for MT5 traders. It provides various features to help traders manage their risk effectively and improve their trading performance. This code demonstrates the basic functionality of Trade Assist Pro.

## External Parameters

- RiskPercentage: Specifies the risk percentage for position sizing. It determines the position size based on the risk amount and stop loss.
- SolidLots: Specifies the fixed lot size for position sizing. If the calculated position size is smaller than SolidLots, it will be set to SolidLots.
- CloseVolumePercentage: Specifies the percentage of position volume to close. It allows partial closure of positions.

## Global Variables

- g_magicNumber: A magic number used for trade identification.

## Expert Initialization Function

The OnInit() function is called during expert advisor initialization. It sets the risk level based on the input parameters and opens the initial position if the position size is greater than or equal to SolidLots.

## Expert Tick Function

The OnTick() function is called on each tick. It checks for order closure and partial closure of positions.

- If there are any open orders, it attempts to close all orders.
- If there are any open positions, it calculates the volume to be closed based on the CloseVolumePercentage and attempts to close the partial position.

## Helper Functions

The code includes several helper functions:

- OpenPosition: Places an order with the specified volume.
- CloseAllOrders: Closes all open orders.
- ClosePartialPosition: Closes a partial position with the specified volume.
- IsAnyOrderOpen: Checks if there are any open orders.
- IsAnyPositionOpen: Checks if there are any open positions.
- GetStopLoss: Calculates the stop loss value.
- GetPositionVolume: Calculates the position volume.

## Product Description

Trade Assist Pro is an advanced risk management expert advisor for MT5 traders. It offers a range of features to help traders effectively manage their risk and improve their trading performance.

Key Features:
- Risk Percentage: Set the risk percentage for position sizing, allowing you to control the amount of risk per trade.
- Fixed Lot Size: Specify a fixed lot size for position sizing, ensuring consistent position sizing regardless of risk.
- Partial Closure: Close a percentage of the position volume, allowing you to lock in profits while still keeping a portion of the trade open.
- Order Closure: Close all open orders with a single click, providing quick and convenient order management.

Trade Assist Pro is designed to work seamlessly with the MT5 trading platform. It is easy to install and configure, making it suitable for both beginner and experienced traders.

Please note that ForexRobotEasy is not the official developer of Trade Assist Pro. We are showcasing a sample code that demonstrates the basic functionality of the product. For detailed reviews and trading results of Trade Assist Pro, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/trade-assist-pro-review-advanced-risk-management-for-mt5-traders/). To find the official developer of Trade Assist Pro, please refer to MQL5.
