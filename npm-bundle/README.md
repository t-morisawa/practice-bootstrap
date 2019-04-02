
# Sassの編集を実際にやってみる（npmモジュール編）

## custom.scssを作る

```
$alert-border-radius: 0 !default;
```

## 逆順はだめで先にカスタムscssを読み込む

```
@import "custom";
@import "~bootstrap/scss/bootstrap";
```

## webpackをインストール
```
npm install --save-dev webpack
npm install --save-dev webpack-cli
```

## webpackの設定

webpack.config.jsをかく

## webpack compile
```
node_modules/.bin/webpack --config webpack.config.js
```

## fileプロトコルでcss in jsを使えない件について

```
[Deprecation] CSS cannot be loaded from `file:` URLs unless they end in a `.css` file extension.
index.html:9 Resource interpreted as Stylesheet but transferred with MIME type text/javascript: "file:///Users/taumu/prog/practice-bootstrap/npm-bundle/dist/main.js".
```

S3に上げてみたものの、2行目の警告は消えてくれない。

```
<link rel="stylesheet" href="./dist/main.js">
```

これがだめ。

```
<script src="./dist/main.js"></script>
```

こうする 

## 参考リンク

https://ics.media/entry/17749/
