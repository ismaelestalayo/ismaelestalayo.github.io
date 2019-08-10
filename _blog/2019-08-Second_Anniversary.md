---
layout: post
title: Second CryptoTracker Anniversary
date: 2019-08-20 17:00:00
image: assets/cryptotracker/hero-art.png
author: Ismael Estalayo
visible: false
---

Predicting crypto-currency prices and applying to portfolio optimization theory


We want to predict the ups and down of crypto-currencies with deep learning, so we will need to build a neural network which will theoretically see the future prices of crypto-coins, and then we will use that data to optimize our portfolio and get rich. 

But... how are we going to build that 'neural-network', and how is it supposedly going to predict the future? The answer is data... tons and tons of it. So our first step is going to be to get that data which we will then feed a model so it can try to learn how the market works. For that purpose I first layed my eyes on [CryptoCompare's API](https://min-api.cryptocompare.com/), which I knew beforehand because it's what I used for my app [CryptoTracker](https://www.microsoft.com/en-us/store/p/cryptotracker/9n3b47hbvblc). It's a pretty complete API, but it had a big flaw for this project: for data older than a week it only stored hourly and daily prices, and that wasn't going to be enough for a neural-network, so I kept searching till I found [Poloniex's API](https://poloniex.com/support/api/) which could give me historical prices with up to 5' of frequency!

Okay, so we have a data provider, now we only need to 'download' that data. For that purpose I'm gonna make a simple Python script which will call the API for a specific coin data since it's beggining with a 5 minute interval:


This short script is going to let us fetch easily the historic prices for each coin by just changing two parammeters: the string `crypto` to whatever crypto-currency we want, and the `startdate` on the URL. The result of running this script is going to be a .csv file with three parammeters on each line: the timestamp of that line's data (epoch format), the weighted average price on that timestamp, and the volume (bought and sold) for that coin:

|Epoch       |Price       |Volume    | 
|------------|------------|----------| 
| 1424373000 |  225       |  0.0044  | 
| 1424373300 |  225       |  0       | 
|  ........  |  ........  |  .....   | 
| 1520765100 |  8637.9644 |  3.9674  | 
| 1520765400 |  8677.6466 |  15.7817 | 
| 1520765700 |  8689.6037 |  22.0042 | 
| 1520766000 |  8695.0347 |  1.5001  |