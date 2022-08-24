# Python Build

## 1. Introduction
---

Now you can code your own strategy easily using our Python Build service! Begin coding your own strategy from scratch, or modify some of our ready-made templates to suit your needs. Get access to our state-of-the-art AlgoBulls Core Trading Engine, which automatically leverages our infra so that you can access the latest historical data to gauge the performance of your strategies. Tweak the various parameters of your strategy to choose the ideal instrument, indicator values, and profit loss percentages as per your needs! View the performance of your strategy using our visual analytics feature and continue to tweak till you are satisfied with the performance. Get your strategy approved for live trading from our experts and deploy it on 30+ supported brokers without coding any broker integration logic.

Go to **Build Strategy** in the sidebar navigation and select **Python Build** to know more.

![pythonbuild](imgs/python_build_select.png)

## 2. An overview
---

![pythonbuild](imgs/python_build_dashboard.png)

**Running Strategies:** This section shows how many strategies are currently active and running in your account. 

**Strategies Saved:** This displays the number of strategies saved in your AlgoBulls account. 

**Execution Time Consumed:** You can view the number of minutes that have been used for backtesting strategies.

!!! note "Note:"

    The use of backtesting is limited to one month. On weekends and after midnight (post 12 AM), you won't be able to backtest strategies.
 
**Analytics Support:** This shows whether or not your analytics support is active. Analytics support is not available to free plan users.

**Professional Support:** This section connects you to other professional support forums for additional support while developing the strategy. 

**Active Plan:** This section displays the current plan active on your AlgoBulls account. 

**Ready Templates:** Ready-to-use templates that you can modify and test.

![pythonbuild](imgs/python_build_ready_templates.png)

**My Coded Strategies:** Strategies that have been coded and saved by you are displayed here. This includes new and modified strategies developed by you.

![pythonbuild](imgs/python_build_my_strategies.png)

**Quick Help:** Resources to help you code better.

![pythonbuild](imgs/python_build_help.png)

## 3. **How to get started with Python Build?**

To start developing your own strategy, you must first activate a plan from the **Plans & Wallet** section. Select the **Developers** option in the **Explore Plans** section and select a plan of your choice. There are currently two developer plans available:

![pythonbuild](imgs/python_build_plans.png)


* **Premium Developer Plan** - Develop your own Algorithmic Trading Strategy with Analytics support, concurrent Strategy Executions, Professional Support, and more.

* **Free Developer Plan** - Develop your own Algorithmic Trading Strategy for Free.

After selecting your preferred plan, you will be able to begin coding. You can either edit the preloaded **Ready templates** or use **My Coded Strategies** section to create your own strategies

## 4. **How to code strategies using Ready Templates?**

![pythonbuild](imgs/python_build_ready_templates.png)

Select a template that you would like to modify from the **Ready Template** section. To view all the ready-to-use templates click on **More**.

![pythonbuild](imgs/python_build_all_ready_templates.png)

Click on the **Code button** placed in the bottom right corner of the selected template to view the strategy code.

![pythonbuild](imgs/python_build_selected_strategy.png)

You should now see the **code editor**, where you can start modifying the code as required.

![pythonbuild](imgs/python_build_code_edit.png)

To save the strategy, click the Save button. This strategy will be added to your list of **My coded strategies**.

![pythonbuild](imgs/python_build_save_strategy.png)

Follow these simple steps to test the strategy's performance

**Step 1**

After clicking **Save & Start**, a pop-up window will appear.

![pythonbuild](imgs/python_build_save_and_start.png)

**Step 2**

In the **customizations** section choose **back data for backtesting** or **live data for paper trading**.

Select the duration option in the customizations section. Add the desired date and time, as well as the quantity/lots. In backtesting you will need to put the start date and end date along with time.

![pythonbuild](imgs/python_build_backtesting.png)

In paper trading you only need to add the start and end time.

![pythonbuild](imgs/python_build_papertesting.png)

**Step 3**

Once you scroll below, you will see the P&L tracker. Switch the P&L tracker ON and enter your desired profit and risk appetite. To keep things simple, you can also leave it turned off.

![pythonbuild](imgs/python_build_pnl.png)

**Step 4**

In the Configuration section, you can check the parameters added or modified by you.
 
**Step 5**

To begin testing the strategy, click on Execute.

