# HTMLはじめのいっぽ

## HTMLとは？

HTMLとは、ハイパー テキスト マークアップ ランゲージ(Hyper Text Markup Language）の略で、テキストをタグで整理するコンピューター言語です。
プログラミング言語と違って、とってもシンプルなので、ご安心を！

基本は、こちら「たいとる」というテキストをh1というタグでマークアップすることで大きく目立たせます。
```
<h1>たいとる</h1>
```
&lt;と&gt;で囲まれたものをタグと呼びます。
先頭に / （スラッシュ）が付いた、タグは通称「閉じタグ」と呼び、そのタグの範囲の終わりを意味します。

HTMLは基本的に大きく2つ、表示されないヘッダと表示されるボディに別れます
```
<html>
<head> 〜 </head>
<body> 〜 </body>
</html>
```
このようにタグは入れ子にすることができます。思ったとおりに表示されない時は、ちゃんと閉じタグになっているか、閉じタグを忘れてないか確認してみましょう。

HTMLには様々なバージョンがありますが、最新版のHTMLであることを表す1行を先頭に付けて、文字コードは utf-8 であることをmetaタグで記述して完成です！

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8"/>
  <title>たいとる</title>
</head>
<body>
  <div>
  <h1>タイトル</h1>
  本文
  </div>
</body>
</html>
```
こちらを index.html と半角小文字で名前を付けて保存します。

ブラウザで開くか、ブラウザへドロップすると、カタカナで「タイトル」と書かれた超シンプルなページが表示できました！
ブラウザのタイトルは「たいとる」とひらがなで書かれています。上のHTMLと見比べてみましょう。

## divタグ

このようにHTMLは、1ページに、1ファイル作っていきます。ページ内に書く内容は自由ですが、ページのタイトル、小見出し、それぞれの本文という形が多いですね。
HTML内の何らかの固まりを divタグ で囲み、その先頭に大目次から順に h1, h2, h3, h4 とタイトルを付けて、本文を書いていきます。

```
<body>
<div>
  <h1>大タイトル</h1>
  <div>
    <h2>中タイトル1</h2>
    本文1
  </div>
  <div>
    <h2>中タイトル2</h2>
    本文2
  </div>
</div>
</body>
```


