# TradingSignals

## Logic behind this EA:
This ExpertAdvisor aims to alert the user for the following signals:

1) When Moving Average Crossover Indicator is Bullish (50 MA is above 200 MA) and price low is equal or below 200 MA, We get a Strong Buy signal.
2) When Moving Average Crossover Indicator is Bearish (50 MA is below 200 MA) and price high is equal or above 200 MA, We get a Sell signal.
3) When Moving Average Crossover Indicator's 50 MA Crossover 200 MA we get a Buy/Sell Signal.
4) When RSI is below 30 or above 70, Buy/Sell signal. 
5) When RSI is below 30 or above 70 and MACD crossover confirmed, Buy/Sell signal. If MACD crossover again, Close order singal.

All those signals are a sum of the strongest signals have shown us on his technical analysis videos here: https://www.patreon.com/InvestAnswers/posts?filters%5Btag%5D=Technical%20Analysis i'm open to suggestions and improvements.

## How to use it:
James suggest the following combinations:

### 1) **RSI & MACD** in this video https://www.youtube.com/watch?v=aPkGDuHC4_o are used in:

**Symbol:** BTCUSD, NEE, NVTA, PLTR, TTD, SNOW, BIDU, SHOP, ILMN

**Timeframe:** 4 Hours

**Settings:**

RSI
- Period: 10
- Price: Close

MACD
- Fast EMA Period: 8  
- Slow EMA Period: 21  
- Signal Period: 5
- Price: Close
- Mode: Signal
 
### 2) **MACO** in this video https://www.youtube.com/watch?v=JwBnwIVqJ8M is used in:

**Symbol:** Bitcoin, Ethereum, Google, Twitter, Gold etc.

**Timeframe:** Daily

**Settings:**
- Fast Moving Average Period: 50
- Slow Moving Average Period: 200
- Price: Close

## How to select signal combinations
The Expert Advisor and all those indicators will always use as timeframe your current timeframe.

Also the Expert Advisor have the following options:
![image](https://user-images.githubusercontent.com/10176426/116484126-16bad780-a891-11eb-8189-21f660fa0255.png)

- If you only want the RSI with MACD Combination, from **RSI with MACD Combination** select **RSI + MACD**  and set the **Enable Moving Averages CrossOver alerts (MACO)** to false.
- If you want RSI signals and MACO signals, from **RSI with MACD Combination** select **RSI** and set the **Enable Moving Averages CrossOver alerts (MACO)** to true.

## How to get Alerts:
I have implement 3 types of alerts.
1) A simple alertBox from MetaTrader platform
2) An email is sent for every alert
3) A mobile notification is sent for every alert

## Installation:
If you dont already use MetaTrader 4 but you still want to have free notification signals follow those steps:
1) Open a Demo account on any Forex Broker that supports MetaTrader 4 like ICMarkets here: https://www.icmarkets.com/global/en/open-trading-account/demo
2) Download MetaTrader 4 and connect it with your Demo account.

Now you will need to install a custom indicator. We need "MA crosses arrows or lines mtf+alerts.mq4", tt is included here in the repository, downloaded from here: https://forex-station.com/app.php/attach/file/3269743
You have to copy the *3-ma-cross-with-alert-mtf.mq4* file on **MQL4\Indicators** folder inside MetaTrader 4 installation. 
To access MetaTrader 4 installation folder:
1) Open MetaTrader 4
2) Click File / Open Data Folder

Also included you will find a Template that will make your chart look like James chart with RSI 20, MACross 50 and 200 and Simple Moving Average 10. To install it you have to put the *SMA20-MACO-RSI.tpl* file on **templates** folder. Open MetaTrader 4, right click on the chart and select **Template/Load Template** and select *SMA20-MACO-RSI.tpl* file.

Finally, the Expert Advisor file *InvestAnswerSignals.mq4* should placed on **MQL4\Experts**
Open MetaTrader 4, click on **View/Navigator** and double click on **InvestAnswersSignlas** from Expert Advisors tab to add this Expert Advisor to your chart. Once you included in your chart, it will show some options you can configure like where to get signal alerts or what settings to use on the Moving Average's.

## How to Setup Mobile Notifications:
1) Make sure from the Expert Advisor's Options that Mobile alerts are on.
2) On your Mobile download the MetaTrader 4 App.
3) Press **Menu/Settigns** and scroll down and find in the Messages section your **MetaQuotes ID**.
4) Add this ID to your Meta Trader 4 PC app on **Tools/Options/Notifications** at **MetaQuotes ID**.

## How to Setup Email Alerts:
1) Make sure from the Expert Advisor's Options that Email alerts are on.
2) From MetaTrader 4, go to **Tools/Options/Email**.
3) Add your email settings.

## Templates:
I have include 2 templates to try to match TradingView layout of James settings. 

**Notice:** Expert Advisor don't depend on those templates to work, as long as you have loaded the Expert Advisor to your chart, it will continue to work in any timeframe and any on screen indicator.
# RSI 10 - MACD 8 21 5
![image](https://user-images.githubusercontent.com/10176426/116484744-6948c380-a892-11eb-8e88-5d8fbcaade8a.png)
# RSI 10 - SMA 20 - MACO 50 200
![image](https://user-images.githubusercontent.com/10176426/116484962-d3616880-a892-11eb-8480-52f4e4592d5f.png)

## Tip Jar
Donations to motivate me to continue improoving this Expert Advisor are greatly appreciated :sparkling_heart:. If you want to find out how to tip me, check my profile page here: https://github.com/CDrosos
