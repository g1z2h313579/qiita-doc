---
title: Qiita CLI と GitHub Actions による記事自動公開のテスト
tags:
  - Qiita
  - QiitaCLI
  - GitHubActions
private: true
updated_at: ''
id: null
organization_url_name: null
slide: false
ignorePublish: false
posting_campaign_uuid: null
agreed_posting_campaign_term: false
---
# はじめに

この記事は、Qiita CLI と GitHub Actions を使った記事自動公開の動作確認用テスト記事です。

# 仕組み

1. ローカルで Markdown ファイルとして記事を書く
2. `main` ブランチに push する
3. GitHub Actions が `qiita publish --all` を実行し、Qiita に記事を公開・更新する
4. 公開後、記事 ID などのメタ情報が bot によってリポジトリにコミットされる

# 確認したいこと

- `QIITA_TOKEN` シークレットで認証できること
- 記事が Qiita 上に作成されること
- 記事 ID がリポジトリに書き戻されること
