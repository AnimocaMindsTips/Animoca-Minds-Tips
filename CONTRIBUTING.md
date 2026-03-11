# Contributing

## Add a skill to the Skills Directory

1. Test the skill on [Animoca Minds](https://animocaminds.ai) — it must work before you submit
2. Open a PR adding one entry to the relevant section in `skills/README.md`
3. Use this format exactly:
   ```
   **[Skill Name](https://app.animocaminds.ai/bazaar/apps/{uuid}/)** — One sentence describing what it does.
   ```
4. Link directly to the individual skill page — not the Bazaar catalogue root
5. If no category fits, suggest a new one in your PR description

## Add an article to the content archive

1. Create a folder: `articles/YYYY/MM/DD-your-slug/`
2. Add `en.md` with YAML frontmatter — see [AGENTS.md](AGENTS.md) for the required fields
3. Translations are optional but welcome — use the language codes in AGENTS.md
4. The article index updates automatically via GitHub Actions

## Standards

- Skills must be personally tested and confirmed working on the platform
- Articles must be original content — no reposts of third-party content
- All links must use full URLs (https://...), not relative paths
- Author field in frontmatter must be `"Animoca Minds"` for platform content

## Questions

Contact the Animoca Brands marketing team before opening a PR if you're unsure whether
a skill or article qualifies.
