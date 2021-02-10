# Marketplace

<iframe width="560" height="315" src="https://www.youtube.com/embed/KpnncgSfKXY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This is the AlgoBulls Platform Marketplace for strategies.

Before adding any strategy to your Portfolio, you can search for strategies here, look into the details for each strategy, and view the backtesting reports to evaluate the performance. 

[ ![Marketplace](imgs/screenshots/mkt1.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/mkt1.png)

## Searching for a Strategy
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/VQCWEm4gJHg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[ ![Marketplace](imgs/screenshots/search_filter.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/search_filter.png)

`Search Bar` - You can type your keywords here.

`Favorites` Toggle - Toggle the switch to see the strategies marked as Favorite (<font size=3>☆</font>)

`Time` - Search for strategies added to the marketplace in the last month, last 3 days, last 2 weeks, or all time. 

`Filter` - You can filter your view as per the following categories shown.

[ ![Marketplace](imgs/screenshots/search_filter_2.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/search_filter_2.png)

`Sort By` - You can sort the strategies into the following:

* Backtest PnL <font size=5>↑ ↓</font>
* Drawdown <font size=5>↑ ↓</font> 
* Transaction Charges <font size=5>↑ ↓</font>
* Most Recent Transactions <font size=5>↑ ↓</font>

[ ![Marketplace](imgs/screenshots/search_sort.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/search_sort.png)

`Pagination` - You can click the < and > for changing pages. You can also choose to view 6/8/10 strategies per page.

[ ![Marketplace](imgs/screenshots/search_pagination.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/search_pagination.png)

## What does a Strategy Card look like
---

[ ![Marketplace](imgs/mkt10.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/mkt10.png)

## A look at the toolbar
---

![Marketplace](imgs/market-place-14.png)

`Expand` - You see a detailed and expanded view of a strategy when you click on the card or click this button. The effect is the same when you click on a Strategy Card.

`Tweak` - Click this button to tweak the parameters of a strategy. This is what happens when you click the `Tweak` button:

* The strategy gets added to your account
* You are re-directed to the [Paper Trading & Backtesting](paperback.md) page
* Click on `Tweak` on the newly added strategy on this page

`Share` - Click this button to get a shareable link for a strategy. You will see this message:

![Marketplace](imgs/screenshots/url_copied.png)

`Add to Favorites` - Click this button to add this strategy to Favorites for easy viewing later.

## When you click on a Strategy Card
---

Clicking on a Strategy Card will give you a detailed and expanded view of the strategy.

[ ![Marketplace](imgs/screenshots/expanded_view.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/expanded_view.png)


### The LHS of the Expanded View for a Strategy Card
---
The Left-hand Side of the expanded view shows the same details and the toolbar as the marketplace.

[ ![Marketplace](imgs/screenshots/lhs.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/lhs.png)

In addition to that, the following details are visible:

 * `Strategy Code` - It is a unique identification code assigned to each strategy. You can search the strategy directly with the code.
 * `Minimum Capital Required` - Minimum capital required in order to trade the strategy. There are different minimum amounts required to trade strategies depending upon the type of security and market the strategy is being traded into.
 * `Transaction Charges (in %)` - Indicative transaction charges strategy is expected to incur per trade.
 * `Recommended Duration (Days)` - Duration over which the strategy is expected to generate positive returns.
 * `Required Risk Appetite` -  Maximum downside investor is expected to bear in order to make profits over the duration of the strategy.

### The RHS of the Expanded View for a Strategy Card
---

The Right-hand Side of the expanded view has 2 tabs:
 
 * `Strategy Algorithm` - Gives an overview of functioning of the strategy. You will find key parameters and entire logic of how the strategy is designed and works.
 * `Backtesting Report` - Backtesting is very crucial before making trading any strategy live. You get the entire trade summary of how the strategy has performed over backtesting period along with various key data points such as Net P/L (Rs & %), No of profitable trades, Hit Ratio, etc.

#### Strategy Algorithm
---
`Strategy Algorithm` has 2 tabs:
 
 [ ![Marketplace](imgs/screenshots/sap.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/sap.png)
 
 * `Parameters` - These are all the parameters used by the strategy. 
    * `Strategy By` - Creator of the strategy.
    * `Strategy Name` - Name of the strategy.
    * `Exchange` - Exchange the strategy is expected to trade on. This depends on the instrument the strategy being executed on such as NSE, NFO and MCX for Indian markets.
    * `Segment` - Segments the strategy is expected to trade on. This depends on the exchange the strategy being executed on such as NSE, NFO and MCX for Indian markets.
    * `Instrument` - Instrument on which the trading will be performed.
    * `Candle Interval` - Candle Interval in which the strategy will be performed. 1 Min, 3 Mins, 5 Mins, 15 Mins and 30 Mins are some of the candle types which can be used to generate signals.
    * `Trading Type` - States the trading type on which strategy will be performed. Intraday and Delivery are two modes supported by the platform. Transaction charges differ for both the trading types.
    * `Trading Start Time` - Start time of the strategy. This can be user defined depending on the trading time.
    * `Trading Stop Time` - Stop time of the strategy. This can be user defined depending on the trading time.
    * `Parameters` - Key parameters of the strategy. This differs from strategy-to-strategy based on the logic. Example: Fast MA Period, Slow MA Period, Signal Period etc.

[ ![Marketplace](imgs/screenshots/sad.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/sad.png)

 * `Details` - 

#### Backtesting Report
---
`Backtesting Report` has 4 tabs:
 
[ ![Marketplace](imgs/screenshots/brs.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/brs.png)
 
 * `Summary` - Summary statistics of the strategy backtesting performed.
    * `Net PnL` - Net PnL of the strategy.
    * `Net PnL %` - Net PnL of the strategy in absolute percentage.
    * `Max Drawdown` - Max drawdown the strategy suffered during backtesting period.
    * `Max Drawdown %` - Max drawdown the strategy suffered during backtesting period in percentage.
    * `Number of Trades` - No. of signals strategy generated during the backtesting.
    * `Number of Wins` - No. of wins during the backtesting period
    * `Number of Looses` - No. of losses during the backtesting period
    * `Number of Long Trades` - No. of Long Trades strategy generated during backtesting period.
    * `Number of Short Trades` - No. of Short Trades strategy generated during backtesting period.
    * `Max Gain` - Max Gain during backtesting period.
    * `Min Gain` - Min Gain during backtesting period. This is different than the Drawdown value because it considers the minimum possible return from strategy.
    * `Avg. Profit per winning trade` - Cumulative Profit for winning trades divided by No. of Wins
    * `Avg. Profit per losing trade` - Cumulative Loss for winning trades divided by No. of Wins
    
[ ![Marketplace](imgs/screenshots/brr.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/brr.png) 
    
 * `Returns` - Shows the returns given by the strategy over a period of time.
    * `All Time` -Returns during the entire backtesting period.
    * `Last month` - Returns during last 1 month.
    * `Last 2 weeks` - Returns during last 2 weeks. 
    * `Last 3 days` - Returns during last 3 days.

[ ![Marketplace](imgs/screenshots/brt.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/screenshots/brt.png)

 * `Tradebook` - Entire trade book for the backtesting period.
    * `Instrument` - Instrument strategy being performed on.
    * `Entry Time` - Entry time of trade.	
    * `Entry` -	Entry trade type such as Buy/Sell
    * `Entry Qty.` - Quantity traded	
    * `Entry Price` - Price at which entry trade was executed	
    * `Exit Time` -	Exit time of trade.
    * `Exit` - Exit trade type such as Buy/Sell	
    * `Exit Qty.` -	Quantity traded. This depends on the number of profit booking trades embedded in the strategy logic.
    * `Exit Price` - Price at which exit trade was executed.	
    * `PnL (Rs.) / PnL %` -	PnL amount and PnL % of each trade.
    * `PnL Cum. (Rs.) / PnL Cum. %` - Cumulative PnL amount and Cumulative PnL % of each trade.
 * `Insights (Beta)` - Graphical representation of trading results over the backtesting period. X-Axis is the daily time series of the backtesting period and Y-Axis is the amount and percentage depending upon the data.
    * `P&L Absolute (Rs.)` - Absolute P&L in Rs./INR.
    * `P&L %` - Absolute P&L in %.
    * `P&L Cumulative Absolute (Rs.)` - Absolute Cumulative P&L in Rs./INR
    * `P&L Cumulative %` - Absolute Cumulative P&L in %.