# yantene/notes

yantene.net のコンテンツ正本 (Markdown + 画像アセット)。

- `notes/<slug>.md` — 記事本文 (フロントマター + Markdown)
- `notes/<slug>/<file>` — 記事に紐づく画像アセット

yantene.net の Worker が `POST /api/v1/notes/refresh` で本リポジトリを読み取り、
D1 (メタデータ) と R2 (パース済み MDAST・画像) に同期する。

## ブランチ運用
- `main` — production が読む
- `staging` — staging が下書き確認用に読む

## フロントマター
```yaml
---
title: 記事タイトル
publishedOn: 2010-01-06
lastModifiedOn: 2010-01-06
---
```
