---
layout: post
title: Visualize anime embeddings
---

So actually in Mangaki, [our algorithms](https://github.com/mangaki/mangaki/tree/master/mangaki/mangaki/algo) allow us to learn a latent representation (also called *embedding*) of every [anime](https://mangaki.fr/anime/) or [manga](https://mangaki.fr/manga/) and every <span style="color: #f60">user</span>, so that **people like anime in their direction**.

![Embeddings in Mangaki](/public/img/embeddings.png)

So for example, people who like [***Steins;Gate***](https://mangaki.fr/anime/16) and [***Durarara!!***](https://mangaki.fr/anime/20) are usually not the same than the ones that like [***Fairy Tail***](https://mangaki.fr/anime/18) or [***Naruto***](https://mangaki.fr/anime/4).

Using your ratings, we can find where you are in this map, and provide recommendations to you accordingly.

![Where are you?](/public/img/here.png)

To know more, here are some resources:

- [The notebook that generated this map](https://github.com/mangaki/notebooks/blob/master/III%20-%20Visualize%20anime%20embeddings.ipynb)
- [Our presentation (video) in Hacker News Kansai in July 2018](https://www.youtube.com/watch?v=nE_rHgfpKms)

And as I was bored, I provided here a [t-SNE](https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding) embedding on France's map. We called it [**Mangaki on Earth**](http://mangaki.fr/map) (MoE).

[![Mangaki embeddings on France map](/public/img/maps.jpg)](https://mangaki.fr/map)

If you want to know where you are on the map, feel free to <a href="mailto:jj@mangaki.fr">get in touch</a>!
