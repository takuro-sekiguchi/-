# HTMLの疑似要素の練習

[今回作成したサイトはこちら](https://taku-web3.com/project/css-pseudo-element/index.html)    

___

## ■新しく学んだこと

- 疑似要素を使うと、HTMLを汚さずにレイアウトを加えることができる。
- SEO的に考えても疑似要素を使う方がいい
- imgタグには疑似要素を当てることはできないので注意

___

### gridで要素を中央寄せにする方法
```css
body {
 display: grid;
 place-items: center;
}
```

___

### font-sizeのremについて
remは「root em」の略で、CSS3から利用できる。  
HTMLの最上位要素であるhtmlタグの文字サイズを基準に設定され、親要素の影響を受けない。
```css
html { font-size: 62.5%; }
```
と記述することで、ブラウザのデフォルト設定の文字サイズが16px * 0.625 = 10pxとなるので、remを扱いやすくなる。

___


###　font-awesomeの使い方
```html
 <link
  rel="stylesheet"
  href="https://use.fontawesome.com/releases/v5.15.4/css/all.css"
  integrity="sha384-DyZ88mC6Up2uqS4h/KRgHuoeGwBcD4Ng9SiP4dIRy0EXTlnuz47vAwmeGwVChigm"
  crossorigin="anonymous"
/>
```
```css
.pseudo-element3 h1::before {
  content: "\f14a";
  font-family: "Font Awesome 5 Free";
}
```