![Equipping Your Animoca Mind with Google Drive Access](assets/banner.png)

# Equipping Your Animoca Mind with Google Drive Access

Your Mind just unlocked Google Drive mastery. Create, read, and edit Google Docs and Sheets directly — no more copy-pasting, no more tab switching. This is a real agentic workflow setup: fast, no code, no headaches. ⚡️

## Step 1: Equip the skill

The Google Drive Suite skill gives your Mind the ability to handle your files instantly. To equip it, copy and paste this prompt directly to your Mind:

> Equip yourself with the app "Google_Drive_Suite" (ID: E71CEC8B-BE18-F111-AD1D-0EA9A5017E89)

Speed: instant. Your Mind now knows exactly how to create, read, and edit files in your Google Drive.

## Step 2: Quick Cloud Enable ☁️

Google Cloud Console is where you create a project and enable the three APIs your Mind needs. Head to [console.cloud.google.com](https://console.cloud.google.com/):

1. **Create** a New Project.
2. **Enable** 3 APIs: Google Drive API, Google Docs API, and Google Sheets API.

![Enable APIs in Google Cloud Console](assets/step-cloud-api.png)

It is just three toggles. Total time: ~20 seconds. ⏱️

## Step 3: The Final Handshake

OAuth credentials (Open Authorization) allow your Mind to securely access your Google Drive on your behalf. This is a two-part setup:

1. **OAuth Client ID:** Create a "Web App" Client ID at APIs & Services. Use the redirect URL `https://developers.google.com/oauthplayground` and download your Client Secret JSON file.

![OAuth Client Secret JSON](assets/step-oauth-client.png)

2. **Access & Refresh Tokens:** Use the [OAuth Playground](https://developers.google.com/oauthplayground/) with the scope `https://www.googleapis.com/auth/drive` to generate your Access token and Refresh token.

![OAuth Playground — Authorize APIs](assets/step-oauth-playground-1.png)

![OAuth Playground — Exchange tokens](assets/step-oauth-playground-2.png)

Paste the Auth code, tokens, and JSON into your Mind. **You're all set!** Your AI now lives inside Google Drive — create, edit, and automate.

Try it out today: [app.animocaminds.ai](https://app.animocaminds.ai)

## Useful links

- [Animoca Minds App](https://app.animocaminds.ai/)
- [Google Cloud Console](https://console.cloud.google.com/)
- [OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)

---
title: "Equipping Your Animoca Mind with Google Drive Access"
title_en: "Equipping Your Animoca Mind with Google Drive Access"
date: "2026-03-16"
author: "Animoca Minds"
language: "en"
content_type: "thread"
source_platform: "x"
source_url: "https://x.com/AnimocaMinds/status/2031684457795916072"
slug: "equipping-animoca-mind-google-drive-access"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2031684457795916072"
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/2026/03/16-equipping-animoca-mind-google-drive-access/en.md"
tags:
  - animoca-minds
  - google-drive
  - google-docs
  - oauth
  - agentic-workflow
  - no-code
---