# note-mkdocs

このリポジトリは、mkdocsを手軽に使う方法についてまとめたリポジトリ

## Motivation

- コンピュータに処理させたいことを、手軽にコーディングしたい
- しかし、納得するコーディング例を見つけるまで、文献調査と試行錯誤に時間がかかる
- そこで、一度調べたコーディング例を、手軽に記録・更新・検索できる mkdocs にまとめておく
- その結果、一度調べたコーディング例であれば、時間をかけずにコーディングできるようになる

## Contibution

1. issueを書き、milestone、projectを付与する
   - タイトル：コンピュータに処理させたいこと
   - 説明文：モチベーション、コーディング例、実行結果、参考文献
1. issue を ToDo から In Progress へ移し、記事を書く（ただし、In Progress は４つまで）
1. 執筆した記事を docs フォルダに移し、リモートリポジトリを更新する
1. GitHub Pages に反映されたか確認する

## Role

- issue: 各記事、mkdocs におけるサイドバー（プライマリ）
- issueのセクション：各記事のセクション、mkdocs におけるサイドバー（セカンダリ）
- milestone: 各記事のカテゴリ、mkdocs におけるナビゲーションバー
- project：書く記事（issue）を管理するカンバンボード
   - ToDo：これから書く記事
   - In Progress：今書いている記事（WIP：4）
   - Done：書き終えた記事
- branch：現在書いている最中の記事

## Reference

- [Mkdocs](https://www.mkdocs.org/)
- [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/)
