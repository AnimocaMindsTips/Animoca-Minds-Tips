# Contributing

## Add a skill to the Skills Directory

1. Test the skill on [Animoca Minds](https://animocaminds.ai) — it must work before you submit
2. Open a PR adding one entry to the relevant section in `skills/README.md`
3. Use this format exactly:
   ```
   **Skill Name** — One sentence describing what it does.
   ```
4. Include the Skill ID in your description so users can equip it via the platform
5. If no category fits, suggest a new one in your PR description

## Add a post to the content archive

1. Create a folder: `posts/YYYY/MM/DD-your-slug/`
2. Add `en.md` with YAML frontmatter — see [AGENTS.md](AGENTS.md) for the required fields
3. Set `content_type` in the frontmatter: `article`, `thread`, `tip`, or `ugc`
4. Translations are optional but welcome — use the language codes in AGENTS.md
5. The content index updates automatically via GitHub Actions

## Standards

- Skills must be personally tested and confirmed working on the platform
- Posts must be original content — no reposts of third-party material without attribution
- All links must resolve at time of submission
