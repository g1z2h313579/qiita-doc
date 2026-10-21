---
title: 使用 Qiita CLI 和 GitHub Actions 自动发布文章的测试
tags:
  - Qiita
  - QiitaCLI
  - GitHubActions
private: true
updated_at: ''
id: null
organization_url_name: null
slide: false
ignorePublish: true
posting_campaign_uuid: null
agreed_posting_campaign_term: false
---
# 前言

本文是一篇测试文章，用于确认使用 Qiita CLI 和 GitHub Actions 自动发布文章的流程是否正常运行。

# 机制

1. 在本地以 Markdown 文件形式编写文章
2. push 到 `main` 分支
3. GitHub Actions 执行 `qiita publish --all`，将文章发布或更新到 Qiita
4. 发布后，文章 ID 等元信息由 bot 提交回仓库

# 需要确认的内容

- 能够通过 `QIITA_TOKEN` secret 完成认证
- 文章能够在 Qiita 上创建
- 文章 ID 能够写回到仓库中
