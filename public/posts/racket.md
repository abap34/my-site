---
title: DrRacketがかなりおもしろIDEだった
author: abap34
date: 2023/10/02
tag: [日記, Racket, Lisp, Scheme]
twitter_id: abap34
github_id: abap34
mail: abap0002@gmail.com
ogp_url: https://images.dog.ceo/breeds/setter-english/n02100735_8071.jpg
description: Racketのソースコードに画像が貼れて流石にビビった...
url: https://abap34.com/posts/racket.html
site_name: abap34.com
twitter_site: @abap34
---

## DrRacket 衝撃の機能
今日で夏休みが終わって後期の授業が始まりました！早起きが辛い！！！


講義は、「関数型プログラミング基礎」というのが始まりました。

Schemeを使うと言われていたので、 [Schemeの環境構築とかもしておいておいたのですが](https://www.abap34.com/posts/hello_scheme.html)、
RacketというSchemeの方言を使うらしく、DrRacketというIDEを使えと言われました。

初回は「慣れるためにとりあえず使ってみて」というなんとも投げやりな感じだったのですが、指定されたサンプルコードを見ていると、


![!?](racket/main.png)

**！？** なんかソースコードに急にロケットの画像が入っています。えぇ...

つまり、

![終わった](racket/shohei.png)

(全然関係ないですが大谷選手ホームラン王おめでとうございます！！！！)


## 一応ソースコードの中身を見てみる
流石に衝撃的すぎます。一応 `main.rkt` の中身を見てみます。


ファイルの先頭を見ると、

```racket
#reader(lib"read.ss""wxme")WXME0111 ## 
#|
   This file uses the GRacket editor format.
   Open this file in DrRacket version 8.10 or later to read it.

   Most likely, it was created by saving a program in DrRacket,
   and it probably contains a program with non-text elements
   (such as images or comment boxes).

            http://racket-lang.org/
|#
 34 7 #"wxtext\0" 
3 1 6 #"wxtab\0"
1 1 8 #"wximage\0"
2 0 8 #"wxmedia\0"
4 1 34 #"(lib \"syntax-browser.ss\" \"mrlib\")\0"
1 0 36 #"(lib \"cache-image-snip.ss\" \"mrlib\")\0"
```

みたいなことが書いてあり、そもそも素(?)のracketのソースコードではなく、DrRacket前提のソースコードになっているみたいです。


続いて、

```racket
�PNG

   
IHDR   �   �   �>a�    IDATx�����,�u��9'"3k���_����pI��H��E-���y �Ȁm�?��������1����آ��F#Y�D��������w�U��q�CDV�{��"�@ݥnݪ�8��|ω�����ޓ\E�s�����^� 

...

IEND�B`�
```

みたいなのがあり画像のバイナリがそのまま入っていました。パワーを感じる。

## 今日のラーメン
後期になって学食がオープンしたので行ってきました。

机が広くて友達と喋りやすくて良さげです。

あとごま団子が謎に入荷していて良かったです。

![学食のラーメン](racket/ramen.jpeg)
