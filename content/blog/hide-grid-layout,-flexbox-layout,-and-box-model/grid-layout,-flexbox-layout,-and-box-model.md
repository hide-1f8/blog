---
title: Grid Layout, Flexbox Layout, and Box Model  
date: "2020-10-26T07:18:49.034Z"
description: グリッドレイアウト、フレックスボックスレイアウト、ボックスモデルについて。
author: Hide
---


今回は、最近学習した、グリッドレイアウト、フレックスボックスレイアウト、ボックスモデルについて書いていきます。

## グリッドレイアウト
入社前に使っていた本には登場せず、いじったことは無かったが、  
書店でよく「グリッドデザイン」というワードが書かれた本を見かけ、少し調べたことはあったので、  
「先に枠を作ってから、その枠にコンテンツを当てはめていくもの」くらいの理解をしていた。  

入社前、html、css、JavaScriptの初心者用の本を終えて、次に何を学ぶか迷っていた時に、  
書店でbootstrapというワードを見かけた。  
少し読むと、グリッドデザインを用いたフレームワークだと分かった。  
CSSは、位置の干渉を、イメージした通りに調整するのが難しそうなので、  
グリッドデザインは細かい位置調整には不向き化もしれないけど、  
意図していないデザインにならないページを簡単に作成するのには  
向いていると思った。

Codecademyでの学習が初めてグリッドデザインに触れる場になった。  
進めていくと似たプロパティ名が多く登場して、枠内へのコンテンツの配置方法も種類があって、  
しっかり区別、記憶ができていない状態となり、説明を読んでも理解ができなくなった。  
その時点で、紙にレイアウトやそれぞれの要素に加えられた設定を描き・書き加えながら、復習し、概念やプロパティも区別していくことで、  
スムーズに先に進めるようになった。  

## フレックスボックスレイアウト
Codecademyでは受講コースに含まれていなかったので、  
主にmozilaのサイトで学んだ。  
初心者用の本で学んだことはあったが、  
それよりもずっと複雑だった。  
途中で、グリッドデザインで学んだ内容や、似た名前のプロパティの使い方が区別できなくなり、  
それらを学びなおして、学習がすすむようになった。  
mozilaのサイトでは、扱うテーマごとに細かく説明がされている。  
その内容も、説明文の近くに設けられた、サンプルコードとその表示例（自分でコードを書き換えて挙動の変化を確認できる）があるので、  
理解し易い。  

ここで、どんなルールでそう動いているのか分からない挙動に気付いた場合、注意が必要になる。  
そのルールを「その場で調べる」のか、「その場で調べずに学習を進める」のか、選ぶ必要がある。  
疑問をすぐに解決しようとせず、少し読み進めると、ちゃんと学習内容として扱っている場合がある。  
「その場で調べる」とは、つまり、サンプルコードをいじったり、説明を読み直したり、他のサイトでも調べたりして、考えて、答えを得たり、おそらく答えだと思える仮説を作ることだ。時間がかかるが、このプロセスに慣れることが開発者には必要だと思う。  
「その場で調べずに学習を進める」とは、分からない部分は放っておいて、先の内容を学びに行くということだ。学習を進めていると、分からない部分をきちんと説明しているセクションがある場合がある。自分ではあまり調べず考えないので、時間はかからない。が、調べて考える能力は身につかない。  

現在ではあまりflexモデルは主流ではないらしいが、デザインを身に着けるには必須の知識だと思う。  

## ボックスモデル
webページ上では、あらゆる要素がボックスに見立てられて配置・表示されている。  
ボックスには種類があり、それぞれ異なるルールで配置・表示されている。  
htmlの要素は、それぞれ、デフォルトで、何かしらのボックスが適用されている。  
cssのdisplayプロパティでは、このデフォルト設定されたボックスを変更できる。  
インライン、ブロック、インラインブロック、フレックス、グリッドなどがある。  
ボックスの種類によって、そのボックスの内側にある要素に適用されるルール、そのボックスが外側にある要素とどう関係するのかを決めるルールが異なる。  
html要素のデフォルトのボックス、displayプロパティで設定できるボックスの挙動を理解・区別しておくことが大切だ。  
また、html要素には、ブラウザが、ボックスではなく、その要素に対して設定しているデフォルトの設定がある。  
（例：``<p>``のmarginプロパティ）  
ある要素の配置・表示が、ボックスによるものなのか、その要素自体に対してのブラウザのデフォルト設定によるものなのかも、区別して覚えないと、  
意図しない配置・表示が起こる。  
