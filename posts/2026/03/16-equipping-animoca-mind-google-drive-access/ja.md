![ガイド：Animoca MindにGoogleドライブアクセスを付与する](assets/banner.png)

# ガイド：Animoca MindにGoogleドライブアクセスを付与する

このガイドでは、Animoca MindをGoogleドライブに接続し、ドキュメントの作成・読み取り・編集ができるようにするための正確な手順を提供します。

## フェーズ1：BazaarからAppを装備する

1. Skills BazaarのGoogle_Drive_suiteに直接アクセスする：[https://app.animocaminds.ai/bazaar/apps/E71CEC8B-BE18-F111-AD1D-0EA9A5017E89](https://app.animocaminds.ai/bazaar/apps/E71CEC8B-BE18-F111-AD1D-0EA9A5017E89)
2. プロンプトをコピーしてMindに送信することで、このAppをMindに装備する。

## フェーズ2：Google Cloudプロジェクトを作成してAPIを有効化する

1. [Google Cloud Console](https://console.cloud.google.com/)にアクセスし、MindにアクセスさせたいドライブのGoogleアカウントでログインする。
2. 新しいプロジェクトを作成する。
3. **「APIとサービス」**に移動し、以下の3つのAPIを有効化する：
   - Google Drive API
   - Google Docs API
   - Google Sheets API

## フェーズ3：OAuth認証情報を生成する

1. **「APIとサービス」**で、追加したAPIの詳細ページに移動する。
2. **「認証情報を作成」**をクリックし、**OAuthクライアントID**を選択する。
3. OAuth設定を入力する：
   - **アプリケーションの種類：** ウェブアプリケーション
   - **名前：** [任意の名前を入力]
   - **承認済みのリダイレクトURI：** [必須]（テスト用）[https://developers.google.com/oauthplayground](https://developers.google.com/oauthplayground)
4. 設定が完了したら、**「Client Secret JSON」**ファイルをコンピューターにダウンロードする。

## フェーズ4：認証コードとトークンを生成する

1. [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)にアクセスする。
2. **ステップ1：APIを選択して承認する**
   - スコープ入力フィールドを見つける。
   - 入力：`https://www.googleapis.com/auth/drive`
   - **「Authorize APIs」**をクリックする（サインインと権限付与が求められる）。
3. **ステップ2：認証コードをトークンに交換する**
   - Playgroundが生成した**[認証コード]**をコピーする。
   - コードを交換するボタンをクリックする。
   - これにより**[リフレッシュトークン]**と**[アクセストークン]**が生成される。

## フェーズ5：認証情報をMindに提供する

1. [https://app.animocaminds.ai/](https://app.animocaminds.ai/)のAnimoca Mindに戻る。
2. 収集した以下の情報をMindに提供する：
   - **[認証コード]**
   - **[アクセストークン]**
   - **[リフレッシュトークン]**
   - **Client Secret JSON**ファイル

これでMindはGoogleドライブ内のファイルを直接作成、読み取り、書き込みできるようになります。

## 関連リンク

- [Animoca Mindsプラットフォーム](https://app.animocaminds.ai/)
- [Skills BazaarのGoogle_Drive_suite](https://app.animocaminds.ai/bazaar/apps/E71CEC8B-BE18-F111-AD1D-0EA9A5017E89)
- [Google Cloud Console](https://console.cloud.google.com/)
- [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)

---
title: "ガイド：Animoca MindにGoogleドライブアクセスを付与する"
title_en: "Guide: Equipping Your Animoca Mind with Google Drive Access"
date: "2026-03-16"
author: "Animoca Minds"
language: "ja"
content_type: "article"
source_platform: "x"
source_url: "https://x.com/AnimocaMinds/status/2031684457795916072"
slug: "equipping-animoca-mind-google-drive-access"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2031684457795916072"
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/2026/03/16-equipping-animoca-mind-google-drive-access/ja.md"
tags:
  - animoca-minds
  - google-drive
  - oauth
  - google-cloud
  - integration
  - tutorial
---