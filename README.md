# InvestAnswerIndicatorsSignals
Indicators with settings inspired from https://InvestAnswers.us Foudner James from https://www.patreon.com/InvestAnswers also you can find him on YouTube at https://www.youtube.com/channel/UClgJyzwGs-GyaNxUHcLZrkg | Fan made.

## Login behind this EA:
This ExpertAdvisor aims to alert the user for the following signals:

1) When Moving Average Cross Indicator is Bullish (50 MA is above 200 MA) and price low is equal or below 200 MA, We get a Strong Buy signal.
2) When Moving Average Cross Indicator is Bearish (50 MA is below 200 MA) and price high is equal or above 200 MA, We get a Sell signal.
3) When Moving Average Cross Indicator's 50 MA Crossover 200 MA we get a Buy/Sell Signal.
4) When RSI is above 70, Sell signal. 
5) When RSI is below 30, Buy signal. 

## How to use it:
James suggest to use Daily TimeFrame and he has demonstrated in his patreon videos https://www.patreon.com/InvestAnswers/posts?filters[tag]=Technical%20Analysis examples where those indicators was used for  Bitcoin, Ethereum, Google, Twitter, Gold etc.
The Expert Advisor will always use as timeframe your current timeframe.

## How to get Alerts:
I have implement 3 types of alerts.
1) A simple alertBox from MetaTrader platform
2) An email is sent for every alert
3) A mobile notification is sent for every alert

## Installation:
You will need to install a custom indicator first. We need "MA crosses arrows or lines mtf+alerts.mq4", tt is included here in the repository, Downloaded from here: https://forex-station.com/app.php/attach/file/3269743
You have to copy the *3-ma-cross-with-alert-mtf.mq4* file on **MQL4\Indicators** folder inside MetaTrader 4 installation. 
To access MetaTrader 4 installation folder:
1) Open MetaTrader 4
2) Click File / Open Data Folder

Also included you will find a Template that will make your chart look like James chart with RSI 20, MACross 50 and 200 and Simple Moving Average 10. To install it you have to put the *SMA20-MACO-RSI.tpl* file on **templates** folder.
Finally, the Expert Advisor file *InvestAnswerSignals.mq4* should placed on **MQL4\Experts**

## How to Setup Mobile Notifications:
1) If you dont already use MetaTrader 4 but you still want to have free notification signals follow those steps:
2) Open a Demo account on any Forex Broker that supports MetaTrader 4 like ICMarkets here: https://www.icmarkets.com/global/en/open-trading-account/demo
3) Download MetaTrader 4 and connect it with your Demo account
4) Add this Expert Advisor to your chart, Make sure from the Expert Advisor Options that Mobile alerts are on.
5) On your Mobile download the MetaTrader 4 App
6) Press menu/Settigns and scroll down and find in the Messages section your MetaQuotes ID
7) Add this ID to your Meta Trader 4 PC app on Tools/Options/Notifications at MetaQuotes ID.

## Tip Jar
Donations to motivate me to continue improoving this Expert Advisor are greatly appreciated. If you want to find out how to tip me, check my profile page here: 
