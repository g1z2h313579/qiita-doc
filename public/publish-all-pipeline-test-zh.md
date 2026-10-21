---
title: 将一篇原稿一键发布到 Zenn、Qiita、note 的测试
tags:
- Python
- GitHubActions
- 自動化
private: true
updated_at: ''
id: null
organization_url_name: null
slide: false
ignorePublish: true
posting_campaign_uuid: null
agreed_posting_campaign_term: false
---

## 前言

本文是一篇测试文章，用于确认从一篇原稿一键发布到 Zenn、Qiita、note 的机制是否正常运行。

## 机制

1. 在 `articles/<slug>/` 下编写日文版和中文版原稿
2. 脚本生成各平台所需的文件
3. Zenn 和 Qiita 通过 git push 发布，note 通过 MCP 的库发布

## 图片

![示例图片](https://raw.githubusercontent.com/g1z2h313579/qiita-doc/main/images/publish-all-pipeline-test/sample.png)

## 代码

```python
# 代码块中的图片语法不会被改写: ![x](images/not-real.png)
print("hello")
```

## 表格

| 平台 | 发布方式 |
|---|---|
| Zenn | GitHub 联动 |
| Qiita | GitHub Actions |
| note | 非官方 MCP |
