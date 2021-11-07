# Trading strategy using the program
[RU](pages/TradingStrategyRU.md).

Today we will analyze one of the most common strategies for trading cryptocurrency and a tool that claims to be a "must have"  tool that helps to facilitate the trader's work. The trading strategy is based on the work with the limit orders’ density in the order book. We will analyze how to find limit orders later, first we need to figure out how to work with levels.
Levels are the most important tool in any financial markets, including the cryptocurrency market. Levels are where there is an imbalance between buyers and sellers.
When you see a repeated bounce of the price from the level, this is, in fact, the level at which the imbalance occurs.
Why are levels so important? It is simple, at these levels there is an accumulation of limit orders of both buyers and sellers (because it is obvious to everyone where to set the stop-loss). The price can bounce off these limit orders. If there is a huge limit order at the level, then the level is suitable for trading. An additional positive sign is that the price on the level is a round number.

#### The level has been found, now we need to search for limit orders.

At the time of writing, Binance can trade futures for more than 120 currencies, and even more coins that do not have futures yet. How do we look for big bids?
If you use CScalp, most likely you understand how inconvenient it is to open each currency pair one after another and search for limit orders manually. I suggest doing the opposite. First, we look for orders, and then we look for levels on the chart.
There is a great search solution - a cryptocurrency screener app for macOS, iPhone and iPad that solves this problem. The app is a fully automated solution for searching orders. The main function of the program is to automatically receive lists of orders directly from the exchange, and the algorithm searches for the largest order. The program shows a table of currencies and in each cell of the table indicates the price of the order in dollars. The app will visually highlight the cell where there are large enough orders and will sound a signal if it finds new ones. You can find more detailed information on how the app works in the manual or on the app website.

[Download link](https://apps.apple.com/app/id1590351885).

#### What is "breakout" and "bounce"

At the beginning of the article we said that we will consider two strategies "rebound" and "breakout". To understand which strategy to use, find on the chart how many times the price touched the found level. If there were no more than 3 such touches, then choose the “rebound” strategy, if there were more than 3 touches - a breakout.

![chart adausdt](/images/chart_adausdt.png)

Take a look at the ADA/USDT chart above. The limit order found by the program for the ADA/USDT currency pair, worth $ 2 million, is marked with a green line at the price level of $ 1.9.
Purple rectangles mark levels or “resistance” zones.
Notice how the price bounced off the first resistance zone several times. The price made 4 touches - where each touch is the very “bounce”, and then abruptly “broke” this level. The price always moves from level to level, therefore, after the breakout, the price already bounces off the limit order that our program found. On the chart, on average, each such bounce makes about 5-6% of the movement! It was possible to open a long position at least twice, on a rebound.
To trade we just need to correctly place our limit order, stop-loss, take-profit and find the entry point to the position. This is done very simply: if the price approaches the level from above, then you need to open a long position for a rebound. The stop should be placed under the limit order that our program found, and the take profit should be calculated from the volatility of the currency. The higher the volatility and the greater the amplitude of the price movement, the more profit you can take.
Trading does not require the use of special terminals, the web version of Binance and any device from Apple is enough to install the “order book” program.

[TradingView](https://ru.tradingview.com/chart/ADAUSDT/5b16LrQa-order-book-trading/).

[Download link](https://apps.apple.com/app/id1590351885).

[Author](t.me/engineerios).
