---
layout: post
title: "Mangakiデータチャレンジ日本語"
---

(also [in English](/2017/07/18/mangaki-data-challenge-en/) / [en français](/2017/07/18/mangaki-data-challenge-fr/))

[Mangaki.fr](https://mangaki.fr)はユーザが (1)アニメ・マンガを評価し、(2)次に見るべきアニメ・マンガの推薦を受けるためのプラットフォームです。フランスの学生により運営され、コードは[GitHubで公開されています](https://github.com/mangaki/mangaki/)。興味がある人なら、誰でもMangakiの機械学習アルゴリズムの改善に参加することができます。 

このコンペティションでは、アニメ・マンガに対するユーザの評価の予測に取り組んでもらいます。データセットとして、実際のユーザによる評価結果が提供されます。外部データの利用は自由とします。また、どのようなプログラミング言語でも参加することができます。入賞者には、手法を宣伝する機会を[このウェブページ](http://universityofbigdata.net/competition/5085548788056064)にて提供します。

<dt>アニメ・マンガの評価の種類</dt>
<dd>
<p>Mangakiでは、ユーザが「視聴後」と「視聴前」の二種類の評価を行います：</p>
<p><img src="/public/img/challenge-ratings.png" alt="Types of ratings on Mangaki"> </p>
<p>視聴後の評価には以下の４種類があります：</p>
<ul>
<li><code>love</code>: とても気に入った</li>
<li><code>like</code>: 気に入った</li>
<li><code>neutral</code>: どちらでもない</li>
<li><code>dislike</code>: 気に入らなかった</li>
</ul>
<p>視聴前の評価には以下の２種類があります：</p>
<ul>
<li><code>willsee</code>: 見たい・読みたい</li>
<li><code>wontsee</code>: 見たくない・読みたくない</li>
</ul>
</dd>
<dt>訓練データ：train.csv</dt>
<dd>
<p><code>train.csv</code>には以下の情報が含まれます：</p>
<pre class="prettyprint highlight">user_id,work_id,rating
50,4041,0
508,1713,0
1780,7053,1
658,8853,0
1003,9401,0
...</pre>
<p>各行は以下の情報を表します：</p>
<ul>
<li><code>user_id</code>: ユーザID（0から1982の間）</li>
<li><code>work_id</code>: 作品ID（0から9896の間）</li>
<li><code>rating</code>: 視聴前評価。<code>1</code>は<code>willsee</code>、<code>0</code>は<code>wontsee</code>を表す。</li>
</ul>
<p>例えば、<code>1780,7053,1</code>は、「ユーザ#1780は 作品#7053を見ていないが、その
作品を見たい（読みたい）と思っている」ことを表します。</p></dd>
<dt>テストデータ：test.csv</dt>
<dd>
<p><code>test.csv</code>には以下の情報が含まれます：</p>
<pre class="prettyprint highlight">user_id,work_id
486,1086
1509,3296
617,1086
270,9648
459,3647
...</pre>
<p>各行は以下の情報を表します：</p>
<ul>
<li><code>user_id</code>: ユーザID（0から1982の間）</li>
<li><code>work_id</code>: 作品ID（0から9896の間）</li>
</ul>
<p>テストデータ内のユーザID・作品IDについて、視聴前評価を予測して提出してください。具体的には、「<code>willsee</code>と評価する確率」を予測し出力してください。提出ファイルの例が<code>submission.csv</code>で示されています：</p>
<pre class="prettyprint highlight">user_id,work_id,prob_willsee
486,1086,XXX
1509,3296,XXX
617,1086,XXX
270,9648,XXX
459,3647,XXX
...</pre>
<p><code>XXX</code>に「<code>willsee</code>と評価する確率」を記述してください。</p>
</dd>
<dt>ボーナスデータ１：watched.csv</dt>
<dd>
<p><code>watched.csv</code>には視聴後予測の情報が含まれています：</p>
<pre class="prettyprint highlight">user_id,work_id,rating
717,8025,dislike
1106,1027,neutral
1970,3949,neutral
1685,9815,like
1703,3482,like
...</pre>
<p>各行は以下の情報を表します：</p>
<ul>
<li><code>user_id</code>: ユーザID（0から1982の間）</li>
<li><code>work_id</code>: 作品ID（0から9896の間）</li>
<li><code>rating</code>: 視聴後評価。<code>love</code>, <code>like</code>, <code>neutral</code>, <code>dislike</code>のいずれか。</li>
</ul>
<p>例えば、<code>717,8025,dislike</code>は、「ユーザ#717は作品#8025を見たが、その
作品を気に入らなかった」ことを表します。</p>
</dd>

[チャレンジはこちら](http://universityofbigdata.net/competition/5085548788056064)