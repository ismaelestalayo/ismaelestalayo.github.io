---
layout: post
title: Crypto Tracker 6.0
date: 2021-09-01 15:00
description: New v6 update for Launch 2021 event
image: https://ismaelestalayo.com/blog/2021/CryptoTracker6/Hero-art.png
author: Ismael Estalayo
visible: true
---


<style>
  img {
    filter: drop-shadow(0px 0px 4px #00000088);
    border-radius: 4px;
  }
  @media (prefers-color-scheme: dark) {
    img {
      filter: drop-shadow(0px 0px 4px #ffffff88);
    }
  }
</style>

After months in the work the 6th big update of CryptoTracker is finally out AND is part of the incredible [Launch 2021](https://uwpcommunity.com/launch/2021/) event, the third annual event of its kind where the UWP community comes together and releases their projects into the wild.
As an already existing app, CryptoTracker has been updated packed with **new features**, a huge **UI overhaul** and a faster and cleaner code (thanks to the MVVM Toolkit).

But before diving into all the changes, this is also a moment to celebrate multiple milestones. In the one hand, this year has been the first one with **user donations** for which I'm incredibly greateful for, and that has personally meant a lot to me. In the other hand, just a week short of its 4th anniversary (August 22nd, 2017), CryptoTracker reached the **50k acquisitions** achievement, which makes me extremely humbled knowing this all started as a summer side-project.

<blockquote style="margin: auto" class="twitter-tweet tw-align-center" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">Excited and humbled to share that Crypto Tracker has surpassed the 50k acquisitions milestone!🎉<br><br>Can&#39;t wait to launch what I&#39;ve been working on for the last months! 🚀 <a href="https://twitter.com/hashtag/UWP?src=hash&amp;ref_src=twsrc%5Etfw">#UWP</a> <a href="https://t.co/G6wMxWVkuP">pic.twitter.com/G6wMxWVkuP</a></p>&mdash; ismael (@ismaelestalayo) <a href="https://twitter.com/ismaelestalayo/status/1427031443285360642?ref_src=twsrc%5Etfw">August 15, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>



## Changelog
Without further ado let's get into all the nitty-gritty details about the update:


### New Home layout
The double column layout is gone, combining the price and volume charts into a single card. This also results in easier correlations of volume trends with price fluctuations besides looking more elegant:

<picture>
  <source srcset="../CryptoTracker6/Home-light.png" media="(prefers-color-scheme: dark)">
  <img src="../CryptoTracker6/Home-dark.png" class="post-center-img"
     style="width: 85vw; max-width: 900px;">
</picture>


### Refined coin view
Each coin's page has been redesigned following a card layout inspired by Windows 11. Like the Home page, the price and volume charts have been merged into one and a **new candle-chart** is also available. New to this page as well is the bottom card showing you all your holdings of the current coin:

<picture>
  <source srcset="../CryptoTracker6/coin-light.gif" media="(prefers-color-scheme: dark)">
  <img src="../CryptoTracker6/coin-dark.gif" class="post-center-img"
     style="width: 85vw; max-width: 900px;">
</picture>

Last but not least, this page has a couple of aces up its sleeve. At the top of the page live buttons to show information about a coin, as well as the ability to change to the **Compact Overlay** view, pin a **Live Tile** to the Start Menu and set custom **price threshold alerts**.

### Portfolio
The portfolio section has been vastly improved as well. At the top of the page your portfolio's **diversification rates** will be shown in a colorful and visual way. There's also a new **backup import/export** feature so you never lose your portfolio (or to have multiple).

<picture>
  <source srcset="../CryptoTracker6/portfolio-light.gif" media="(prefers-color-scheme: dark)">
  <img src="../CryptoTracker6/portfolio-dark.gif" class="post-center-img"
     style="width: 85vw; max-width: 900px;">
</picture>

Finally, the ability to **sort and duplicate** purchases has been added, as well as the option to temporarily group all purchases by coin, to combine all the same coin's holdings in a single entry and show its total stats.


### Support for 800+ cryptos
The ammount of supported alt-coins has been greatly increased (thanks to the use of different APIs), and the Coins page has been substantially improved making it **more information-dense** with an added historic chart (plus **sortable columns** have been added):
<picture>
  <source srcset="../CryptoTracker6/Coins-light.png" media="(prefers-color-scheme: dark)">
  <img src="../CryptoTracker6/Coins-dark.png" class="post-center-img"
     style="width: 85vw; max-width: 900px;">
</picture>


### Wrapping up
In addition to all the aforementioned features, a handful of bug-fixes have been included as improved app speeds largely thanks to the [MVVM Toolkit](https://docs.microsoft.com/en-us/windows/communitytoolkit/mvvm/introduction), which has also resulted in a **more mantainable code**.

Lastly, I'd like to use these last lines to thank the entire [UWP community](https://uwpcommunity.com/) and the amazing mods behind it that made this event possible. Also a huge shotout to everyone that has ever downloaded, rated, sent feedback or even donated for CryptoTracker as this wouldn't have been possible without you!


<!--

After a long hiatus without any important new features, this new update is filled with them (and the obvious bugfixes along the way):

Simple yet powerful cryptocurrency portfolio tracker designed with simplicity and functionality in mind.

- Minimal yet powerful cryptocurrency portfolio tracker designed with simplicity and functionality in mind.
- Choose from over 800 crypto and 15 fiat currencies
- Personal finance tracker that helps you manage your portfolio of cryptocurrencies in a single place.
- Follow the evolution of cryptocurrency markets
- Track all your cryptocurrency holdings in one place
- Simply add your transactions to the app, and let it track its earnings
- Conversion tool between any currency

-->