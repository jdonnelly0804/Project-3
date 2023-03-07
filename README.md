# Project-3 - News Trading Bot + Sentiment Analysis 

---
## Project Overview:
This project is a mixture of two main coding projects that each have two different methods of getting essentially to the same end goal. There are four total notebooks. Two notebooks are intended to be a news trading bot that takes long/short positions on the market based on macroeconomic news. This includes the release of monthly CPI, fed FOMC decisions for rate hikes/cuts and also nonfarm payroll data. The first implementation of this is under "cpi_trade_twitter". This makes use of the twitter API as well as a known account that posts economic data using a bloomberg terminal. The data is then drawn from those tweets and used to make decisions to long/short the market.
>
The second file that trades news is called "cpi_trade_websocket". This notebook does the exact same thing that the first trading bot does, but the implementation allows it to be faster. This was a change I made to the code throughout the time that I was working out how to do this. Ultimately there are tons of people trying to bot this news and what success comes down to is who can be the first to get their trade in. I found that using a websocket was faster - due to the twitter API having a delay of a few seconds. 
> 
The third and fourth notebook are both machine learning code that are used to do sentiment analysis on tweets from twitter. I used the twitter API to pull hundreds of tweet with the keyword "Bitcoin" in it. After this I cleaned up the tweets and then performed sentiment analysis on them. The first attempt uses 'Textblob' a natural language processing library that can perform sentiment analysis on text. The second notebook - the SVM analysis - was my attempt at creating some machine learning model that could properly figure out sentiment. I personally labeled over 100 tweets that I pulled with either being positive or negative sentiment and then used a SVM model to predict on tweets. The overall accuracy was around 69%, so not great. 

---
## Usage and Installation:
In order to use the code from these notebooks you would need to download the proper libraries for the imports. On top of this you would need to create a twitter account and get twitter API keys as well as setup your twitter account on twitters development website. Once you do this you can authorize pulling tweets with your own account and go from there. You would also need to familiarize yourself with websockets, download the library, and find a website that has a live websocket feed or use the websocket that I used.

---
## Results and Summary:
