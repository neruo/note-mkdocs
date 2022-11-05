# mkdocs 環境を構築する

## モチベーション

mkdocs で記事を閲覧する環境を構築したい

## 構築手順

### Step1. インストール

`pip` で `mkdocs-material` をインストールする

```shell
pip install mkdocs-material
```

### Step2. セットアップ

`mkdocs` コマンドで、プロジェクトを作成する

```shell
mkdocs new .
```

### Step3. サイト名の変更

お好みで、Webサイト名を変更する（ここでは、`note mkdocs` に変更）

``` yaml title="mkdocs.yml"
site_name: note mkdocs
```

### Step4. テーマの変更

お好みで、Webサイトに適用するテーマを変更する（ここでは、`material` テーマに変更）

```yaml title="mkdocs.yml"
theme:
  name: material
```

### Step5. プレビューする

記事をプレビューする

```shell
mkdocs serve
```
