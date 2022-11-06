# コードインラインを書く

コードブロックに含まれる一部のコードを、本文で引用しながら説明したいときがあります。
コードインラインは、本文の途中でコードにハイライトをつけて表示する方法です。
本ページでは、コードインラインを書く方法について説明します。

## 書く準備

はじめに、`mkdcos.yml` で次の `markdown_extensions` を有効にしておきます。

``` yaml title="mkdocs.yml"
markdown_extensions:
  - pymdownx.highlight:
      anchor_linenums: true
  - pymdownx.inlinehilite
  - pymdownx.snippets
  - pymdownx.superfences
```

## 書き方の一例

コードインラインは、コードをバッククォートで囲うことで、書くことができます。
さらに、バッククォートの先頭に `#!言語` （ここでは、`#!python`）をつけることで、ハイライトをつけることができます。
ここでは、`python` の `#!python print()` を題材に、その一例を示しています。

```` markdown title="コードインライン"
`python` の `#!python print()` は、括弧内の値を出力する関数です。
````

<div class="result" markdown>

`python` の `#!python print()` は、括弧内の値を出力する関数です。

</div>

## おわりに

本ページでは、コードインラインを書く方法について説明しました。
さらに詳細に知りたい方は、ぜひ参考文献を調べてみてください。

## 参考文献

- [Material for MkDocs: Highlighting inline code blocks](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/#highlighting-inline-code-blocks)
