# note-mkdocs

このリポジトリは、mkdocsを手軽に使う方法についてまとめたリポジトリ

## Motivation

- コンピュータに処理させたいことを、手軽にコーディングしたい
- しかし、納得するコーディング例を見つけるまで、文献調査と試行錯誤に時間がかかる
- そこで、一度調べたコーディング例を、手軽に記録・更新・検索できる mkdocs にまとめておく
- その結果、一度調べたコーディング例であれば、時間をかけずにコーディングできるようになる

## Contibution

1. コンピュータに処理させたいことを、issue のタイトルに書き、milestone、projectを付与する
2. issue の説明文に、次のことを書く
   - モチベーション、コーディング例、実行結果、参考文献
3. project で In Progress が4つ未満（WIP:4）であれば、issue を ToDo から In Progress に移す
4. その issue を実現する記事を、markdown で書く
5. 執筆した markdown を docs フォルダに移動し、リモートリポジトリを更新する
6. 執筆した markdown が反映されているか、GitHub Pages で確認する

## Role

- milestone: 各記事のカテゴリ、mkdocs におけるナビゲーションバー
- issue: 各記事、mkdocs におけるサイドバー（プライマリ）
- issueのセクション：各記事のセクション、mkdocs におけるサイドバー（セカンダリ）
- project：カンバン方式で書く記事を管理する
   - ToDo：これから書く記事
   - In Progress：今書いている記事（WIP：4）
   - Done：書き終えた記事

## Reference

- [Mkdocs](https://www.mkdocs.org/)
- [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/)
