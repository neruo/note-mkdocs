# コードブロックを書く

関数やクラスなど、まとまったコードを説明したいときがあります。
コードブロックは、まとまったコードをハイライト付きで読み手に示す方法です。
本ページでは、mkdocs でコードブロックを書く方法について説明します。

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

mkdocs では、3つのバッククォートでコードを囲うことで、次のようにコードブロックを書くことができます。
ここでは、[バブルソート関数](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/?h=code+blocks#adding-a-title)を題材に、その一例を示しています。


```` markdown title="コードブロック"
``` python
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
````

<div class="result" markdown>

``` py
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

</div>

mkdocs では、コードブロックをクリップボードへコピーする機能があります。
コードブロック内の右上のアイコンをクリックすると、コードブロックがテキストとしてコピーされます。

## オプション

コードブロックには、次のようなオプションをつけることができます。
このようなオプションをつけると、次のようにコードブロックをかっこよくできます。

<figure markdown>
|  オプション  |  書き方  |
| :---: | :---: |
|  コードブロック名を表示  |  `title="<custom title>"`  |
|  行番号を表示  |  `linenums="1"`  |
|  特定の行を強調  |  `hl_lines="<line number> ..."`  |
</figure>

```` markdown title="コードブロック"
``` python title="bubble_sort.py" linenums="1" hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
````

<div class="result" markdown>

``` py title="bubble_sort.py" linenums="1" hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

</div>

## おわりに

本ページでは、mkdocs でコードブロックを書く方法について説明しました。
さらに詳細に知りたい方は、ぜひ参考文献を調べてみてください。

## 参考文献

- [Material for MkDocs: Code blocks](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/)
