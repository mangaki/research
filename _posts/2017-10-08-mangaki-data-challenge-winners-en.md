---
layout: post
title: "Mangaki Data Challenge Winners"
---

(Cet article est aussi disponible [en français](/2017/10/06/mangaki-data-challenge-winners-fr/).)

## The Mangaki Data Challenge

<p align="center"><a href="https://mangaki.fr"><img src="/public/img/mangaki.png" style="display: inline; margin: 0" /></a></p>

From July 1 to October 1, [Mangaki](https://mangaki.fr) and the [Kashima Lab](http://www.ml.ist.i.kyoto-u.ac.jp/en/) of [Kyoto University](http://www.kyoto-u.ac.jp/en) organized the **Mangaki Data Challenge**.

The contest was announced at [Anime Expo](http://www.anime-expo.org) on July 2, 2017, in **Los Angeles**!

## Statement

Participants had to determine whether certain users are interested or not in some anime or manga. Competitors had access to Mangaki ratings as open data.

**Read the full problem statement** in [French](/2017/07/18/mangaki-data-challenge-fr/), [English](/2017/07/18/mangaki-data-challenge-en/) or [Japanese](/2017/07/18/jp/).

## Leaderboard

1st prize.

:   [**GeniusIke**](http://wattlebird.github.io/about/) (Microsoft, China), who wins a background artbook [Your Name.](https://mangaki.fr/anime/14495) and the OST of Shaft's [Fireworks](https://mangaki.fr/anime/18331) movie!  
- [Listen (legally) to Fireworks OST samples on YouTube.](https://www.youtube.com/watch?v=PLydu6Z6h_Q)
- [See the winning solution.](https://wattlebird.github.io/2017/10/02/Mangaki-data-challenge-1st-place-solution/)

<p align="center"><img src="/public/img/your-name-is-fireworks.jpg" /></p>

2nd prize.

:   **ηzw**, who wins a subscription to the anime streaming website [Wakanim](https://www.wakanim.tv).

<p align="center"><img src="/public/img/wakanim.jpg" /></p>

3rd prize.

:   **karekyasu**, who wins 2 collector [JoJolion](https://mangaki.fr/manga/5910) ecocups designed by [Sedeto](http://sedeto.fr).

<p align="center"><img src="/public/img/jojolion.png" /></p>

[**See the full leaderboard**](http://universityofbigdata.net/competition/5085548788056064?lang=en) on University of Big Data.

## What are the winning solutions?

The winner, **GeniusIke** (AUC = 86%), [described his solution in a blog post](https://wattlebird.github.io/2017/10/02/Mangaki-data-challenge-1st-place-solution/) and [published his code on GitHub](https://github.com/wattlebird/MangakiChallenge)!

Please note that a simple solution that predicts a linear combination of the training set allowed **BC** to reach the 5th place with 82.6% AUC!  
(See [the leaderboard](http://bit.ly/mangakidatachallenge) and [this notebook](https://github.com/mangaki/notebooks/blob/master/Mangaki%20Data%20Challenge.ipynb).)

## What is Mangaki's score?

We got 81% AUC with a *gradient boosting tree* with which we could have been 8th. [See our described solution!](https://github.com/mangaki/notebooks/blob/master/Mangaki%20Data%20Challenge.ipynb)

We are wondering, according to our recent research article ([BALSE](https://github.com/mangaki/balse), accepted at [MANPU 2017](http://manpu2017.imlab.jp)), if using posters would have allowed us to improve this score significantly!

## What countries did participate?

- France: 13
- Japan: 6
- US: 5
- China, Spain, Taiwan, Korea, Russia, India, Hungary, Mexico: 1

## Why did we organize this contest?

For the following reasons:

- Promote the [**Mangaki** open source project](https://github.com/mangaki/mangaki/)
- Publish our ratings in **open data**  
(some teachers are already using them in their courses, or [even in high school](https://github.com/mangaki/movielens/))
- Get more people involved in **data science competitions**

Follow us on [Twitter](https://twitter.com/mangakifr) and [Facebook](https://fb.me/mangakifr) to be informed of our next challenge!

And congrats again to all participants!
