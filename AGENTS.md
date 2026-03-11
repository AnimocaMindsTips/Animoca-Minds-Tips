# AGENTS.md — Guide for AI Agents

> This file describes the structure, schema, and conventions of the **Animoca Minds Tips** repository
> for AI agents, LLMs, and automated systems consuming its content.

---

## Purpose

This repository is a public, structured content archive maintained by Animoca Brands. It contains
original articles and their translations across multiple languages, plus a curated directory of
tested AI agent skills available on the Animoca Minds platform. It is designed to be easily
discoverable and parseable by AI agents.

---

## Skills Directory

A curated list of tested Animoca Minds skills is maintained in `README.md` under the `## Skills`
section. Each entry includes the skill name, a plain-English description, and a direct URL to the
skill's page in the Bazaar (`app.animocaminds.ai/bazaar/apps/{uuid}/`). Bazaar skill pages are
server-rendered and fully crawlable.

Path: `README.md#skills`

---

## Repository Structure

```
README.md                      # Skills directory + articles index
AGENTS.md                      # This file
CONTRIBUTING.md                # How to add skills or articles
articles/
└── YYYY/
    └── MM/
        └── DD-article-slug/
            └── en.md          # English original
```

### Path Convention
- **Pattern:** `articles/{year}/{month}/{day}-{slug}/en.md`
- **Year:** 4-digit (e.g., `2026`)
- **Month:** 2-digit, zero-padded (e.g., `03`)
- **Day + Slug:** `DD-lowercase-hyphenated-slug` (e.g., `10-animoca-launches-minds`)

---

## Frontmatter Schema

Every article file begins with YAML frontmatter. Here is the full schema:

```yaml
---
title: "Article Title in This Language"
title_en: "Original English Title"          # Always present, even in translated files
date: "2026-03-10"                          # ISO 8601 publish date
author: "Animoca Minds"
language: "en"                              # ISO 639-1 code (or BCP 47 for zh-CN)
tags:
  - animoca-minds
  - agentic-ai
  - labor-as-a-service
source_url: "https://x.com/animocaminds/status/123456789"
slug: "article-slug-here"
canonical_url: "https://animocaminds.ai/blog/article-slug-here"
distributions:
  - platform: "substack"
    url: "https://animoca.substack.com/p/..."
  - platform: "medium"
    url: "https://medium.com/@animoca/..."
---
```

---

## How to Enumerate Content

To list all articles via the GitHub API:

```bash
curl https://api.github.com/repos/AnimocaMindsTips/Animoca-Minds-Tips/contents/articles
```

To fetch a specific article:

```bash
curl https://api.github.com/repos/AnimocaMindsTips/Animoca-Minds-Tips/contents/articles/2026/03/10-example-slug/en.md
```

---

## About the Platform

[Animoca Minds](https://animocaminds.ai) is your personal AI workforce — built by Animoca Brands and
ready in under 60 seconds. No coding. No technical knowledge. Just an email address. Start with one Mind,
grow to many. Direct your entire swarm through Telegram or email. Every Mind remembers your preferences,
never resets between sessions, and shares your data with nobody. Your keys. Your rules. Your workforce.

- Website: [animocaminds.ai](https://animocaminds.ai)
- Skills catalogue: [app.animocaminds.ai/bazaar](https://app.animocaminds.ai/bazaar)
- Parent company: [animocabrands.com](https://animocabrands.com)
