# Portfolio

This page lists all the strategies opted/built by you.

![Portfolio](imgs/portfolio.png)

Each strategy listed on this page can be tweaked with many parameters, including the quantity with which you want to execute that particular strategy. Also, you can start/stop strategies from here, giving you complete control over what strategies you want to currently execute and monitor.

Note: Once you click `Start` to run a strategy, wait patiently for the button to change to `Stop`. When the button finally changes to `Stop`, you can be sure that your strategy is now successfully running. 

## Tweaks
This section gives you fine control over a strategy through a variety of sections.

The sections are:

**General, Strategy, Instruments, RMS, Resume, Exit and Misc**

Note: Press **Save** once you have finished tweaking.

Note: Press **Reset Defaults** to reset default parameters for that strategy.

# Fields

The following list gives a short brief about each field within each section.

## General
---
`Start Time (24 Hours)` - Give the start time for the strategy.

`End Time (24 Hours)` - Give the end time for the strategy.

![General](imgs/general.png)

## Strategy
---
`Candle` - Give the Candle Size here with which you want to trade (in number of minutes).

`Strategy Mode` - Choose among Intraday/Delivery

`Parameters` - Parameters are specific to a particular strategy. The parameters will be always filled with default values. You may choose to keep the default values or change them as required. 

Example: For the image shown below, the strategy is `Exponential Moving Average Crossover`, having 2 parameters: `Small Average` and `Big Average`. 

![Strategy](imgs/strategy.png)

## Instruments
---
`Instrument` - Choose the instrument on which you would like to fire the strategy.

Example: Stocks, Commodities, Currencies or Futures.

![Instrument](imgs/ins.png)

## RMS (Risk Management System)
---

`Target (%)` - Give that target percentage that you would like to reach.

A price target is the projected future price level of an asset as stated by an investment analyst or advisor. The price target is based on assumptions about the asset's future supply and demand, technical levels.

`Stoploss (%)` - Give the stoploss percentage where you would like to cut your losses.

A stop-loss order is an order placed with a broker to buy or sell once the stock reaches a certain price. A stop-loss is designed to limit an investor's loss on a security position.

`Trailing Stoploss (%)` -  Give the trailing stoploss percentage where you would like to cut your losses.

You also get an ability to trail your stoploss. So, if the contract/stock moves in your direction by a particular number of ticks, the stoploss will go up/down based on that.

![RMS](imgs/rms.png)

## Resume
---

This is applicable only for Delivery Based Trading Strategies.

Tick the relevant values if you wish to continue on the next day on the same carry-forward instrument. Unticking the values will square off everything a few minutes before the market closes.

The values are: **Resume Positions on start, Resume Holdings T+1 on start, Resume Holdings T+2 on start**

![Resume](imgs/resume.png)

---

## Exit
---

If you tick the Exit options given here, then the Resume options mentioned above will be unticked automatically.

You can tick these values to choose the required exit options for your strategy.

The values are: **Resume Holdings T+1 on start, Resume Holdings T+2 on start, Exit Intraday Orders on Stop, Exit T+0 Delivery orders on stop, Exit T+1 Delivery orders on stop, Exit T+2 Delivery orders on stop**

![Exit](imgs/exit.png)

## Misc
---

`Instrument max orders count` - Give the maximum order count that you would like the strategy to consider.

After the count is reached, your strategy stops running automatically.

`Remove instrument if order rejected` - Tick this if you want the strategy to stop if the order is rejected for any reason by the broker.

`Crossover accuracy decimals` - Give the number of decimals that you would like the strategy to consider for accuracy.

This value is generally 2 for stocks and 4 for currencies.

![Misc](imgs/misc.png)
