![指南：为您的Animoca Mind配置Google Drive访问权限](assets/banner.png)

# 指南：为您的Animoca Mind配置Google Drive访问权限

本指南提供了将Animoca Mind连接到Google Drive的精确步骤，使其能够创建、读取和编辑文档。

## 第一阶段：安装技能

1. 将以下命令发送给您的Mind来装备 **Google_Drive_suite**：

```
Equip yourself with the app "Google_Drive_Suite" (ID: E71CEC8B-BE18-F111-AD1D-0EA9A5017E89)
```
2. 复制提示词发送给Mind完成装备。

## 第二阶段：创建Google Cloud项目并启用API

1. 前往[Google Cloud Console](https://console.cloud.google.com/)登录。
2. 创建新项目。
3. 在**"API和服务"**中启用：Google Drive API、Google Docs API、Google Sheets API。

## 第三阶段：生成OAuth凭据

1. 点击**"创建凭据"** → **OAuth客户端ID**。
2. 应用类型：Web应用程序。授权重定向URI（测试）：https://developers.google.com/oauthplayground
3. 下载**"Client Secret JSON"**文件。

## 第四阶段：生成授权码和令牌

1. 前往[Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)。
2. 范围：`https://www.googleapis.com/auth/drive` → **Authorize APIs**。
3. 交换代码获取**[刷新令牌]**和**[访问令牌]**。

## 第五阶段：向Mind提供凭据

1. 返回[https://app.animocaminds.ai/](https://app.animocaminds.ai/)。
2. 提供：[授权码]、[访问令牌]、[刷新令牌]、Client Secret JSON文件。

Mind现在能够直接在Google Drive中创建、读取和写入文件了。

## 实用链接

- [Animoca Minds平台](https://app.animocaminds.ai/)
- [Google Cloud Console](https://console.cloud.google.com/)
- [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)

---
title: "指南：为您的Animoca Mind配置Google Drive访问权限"
title_en: "Guide: Equipping Your Animoca Mind with Google Drive Access"
date: "2026-03-16"
author: "Animoca Minds"
language: "zh-CN"
content_type: "article"
source_platform: "x"
source_url: "https://x.com/AnimocaMinds/status/2031684457795916072"
slug: "equipping-animoca-mind-google-drive-access"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2031684457795916072"
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/2026/03/16-equipping-animoca-mind-google-drive-access/zh-CN.md"
tags:
  - animoca-minds
  - google-drive
  - oauth
  - google-cloud
  - integration
  - tutorial
---