---
layout: post
title: Systèmes de recommandation
---

Vous connaissez le principe, un utilisateur s'inscrit, rentre ses préférences, le système lui recommande des œuvres susceptibles de lui plaire.

![Les œuvres à Mangaki](/public/img/ratings.png)

## Particularités de mangaki.fr

- Les notes : **j'adore / j'aime / neutre / je n'aime pas / je veux voir / je ne veux pas voir**
- On peut vous recommander des mangas même si vous n'avez noté que des séries animées

## Plus proches voisins (KNN)

**Principe.** Trouver des utilisateurs qui vous ressemblent en matière de goûts pour vous recommander ce qu'ils ont aimé que vous n'avez pas vu.

- Quelles valeurs assigner à chaque rating (`favorite`, `like`, `willsee`, etc.) ?
- Combien de voisins choisir ? Pour estimer la valeur d'une œuvre, faut-il considérer les 15 plus proches voisins *ayant noté cette œuvre* ? C'est ce que @Karypis2008[^1] conseille.

[Voir le code de la KNN sur GitHub](https://github.com/mangaki/mangaki/blob/master/mangaki/mangaki/utils/knn.py)

## SVD

**Principe.** Trouver des profils types et répartir les utilisateurs selon cette base de profils types.

- Comment considérer les entrées manquantes ? On les replace par la moyenne.
- Avantage : on peut construire le Top 8000 d'un individu.

[Voir le code de la SVD sur GitHub, depuis scikit-learn](https://github.com/mangaki/mangaki/blob/master/mangaki/mangaki/utils/svd.py)

## De l'intérêt de la fonction d'erreur

- Quelle fonction d'erreur choisir ? La RMSE ou simplement compter le nombre de faux positifs et négatifs ? Dans @Karypis2008[^1], ils suggèrent plutôt une sorte d'Expected Utility qui pénalise plus les faux positifs que les faux négatifs.

 [^1]: @Karypis2008 *Information Gain through Clustered Neighbors*, dans [*Learning preferences of new users in recommender systems: an information theoretic approach*](http://preview.kdd.org/exploration_files/WebKDD08-Al-Rashid.pdf), ACM SIGKDD 2008.
