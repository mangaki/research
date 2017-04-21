---
layout: post
title: Test our algorithms on Movielens!
---

You can run [our 5-fold cross validation](https://github.com/mangaki/mangaki/blob/master/mangaki/mangaki/management/commands/compare.py) on the Movielens dataset.

Download the Movielens dataset prepared by our team:

- [ratings-ml.csv](https://mangaki.fr/static/data/ratings-ml.csv)
- (optional) [works-ml.csv](https://mangaki.fr/static/data/works-ml.csv) if you want to know the titles of the movies

Clone the GitHub repo and:
    
    git clone git@github.com:mangaki/mangaki.git
    cd mangaki
    python3 -m venv venv
    . venv/bin/activate
    pip install -r requirements.txt
    # Put the ratings-ml.csv file in the data folder
    ./mangaki/manage.py compare movies

It will run everything and display:

    Final results
    als-20: RMSE = 1.122326
    svd-20: RMSE = 1.157234

Feel free to modify the `mangaki/mangaki/management/commands/compare.py` file to compare more algorithms.
