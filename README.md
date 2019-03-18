
# Document
https://getbootstrap.com/docs/4.3/getting-started/introduction/

# memo
## theme
 
 https://getbootstrap.com/docs/4.1/getting-started/theming/
 
 Sassを使ってCSSを書いている。Lessは捨てたらしい。
 
 あまり詳しく読んでいないが参考になりそう。
 
## npm

VueやReactを使う場合はCDNではなくソースに含めてビルドすることもある。

その場合Bootstrapのコードを触ることになるので後ほど勉強するのもあり。

- https://getbootstrap.com/docs/4.1/getting-started/build-tools/
- https://getbootstrap.com/docs/4.1/getting-started/webpack/

## デザインガイドライン

https://getbootstrap.com/docs/4.1/getting-started/accessibility/

## Grid
```
<div class="container">
  <div class="row">
    <div class="col-sm">
      One of three columns
    </div>
    <div class="col-sm">
      One of three columns
    </div>
    <div class="col-sm">
      One of three columns
    </div>
  </div>
</div>
```

```
Containers provide a means to center and horizontally pad your site’s contents. Use .container for a responsive pixel width or .container-fluid for width: 100% across all viewport and device sizes.
Rows are wrappers for columns. Each column has horizontal padding (called a gutter) for controlling the space between them. This padding is then counteracted on the rows with negative margins. This way, all the content in your columns is visually aligned down the left side.
In a grid layout, content must be placed within columns and only columns may be immediate children of rows.
Thanks to flexbox, grid columns without a specified width will automatically layout as equal width columns. For example, four instances of .col-sm will each automatically be 25% wide from the small breakpoint and up. See the auto-layout columns section for more examples.
Column classes indicate the number of columns you’d like to use out of the possible 12 per row. So, if you want three equal-width columns across, you can use .col-4.
Column widths are set in percentages, so they’re always fluid and sized relative to their parent element.
Columns have horizontal padding to create the gutters between individual columns, however, you can remove the margin from rows and padding from columns with .no-gutters on the .row.
To make the grid responsive, there are five grid breakpoints, one for each responsive breakpoint: all breakpoints (extra small), small, medium, large, and extra large.
Grid breakpoints are based on minimum width media queries, meaning they apply to that one breakpoint and all those above it (e.g., .col-sm-4 applies to small, medium, large, and extra large devices, but not the first xs breakpoint).
You can use predefined grid classes (like .col-4) or Sass mixins for more semantic markup.
```

## utilities-for-layout

なんかオーバーライドしたい時に使えるらしい

https://getbootstrap.com/docs/4.1/layout/utilities-for-layout/

## Reboot

bootstrapのreset.cssの思想について書かれているので参考になるかもしれない

https://getbootstrap.com/docs/4.1/content/reboot/

## typography

全体の文字サイズ変えたいならこれ

https://getbootstrap.com/docs/4.1/content/typography/#responsive-typography

## パンくず

https://getbootstrap.com/docs/4.1/components/breadcrumb/

## コンポーネント

各パーツのデザイン思想が乗ってるので熟読しても良い

https://getbootstrap.com/docs/4.1/components

## 拡張する際の設計思想的な話

https://getbootstrap.com/docs/4.1/extend/approach/
## HTML
 - aria-label属性:アクセシビリティのためにつける
 - パンくずリストにはnav要素を使うとよい

## Bootstrapカスタマイズ
自前のCSSを使ってカスタマイズするのではなく、ソースコード取ってきてカスタマイズSassを使うべしとのこと。

```
Bootstrap 4を使うならSassを使って3倍幸せになろう
https://qiita.com/tonkotsuboy_com/items/1855734522bfe7ef7dad

Bootstrap 4 をカスタマイズする
https://qiita.com/pikanji/items/111cfb353bd6ec1eabb5
```