![pythonbuild](imgs/python_build_terms_check.png)

**Step 6**

Go to the **Results** section to see how the strategy has performed.

!!! note "Note:" 

    Backtesting/Paper Trading would be available from Monday - Friday (excluding NSE holidays) from 9 AM to 11:30 PM. You can code your strategy & analyse the strategy results 24x7.

![pythonbuild](imgs/python_build_results.png)

![pythonbuild](imgs/python_build_stats.png)

![pythonbuild](imgs/python_build_pnl_book.png)

![pythonbuild](imgs/python_build_user_log.png)

![pythonbuild](imgs/python_build_order_history.png)

You can **rename** a strategy by clicking the edit symbol besides the strategy name.

![pythonbuild](imgs/python_build_strategy_rename.png)

!!! note "Note:" 
    The Analytics & Graph sections are only visible to premium plan users. If you are using a free plan, switch to a [premium developer plan now](https://devel.appv2.algobulls.com/wallet/checkout?packageType=PackageCombo&plan=5&type=renew).

**How to view the Results?**

Once you start the strategy, it may take a while for it to complete the execution. You can Switch to the Results tab after you run your strategy.  Even if the strategy execution is not complete, you will still see intermediate results.

Only Premium developer plans users will be able to view the strategy analytics values & graphs.

## 5. How to view Analytics?

**Statistics:** In the statistics section, you can view a strategy’s Stats & various other metrics in the form of graphs like P&L and ROI.

**i. Stats:** In this section you can see the **hit ratio, number of trades, average trades per day**.

![pythonbuild](imgs/python_build_stats.png)

**ii. P&L (INR):**  The trade by trade P&L in INR.

![pythonbuild](imgs/python_build_pnl_2.png)

**iii. P&L %:** The trade by trade P&L in percentage form.

![pythonbuild](imgs/python_build_pnl_percent.png)

**iv. ROI (INR):** Cumulative P&L of all the trades.

![pythonbuild](imgs/python_build_roi_inr.png)

**v. ROI%:** You will be able to view the ROI in percentage here.

![pythonbuild](imgs/python_build_roi_percent.png)

[**vi. The Graph Tool**](https://help.algobulls.com/member/strategy-card.html#6-graph-toolbar) 

![pythonbuild](imgs/python_build_graph_tool_2.png)

**P&L Book:** View detailed trade by trade report. Premium users can analyse this data in the form of heatmaps for Gross Profit & Loss, Trading Volume & Total number of Trades.

![pythonbuild](imgs/python_build_pnl_book.png)

![pythonbuild](imgs/python_build_trade_volume.png)

![pythonbuild](imgs/python_build_total_trade.png)

**User Log:**  Real time logs from strategy execution are displayed in this section. Use these logs to debug your strategy’s behaviour and performance.

![pythonbuild](imgs/python_build_user_log.png)

**Order History:** View the order state transition for every order placed by your strategy in depth. 

![pythonbuild](imgs/python_build_order_history.png)

## 6. **How to code a new strategy?**

If you want to create your own strategy, click on the **+ Sign** in the **Code New Strategy** option under the **My Coded Strategies** section.

![pythonbuild](imgs/python_build_new_strategy.png)

A new blank code editor will open, allowing you to start coding your new strategy. After you've finished coding, click **Save** to save this strategy in the **My Coded Strategies** section.

![pythonbuild](imgs/python_build_code_new_strategy.png)

Next, you need to configure the strategy’s parameters by clicking on the settings symbol in the top right corner of the code editor. In this section you can add, view & edit the strategy parameters.

To test the behaviour and performance of the strategy, click on **Save & Start** and follow the directions given earlier. The performance of the strategy will soon be available in the **Results** section.

You can rename a strategy by clicking the edit symbol besides the strategy name. 

![pythonbuild](imgs/python_build_rename_new_strategy.png)

## 7. **How to Configure Strategy Parameters?**

![pythonbuild](imgs/python_build_new_strategy_parameters.png)

You can configure the strategy’s parameters by clicking on the settings symbol on the top right corner of the code editor. In this section you can view a strategy’s parameters or edit these parameters too.

To know more about the parameters, [click here](https://help.algobulls.com/member/tweak.html).

![pythonbuild](imgs/python_build_edit_configuration.png)

