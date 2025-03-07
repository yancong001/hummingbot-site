The sample scripts below can be found in the [/scripts](https://github.com/hummingbot/hummingbot/tree/master/scripts) folder in the Hummingbot codebase.

In the Hummingbot client, run a script with:

```
start --script [SCRIPT NAME]
```

## Adjusted Mid Price

* **Code**: [adjusted_mid_price](https://github.com/hummingbot/hummingbot/blob/master/scripts/adjusted_mid_price.py)
* **Author**: [cmichaeltimmons](https://github.com/cmichaeltimmons)
* **Release Added**: [1.9.0](/release-notes/1.9.0)
* **Description**: This is an example of a pure market making strategy with an adjusted mid price.  The mid price is adjusted to the midpoint of a hypothetical buy and sell of a user defined {test_volume}.

## Advanced Directional

* **Code**: [advanced_directional_strategy_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/advanced_directional_strategy_example.py)
* **Author**: [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.13.0](/release-notes/1.13.0)
* **Description**: A directional trading strategy that uses two timeframes of the same trading pair `(ETH-USDT)` and based on the RSI and Bollinger Bands is going long or short. The weigths of the indicators are the same, that means that `0.5 * RSI + 0.5 * BBANDS = signal_value`, but we are going to prioritize 1m timeframe so after calculating the signal for 1m and 3m, we are going to multiply the value of 1m by 0.7 and 3m by 0.3.

## AMM Price

* **Code**: [amm_price_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/amm_price_example.py)
* **Author**: [fengtality](https://github.com/fengtality)  
* **Release Added**: [1.13.0](/release-notes/1.13.0)
* **Description**: This example shows how to call the /amm/price Gateway endpoint to fetch price for a swap

## AMM Trade

* **Code**: [amm_trade_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/amm_trade_example.py)
* **Author**: [fengtality](https://github.com/fengtality)  
* **Release Added**: [1.13.0](/release-notes/1.13.0)  
* **Description**: This example shows how to call the /amm/trade Gateway endpoint to execute a swap transaction

## Buy dip

* **Code**: [buy_dip_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/buy_dip_example.py)
* **Author**: [aarmoa](https://github.com/aarmoa)
* **Release Added**: [1.4.0](/release-notes/1.4.0)
* **Description**: This strategy buys ETH (with BTC) when the ETH-BTC drops 5% below 50 days moving average (of a previous candle)
    This example demonstrates:
      - How to call Binance REST API for candle stick data
      - How to incorporate external pricing source (Coingecko) into the strategy
      - How to listen to order filled event
      - How to structure order execution on a more complex strategy

## Buy low sell high

* **Code**: [buy_low_sell_high](https://github.com/hummingbot/hummingbot/blob/master/scripts/buy_low_sell_high.py)
* **Author**: [Alkhalifah-blockchain](https://github.com/Alkhalifah-blockchain)
* **Release Added**: [1.9.0](/release-notes/1.9.0)
* **Description**: The script will be calculating the MA for a certain pair, and will execute a buy_order at the golden cross and a sell_order at the death cross.

## Buy only three times

* **Code**: [buy_only_three_times_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/buy_only_three_times_example.py)
* **Author**:  [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.7.0](/release-notes/1.7.0)
* **Description**: This example places shows how to add a logic to only place three buy orders in the market, use an event to increase the counter and stop the strategy once the task is done.

## Candles Example

* **Code**: [candles_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/candles_example.py)
* **Author**: [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.13.0](/release-notes/1.13.0)
* **Description**: This is a strategy that shows how to use the new Candlestick component. It acquires data from both Binance spot and Binance perpetuals to initialize three different timeframes of candlesticks. The candlesticks are then displayed in the status, which is coded using a custom format status that includes technical indicators.

## DCA Example

* **Code**: [dca_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/dca_example.py)
* **Author**: [aarmoa](https://github.com/aarmoa)
* **Release Added**: [1.4.0](/release-notes/1.4.0)
* **Description**: This example shows how to set up a simple strategy to buy a token on fixed (dollar) amount on a regular basis

## Format Status

* **Code**: [format_status_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/format_status_example.py)
* **Author**: [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.7.0](/release-notes/1.7.0)
* **Description**: This example shows how to add a custom `format_status` to a strategy and query the order book.

## Log Price

* **Code**: [log_price_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/log_price_example.py)
* **Author**: [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.7.0](/release-notes/1.7.0)
* **Description**: This example shows how to get the ask and bid of a market and log it to the console.

## Microprice Calculator

* **Code**:  [microprice_calculator](https://github.com/hummingbot/hummingbot/blob/master/scripts/microprice_calculator.py)
* **Author**: [ntnle](https://github.com/ntnle)
* **Release Added**: [1.13.0](/release-notes/1.13.0)
* **Description**: A script that can compute the microprice adjusted midprice of token pairs and display that midprice adjusted for the imbalance of the order book, and other information.

## Simple Directional strategy

* **Code**: [simple_directional_strategy_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/simple_directional_strategy_example.py)
* **Author**: [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.13.0](/release-notes/1.13.0)
* **Description**: A simple trading strategy that uses RSI in one timeframe to determine whether to go long or short.

## Simple PMM

* **Code**: [simple_pmm_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/simple_pmm_example.py)
* **Author**:  [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.9.0](/release-notes/1.9.0)
* **Description**: The bot will place two orders around the `price_source` (mid price or last traded price) in a `trading_pair` on exchange, with a distance defined by the `ask_spread` and `bid_spread`. Every `order_refresh_time` in seconds, the bot will cancel and replace the orders.

## Simple RSI

* **Code**: [simple_rsi_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/simple_rsi_example.py)
* **Author**: [shibanovp](https://github.com/shibanovp)
* **Release Added**: [1.10.0](/release-notes/1.10.0)
* **Description**: The strategy is to buy on overbought signal and sell on oversold.

## Simple VWAP

* **Code**: [simple_vwap_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/simple_vwap_example.py)
* **Author**: [cardosofede](https://github.com/cardosofede)
* **Release Added**: [1.7.0](/release-notes/1.7.0)
* **Description**: This example lets you create one VWAP in a market using a percentage of the sum volume of the order book until a spread from the mid price. This example demonstrates:
      - How to get the account balance
      - How to get the bids and asks of a market
      - How to code a "utility" strategy

## Simple XEMM

* **Code**: [simple_xemm_example](https://github.com/hummingbot/hummingbot/blob/master/scripts/simple_xemm_example.py)
* **Author**: [fengtality](https://github.com/fengtality)
* **Release Added**: [1.10.0](/release-notes/1.10.0)
* **Description**:  A simplified version of Hummingbot `cross-exchange market making` strategy, this bot makes a market on the maker pair and hedges any filled trades in the taker pair. If the spread (difference between maker order price and taker hedge price) dips below `min_spread`, the bot refreshes the order

## Triangular Arbitrage

* **Code**: [triangular_arbitrage](https://github.com/hummingbot/hummingbot/blob/master/scripts/triangular_arbitrage.py)
* **Author**: [supervik](https://github.com/supervik)
* **Release Added**: [1.10.0](/release-notes/1.10.0)
* **Description**:  This script executes arbitrage trades on 3 markets of the same exchange when a price discrepancy among those markets is found.
