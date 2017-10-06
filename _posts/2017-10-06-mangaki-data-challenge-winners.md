---
layout: post
title: "Palmarès du Mangaki Data Challenge"
---

## Le Mangaki Data Challenge

<p align="center"><a href="https://mangaki.fr"><img src="/public/img/mangaki.png" style="display: inline; margin: 0" /></a></p>

Du 1er juillet au 1er octobre, l’association [Mangaki](https://mangaki.fr) et le [Kashima Lab](http://www.ml.ist.i.kyoto-u.ac.jp/en/) de [l’université de Kyoto](http://www.kyoto-u.ac.jp/en) ont organisé le **Mangaki Data Challenge**.

Le concours a été annoncé à [Anime Expo](http://www.anime-expo.org) le 2 juillet 2017, à **Los Angeles** !

## Énoncé

Les participants devaient déterminer si certains utilisateurs ont envie de lire certains mangas ou s'ils n'ont pas envie de les lire, à partir du profil de tous les utilisateurs du site.

**Voir l’énoncé complet** en [français](/2017/07/18/mangaki-data-challenge-fr/), [anglais](/2017/07/18/mangaki-data-challenge-en/) ou [japonais](/2017/07/18/jp/).

## Palmarès

1er prix.

:   [**GeniusIke**](http://wattlebird.github.io/about/) (Microsoft, China), qui gagne un background artbook [Your Name.](https://mangaki.fr/anime/14495) et l’OST du film [Fireworks](https://mangaki.fr/anime/18331) (Shaft) qui sortira en France le 3 janvier 2018 !  
- [Écouter des extraits de l'OST de Fireworks sur YouTube.](https://www.youtube.com/watch?v=PLydu6Z6h_Q)
- [Voir la solution du gagnant.](https://wattlebird.github.io/2017/10/02/Mangaki-Data-challange-1st-place-solution/)

<p align="center"><img src="/public/img/your-name-is-fireworks.jpg" /></p>

2e prix.

:   **ηzw**, qui gagne un abonnement à [Wakanim](https://www.wakanim.tv).

<p align="center"><img src="/public/img/wakanim.jpg" /></p>

3e prix.

:   **karekyasu**, qui gagne 2 ecocups collector [JoJolion](https://mangaki.fr/manga/5910) par [Sedeto](http://sedeto.fr).

<p align="center"><img src="/public/img/jojolion.png" style="display: inline" /><img src="/public/img/jojolion.png" style="display: inline" /></p>

[**Voir le palmarès complet**](http://universityofbigdata.net/competition/5085548788056064?lang=en) sur University of Big Data.

## Quelles sont les solutions des gagnants ?

Le gagnant, **GeniusIke** (AUC = 86 %), a [décrit sa solution dans un billet de blog](https://wattlebird.github.io/2017/10/02/Mangaki-Data-challange-1st-place-solution/) et a [publié son code sur GitHub](https://github.com/wattlebird/MangakiChallenge) !

À noter que la simple solution consistant à prédire une combinaison linéaire du training set a permis à **BC** d’arriver 5e avec une AUC de 82.6 % !  
(Cf. [le palmarès](http://bit.ly/mangakidatachallenge) ainsi que [ce notebook](https://github.com/mangaki/notebooks/blob/master/Mangaki%20Data%20Challenge.ipynb).)

## Quel est le score de Mangaki ?

Une AUC de 81 % avec un *gradient boosting tree* qui nous aurait fait arriver 8e. [Voir notre solution !](https://github.com/mangaki/notebooks/blob/master/Mangaki%20Data%20Challenge.ipynb)

On se demande avec notre récent travail de l’été ([BALSE](https://github.com/mangaki/balse), accepté à [MANPU 2017](http://manpu2017.imlab.jp)) si utiliser les posters aurait permis d’améliorer ce score significativement !

## Quels pays ont participé ?

- France : 13
- Japan : 6
- US : 5
- China, Spain, Taïwan, Korea, Russia, India, Hungary, Mexico : 1

## Pourquoi organiser ce concours ?

Plein de raisons !

- Parler du [projet open source **Mangaki**](https://github.com/mangaki/mangaki/)
- Promouvoir nos ratings en **open data**  
(certains professeurs peuvent les utiliser dans leurs cours)
- Intéresser plus de gens aux **compétitions de data science**

Suivez-nous sur [Twitter](https://twitter.com/mangakifr) et [Facebook](https://fb.me/mangakifr) pour être au courant du prochain challenge !

Et encore bravo à tous les participants !
