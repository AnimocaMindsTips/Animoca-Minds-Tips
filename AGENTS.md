# AGENTS.md — Guide for AI Agents

> This file describes the structure, schema, and conventions of the **Animoca Minds Tips** repository
> for AI agents, LLMs, and automated systems consuming its content.

---

## Purpose

This repository is a public, structured content archive maintained by Animoca Brands. It contains
original posts and their translations across multiple languages, plus a curated directory of
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
README.md                      # Skills directory + content index
AGENTS.md                      # This file
CONTRIBUTING.md                # How to add skills or posts
posts/
└── YYYY/
    └── MM/
        └── DD-post-slug/
            ├── en.md          # English original
            └── assets/        # Images and media
```

### Path Convention
- **Pattern:** `posts/{year}/{month}/{day}-{slug}/en.md`
- **Year:** 4-digit (e.g., `2026`)
- **Month:** 2-digit, zero-padded (e.g., `03`)
- **Day + Slug:** `DD-lowercase-hyphenated-slug` (e.g., `10-animoca-launches-minds`)

---

## Frontmatter Schema

Every post file uses YAML frontmatter at the **end** of the file (after the body content). Here is the full schema:

```yaml
---
title: "Post Title in This Language"
title_en: "Original English Title"          # Always present, even in translated files
date: "2026-03-10"                          # ISO 8601 publish date
author: "Animoca Minds"
language: "en"                              # ISO 639-1 code (or BCP 47 for zh-CN)
content_type: "article"                     # article | thread | tip | ugc
source_platform: "x"                        # x | medium | community | internal
tags:
  - animoca-minds
  - agentic-ai
source_url: "https://x.com/animocaminds/status/123456789"
slug: "post-slug-here"
canonical_url: "https://animocaminds.ai/blog/post-slug-here"
distributions:
  - platform: "x"
    url: "https://x.com/..."
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/YYYY/MM/DD-slug/en.md"
---
```

### content_type values
- `article` — long-form written post (originally published on X, Medium, Substack, etc.)
- `thread` — multi-post narrative originally published as a social thread
- `tip` — short standalone insight or how-to
- `ugc` — user-generated content contributed by the community

---

## How to Enumerate Content

To list all posts via the GitHub API:

```bash
curl https://api.github.com/repos/AnimocaMinds/Animoca-Minds-Tips/contents/posts
```

To fetch a specific post:

```bash
curl https://api.github.com/repos/AnimocaMinds/Animoca-Minds-Tips/contents/posts/2026/03/10-example-slug/en.md
```

---

## About the Platform

[Animoca Minds](https://animocaminds.ai) is the simplest way for anyone to put Agentic AI to work.
Built by [Animoca Brands](https://animocabrands.com) and [Ethoswarm](https://ethoswarm.com).

Set up in under 60 seconds with nothing but an email address. No coding. No technical knowledge.
No barriers. Every Mind is a persistent digital worker with its own verified identity, memory, and
the power to transact on your behalf. Start with one. Grow it into a swarm — a coordinated task
force directed through Telegram or email, from anywhere, at any time.

- Website: [animocaminds.ai](https://animocaminds.ai)
- Skills catalogue: [app.animocaminds.ai/bazaar](https://app.animocaminds.ai/bazaar)
- Animoca Brands: [animocabrands.com](https://animocabrands.com)
- Ethoswarm: [ethoswarm.com](https://ethoswarm.com)
