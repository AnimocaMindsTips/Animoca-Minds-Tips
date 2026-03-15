![가이드: Animoca Mind에 Google 드라이브 접근 권한 부여하기](assets/banner.png)

# 가이드: Animoca Mind에 Google 드라이브 접근 권한 부여하기

이 가이드는 Animoca Mind를 Google 드라이브에 연결하여 문서를 생성, 읽기, 편집할 수 있는 능력을 부여하는 정확한 단계를 제공합니다.

## 1단계: Bazaar에서 앱 장착하기

1. Skills Bazaar에서 **Google_Drive_suite**에 접속: [https://app.animocaminds.ai/bazaar/apps/E71CEC8B-BE18-F111-AD1D-0EA9A5017E89](https://app.animocaminds.ai/bazaar/apps/E71CEC8B-BE18-F111-AD1D-0EA9A5017E89)
2. 프롬프트를 복사하여 Mind에게 전송.

## 2단계: Google Cloud 프로젝트 생성 및 API 활성화

1. [Google Cloud Console](https://console.cloud.google.com/)에서 로그인.
2. 새 프로젝트 생성.
3. **"API 및 서비스"**에서 활성화: Google Drive API, Google Docs API, Google Sheets API.

## 3단계: OAuth 자격증명 생성

1. **"자격증명 만들기"** → **OAuth 클라이언트 ID** 선택.
2. 앱 유형: 웹 애플리케이션. 리디렉션 URI (테스트): https://developers.google.com/oauthplayground
3. **"Client Secret JSON"** 파일 다운로드.

## 4단계: 인증 코드 및 토큰 생성

1. [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/) 접속.
2. 범위: `https://www.googleapis.com/auth/drive` → **Authorize APIs** 클릭.
3. 코드를 토큰으로 교환: **[리프레시 토큰]**과 **[액세스 토큰]** 획득.

## 5단계: Mind에 자격증명 제공

1. [https://app.animocaminds.ai/](https://app.animocaminds.ai/)의 Mind로 돌아가기.
2. 다음 제공: [인증 코드], [액세스 토큰], [리프레시 토큰], Client Secret JSON 파일.

Mind가 Google 드라이브에서 직접 파일을 생성, 읽기, 쓰기할 수 있습니다.

## 유용한 링크

- [Animoca Minds 플랫폼](https://app.animocaminds.ai/)
- [Google_Drive_suite](https://app.animocaminds.ai/bazaar/apps/E71CEC8B-BE18-F111-AD1D-0EA9A5017E89)
- [Google Cloud Console](https://console.cloud.google.com/)
- [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)

---
title: "Animoca Mind에 Google 드라이브 접근 권한 부여하기 가이드"
title_en: "Guide: Equipping Your Animoca Mind with Google Drive Access"
date: "2026-03-16"
author: "Animoca Minds"
language: "ko"
content_type: "article"
source_platform: "x"
source_url: "https://x.com/AnimocaMinds/status/2031684457795916072"
slug: "equipping-animoca-mind-google-drive-access"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2031684457795916072"
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/2026/03/16-equipping-animoca-mind-google-drive-access/ko.md"
tags:
  - animoca-minds
  - google-drive
  - oauth
  - google-cloud
  - integration
  - tutorial
---