# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for new entries, PATCH for description/URL fixes.

## [Unreleased]

### Planned for v1.1.0
- Expand CLI Extensions coverage from ~70 curated → ~150 by pulling deeper from the [public registry](https://geminicli.com/extensions.json).
- Add per-extension star-count badges (mirroring how the registry ranks).
- Track Connected Apps surface renaming history in a dedicated mini-timeline.
- Add `awesome-lint` to CI once the repo is ≥30 days old (lint blocks submissions on `git-repo-age` until 2026-06-09).

---

## [1.0.0] — 2026-05-10

### Added
- Initial seed covering Gemini's two extension surfaces:
  - **Consumer Connected Apps:** 26 entries across Productivity, Communication, Media, Smart Home, Education, Developer Tools, OEM Partner Apps + 7 auto-invoked public-info services.
  - **Gemini CLI Extensions:** ~70 curated entries across Cloud, Databases, Dev/DevOps, Observability, Productivity, AI/Agents, Web/Browser. The full registry (~987 entries) lives at [geminicli.com/extensions.json](https://geminicli.com/extensions.json) — we curate the highest-signal subset.
- README.md with About, Legend (🅖 🤝 🛠️ 📡 🧠 🤖), Contents, and curated sections.
- CONTRIBUTING.md with surface-specific submission guidance and Connected Apps naming history.
- CHANGELOG.md (this file).
- LICENSE (CC0-1.0) — awesome-list canonical convention.
- code-of-conduct.md (Contributor Covenant 2.1).
- .editorconfig + .gitignore.
- Badges row: Awesome, License (CC0-1.0), Last Commit, Track Awesome List.

### Notes
- Connected Apps list assembled from Google's official [help center](https://support.google.com/gemini/answer/13695044) and release notes through May 2026.
- CLI Extensions list assembled from the public registry (~987 entries), filtered to: all Google-owned extensions across `google`, `gemini-cli-extensions`, `googlecloudplatform`, `googleworkspace`, `firebase`, `googleapis` orgs + the highest-signal third-party entries by topic.

[Unreleased]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/rdmgator12/Gemini-Awesome-List-/releases/tag/v1.0.0
