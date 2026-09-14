# public-pages

顧客・関係者へ共有する、小さな静的Webページの公開用リポジトリです。GitHub Pages で公開します。

## 公開前レビュー（必須）

このリポジトリは Public です。**新規ページ・更新ページを commit / push / PR 作成する前に、AIエージェントによる公開可否レビューを行ってください。** GitHub Pagesへ反映される前でも、リポジトリへ入った時点で内容は閲覧可能です。

最低限、次を確認します。

- 氏名、住所、電話番号、メールアドレス、口座番号、マイナンバー等の個人情報
- PIN、パスワード、APIキー、トークン、Cookie、秘密鍵等の認証情報
- 正確なGPS座標、非公開URL、スプレッドシートID等の内部情報
- 給与実額、契約内容、未公開の経営・顧客情報
- HTML / JavaScriptからの意図しない外部送信・外部通信
- ページ目的に不要な情報
- 一般公開を目的としないページの `noindex,nofollow,noarchive`

レビュー結果は `公開可` / `修正後に公開可` / `公開不可` のいずれかを明示します。`公開可` になるまで公開リポジトリへ追加しません。

> `noindex` は検索結果への掲載を抑える指定であり、アクセス制御ではありません。URLを知っている人は閲覧できる前提で判断します。

## 構成

```text
public-pages/
├── index.html
├── AGENTS.md
├── .nojekyll
└── mikawaya/
    └── requirements-2026-09/
        └── index.html
```

公開URL:

- https://yitoworks.github.io/public-pages/
- https://yitoworks.github.io/public-pages/mikawaya/requirements-2026-09/

## 新しいページを追加する

案件・用途ごとにサブディレクトリを作り、原則として HTML / CSS / JavaScript だけで完結させます。認証やサーバー保存が必要な内容は、このリポジトリへ置かず別の方法を検討します。

## GitHub Pages 初回設定

GitHub の `Settings > Pages` で以下を設定します。

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/ (root)`
