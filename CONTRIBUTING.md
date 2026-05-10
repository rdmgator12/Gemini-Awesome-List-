# Contributing

This list curates Gemini's two extension surfaces: **Consumer Connected Apps** (closed Google-curated list) and **Gemini CLI Extensions** (open ~987-entry public registry). Contributions welcome.

> This is an independent, community-maintained project. Not affiliated with, endorsed by, or sponsored by Google LLC.

## What You Can Contribute

### Consumer Connected Apps additions
When Google adds a new Connected App (announced via [release notes](https://gemini.google/release-notes/) or [the Connected Apps help page](https://support.google.com/gemini/answer/13695044)), submit a PR adding it to the appropriate category with a description and use case. Note Android-only / OEM-specific scope where relevant via the 🤖 emoji legend.

### CLI Extension additions
Submit a PR for any CLI extension that is:
- **Officially maintained by Google** (any `google`, `gemini-cli-extensions`, `googlecloudplatform`, `googleworkspace`, `firebase`, or `googleapis` GitHub org), **OR**
- **High-signal third-party** with: a documented `gemini-extension.json` manifest, a real production use case, and either non-trivial GitHub stars or a reputable maintainer.

We don't mirror the full registry — see the [Gemini CLI Extensions registry](https://geminicli.com/extensions.json) for that. We curate.

### Improved Descriptions
If a description or use case is generic or vague, submit a PR with a more specific one. Use cases should describe what the extension actually unlocks, not what its homepage marketing says.

### Category Corrections
If an extension is in the wrong category, submit a PR moving it.

### Legend / Metadata Corrections
If a 🅖 / 🤝 / 🛠️ / 📡 / 🧠 / 🤖 emoji is wrong (e.g., a Google extension is mismarked as community), submit a PR fixing it.

### Field Reports
Tested an extension and have real-world notes? Add a brief field report below the entry:

```markdown
- 🅖 📡 [Extension Name](https://github.com/...) - Description. *Use case: ...*
  > **Field report:** One paragraph on what worked, what didn't, what surprised you. Be specific.
```

## Guidelines

- One PR per change unless closely related.
- Keep descriptions concise — one sentence for the description, one for the use case.
- Use cases should be specific and practical, not marketing copy.
- For CLI extensions, link to the **GitHub repository**, not a vendor marketing page (the registry is repo-keyed).
- For Connected Apps, link to the [Connected Apps help center](https://support.google.com/gemini/answer/13695044) or the vendor homepage.
- Maintain alphabetical order within categories.
- Apply the legend correctly:
  - 🅖 = built/maintained by Google (any of the orgs listed above)
  - 🤝 = official partner / OEM relationship (Spotify, OpenStax, Samsung, etc.)
  - 🛠️ = community / third-party
  - 📡 = ships an MCP server (per `gemini-extension.json`)
  - 🧠 = ships skills (portable to/from Anthropic skills via skill-porter)
  - 🤖 = Android-only (Connected Apps surface)

## Surface Notes

Gemini renamed the consumer surface three times: *Extensions* (2024) → *Apps* (early 2025) → *Connected Apps* (Oct 2025). When citing Google docs, prefer the current "Connected Apps" name even if the linked help article still says "Extensions" or "Apps." The CLI surface has consistently been called **Extensions**.

Public-info services (Maps, Flights, Hotels, YouTube, Search, Shopping, News) are auto-invoked from natural prompts as of Oct 2025 and don't appear as toggleable Connected Apps. They live in their own section at the bottom of the Consumer surface.

## Updates

This list is updated as Google publishes new Connected Apps and as the CLI registry adds high-signal extensions. If you notice changes that aren't reflected here, please open an issue or PR.
