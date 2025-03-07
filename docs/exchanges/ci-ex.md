# `ciex`

## 📁 Connector Info

* Type: SPOT CLOB DEX
* Folder: [hummingbot/connector/exchange/ciex](https://github.com/hummingbot/hummingbot/tree/master/hummingbot/connector/exchange/ciex)
* Maintainer: [CoinAlpha](https://coinalpha.com)

## 🏆 Exchange Tier

![](https://img.shields.io/static/v1?label=Hummingbot&message=BRONZE&color=green)

Bronze exchange connectors have passed the Minimum Voting Power Threshold in the latest Poll and are included in each monthly release. They are not maintained by Hummingbot Foundation but may be maintained by a community member.

## ℹ️ Exchange Info

* Website: <https://ci-ex.com/en_US/>
* CoinMarketCap:
* CoinGecko:
* API docs:
* SDK:

## 🔑 Connection

Run `connect ciex` in order to enter your API keys:

```
Enter your CI-EX API key >>>
Enter your CI-EX secret key >>>
```

If connection is successful:

```
You are now connected to ciex.
```

## 🪙 Fees

Hummingbot assumes 0.75% maker fees and 0.75% taker fees ([source](https://github.com/hummingbot/hummingbot/blob/master/hummingbot/connector/exchange/ciex/ciex_utils.py#L9)).

Users can override these assumptions with [Override Fees](/global-configs/override-fees/).
