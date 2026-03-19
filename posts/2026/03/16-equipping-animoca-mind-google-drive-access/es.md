![Guía: Equipa tu Animoca Mind con acceso a Google Drive](assets/banner.png)

# Guía: Equipa tu Animoca Mind con acceso a Google Drive

Esta guía te proporciona los pasos exactos para conectar tu Animoca Mind a Google Drive, otorgándole la capacidad de crear, leer y editar documentos.

## Fase 1: Instala la habilidad

2. Equipa esta aplicación a tu Mind copiando el prompt y enviándoselo.

## Fase 2: Crea un proyecto de Google Cloud y activa las APIs

1. Ve a la [Consola de Google Cloud](https://console.cloud.google.com/) e inicia sesión con la cuenta de Google asociada al Drive.
2. Crea un nuevo proyecto.
3. Ve a **"APIs y servicios"** y activa: Google Drive API, Google Docs API, Google Sheets API.

## Fase 3: Genera las credenciales OAuth

1. En **"APIs y servicios"**, haz clic en **"Crear credenciales"** → **ID de cliente OAuth**.
2. App type: Aplicación web. Authorized redirect URI (testing): https://developers.google.com/oauthplayground
3. Descarga el archivo **"Client Secret JSON"**.

## Fase 4: Genera el código de autorización y los tokens

1. Ve al [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/).
2. Scope: `https://www.googleapis.com/auth/drive` → **Authorize APIs**.
3. Intercambia el código por tokens: obtendrás un **[Refresh token]** y un **[Access token]**.

## Fase 5: Proporciona las credenciales a tu Mind

1. Regresa a [https://app.animocaminds.ai/](https://app.animocaminds.ai/).
2. Proporciona: [Código de autorización], [Access token], [Refresh token], Client Secret JSON.

Tu Mind ahora podrá crear, leer y escribir archivos en tu Google Drive.

## Enlaces útiles

- [Plataforma Animoca Minds](https://app.animocaminds.ai/)
- [Consola de Google Cloud](https://console.cloud.google.com/)
- [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground/)

---
title: "Guía: Equipa tu Animoca Mind con acceso a Google Drive"
title_en: "Guide: Equipping Your Animoca Mind with Google Drive Access"
date: "2026-03-16"
author: "Animoca Minds"
language: "es"
content_type: "article"
source_platform: "x"
source_url: "https://x.com/AnimocaMinds/status/2031684457795916072"
slug: "equipping-animoca-mind-google-drive-access"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2031684457795916072"
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/2026/03/16-equipping-animoca-mind-google-drive-access/es.md"
tags:
  - animoca-minds
  - google-drive
  - oauth
  - google-cloud
  - integration
  - tutorial
---