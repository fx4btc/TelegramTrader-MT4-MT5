**MT4**  [Test Demo now](http://t.me/TTraderMT4Bot)
**MT5**  [Test Demo now](http://t.me/TTraderMT5Bot)

## TelegramTrader ChatRoom
**MT4**  [FOREX](http://t.me/forex_telegram_trader)
**MT5**  [CRYPTO](http://t.me/crypto_telegram_trader)

# TelegramTrader-MT4-MT5
Connect Telegram Messenger to Metatrader for Trading, Controlling Robots, Monitoring Platform. Open trades, Open charts, use custom templates for technical analsysi on the go. Launch templates with robots attached to charts for semi-auto trading. Get prices and Daily Percentage change. Get the swap rates positive or negative from SWAP_LONG or SWAP_SHORT 

Use with Demo or Live trading accounts. 

## Standard commands
* Quotes (daily percentage change)
* Charts (any chart timeframe with custom templates)


## TT 1.0 Trading commands
* Buy or Sell (Market Order)
* Lock in profits (**Trail** button)
* Move takeprofit to breakeven (**Breakeven** or BE button)
* Close position and reverse direction (**Reverse** button)
* Move Takeprofit to recent fractal (**SetTakeProfit** button)
* Move Stoploss to recent fractal (**SetStopLoss** button)
* Close all positions immediately (**Close** button)
* Close your profitable positions (**Profit** button)

## TT 1.0 Bot commands
* Attach bots to any market on any timeframe
* Delete the bots from the charts
* turn on bots or turn bots off at anytime ( requires some coding into your robot)

## TT 2.0 Trading commands

| Function | Telegram Keyboard Commands |
|----------- | ----------|
| Price |	/p |
| Chart |	/c |
| OrderBook |	/book |
| Position |	/pos |
| Cancel Orders |	/cancel |
| Close Position |	/close |
| Buy Limit Order |	/bid |
| Sell Limit Order |	/ask |
| Limit Order Price |	/ask_p1000 /bid_p10 |
| Volume change |	/Volume value |
| Symbol change |	/Symbol BTCUSD |




# Adding the files to your MetaTrader Platform
Download the github zip folder to your desktop , extract the contents and prepare moving the files to the appropiate directories from the directions below.
1. Open Metatrader Platform and locate the Navigation Bar on the Top of platform
2. Click on **File**
3. Click on **Open Data Folder** and this will open the file directory where you place the following files
  * Open the **MQL4/MQL5** folder
  * Open the **Include** folder and place the files from the github zip folder **include** , Overwrite the files if present.
 * Open the **Experts** folder and place the files from the github zip folder **Telegram_Trader.ex4/ex5** 
  * restart the platform ( close application and reopen)
  
# Platform Setup Guide
1. Open Metatrader platform and locate the Navigation Bar on the Top of platform
2. Click on **Tools**
3. Click on **Options**
4. Click on **Expert Advisors**
  * Allow automated trading ( checkbox)
  * Allow dll imports ( chechbox)
  * Allow WebRequests for listed URL (checkbox)
  * uncheck the other remaining boxes
5. Add new URL :
  * https://api.telegram.org
6. Locate the Navigation Bar on the Top of platform
7. Click on **View**
8. Click on **Navigator** and you will see Navigator Window embedded into the Platform
9. Double Click on **Expert Advisors** and this will show all your robots
10. Drag and Drop **Telegram_Trader** on to any Open Chart ( anytime Time-Frame, any Market is ok)
  * Alternatively you can simply double-click the **Telegram_Trader** to attach the robot to the most recently selected chart that you have open. 
# Telegram_Trader Robot Guide 
| Input Variable | Value Description |
| ----------- | ----------- |
| Trading Experience Mode | Adjusts your lotsize from 0.01, 0.05, 0.1, 0.5, 1.0 (select,noob,fomo, expert, btfd,pro)
| Alternative Lotsize | Adjust your own lotsize if Trading Experience Mode = Select
|TELEGRAM_TOKEN | Insert your Telegram_Token |
| [PM @botfather](https://telegram.me/botfather) within the telegarm application (search box) | Type in **/newbot**, give a name, give the @handle_name_bot that you want your bot to have  , and copy paste the Telegram Token into the TELEGRAM_TOKEN. If you are stuck on this step, google "How to make a Telegam bot" |
|WHITE_LIST_USERS | Insert your telegram username here, unless you want to share the bot and your trading account with every Telegram User like I do ( So that users can demo the application and share the charts with a trading group.) |
|TEMPLATE_MAX | This is the number of custom templates you plan to navigate through, aka your visual elements(indicators) |
|TEMPLATES | list your template names with **;** seperating the names. Such as **MACD;ADX;BOLLINGERBANDS;ELLIOTWAVE;ETC;DEFAULT** |
| BOT_TEMPLATE_MAX | This is the number of custom templates you plan to navigate through to control your robots |
| BOT_TEMPLATES | list your template names with **;** seperating the names. Such as **BREAKOUT;MARKETMAKER;PUMPBOT** |
| TRADE_ID | The Order Id of your manual trades ( aka MAGIC_NUMBER: This is what MetaTrader calls the order# within the documents ) |
| ALLOW_TRADING | You can turn off the trading functions so that other telegram users can't trade your account if you share it within a trading group |
| CHART_WIDTH | pixles of the screenshot size |
| CHART_HEIGHT | pixles of the screenshot size |


  
