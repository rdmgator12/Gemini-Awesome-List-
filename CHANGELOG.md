# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for new entries, PATCH for description/URL fixes.

## [Unreleased]

### Planned for v1.1.0
- Expand CLI Extensions coverage from ~130 curated → ~200 by pulling deeper from the [public registry](https://geminicli.com/extensions.json).
- Add per-extension star-count badges (mirroring how the registry ranks).
- Track Connected Apps surface renaming history in a dedicated mini-timeline.

---

## [1.0.2] — 2026-05-15

### Added
- **Databases and Data:** Bigtable (GoogleCloudPlatform/cloud-bigtable-ecosystem), BigQuery Remote MCP, Cloud DB Context Enrichment — all Google-owned, surfaced by re-diff against the live registry.
- **Observability and SRE:** Observability (GCP) — Google's cross-resource observability MCP at `gemini-cli-extensions/observability`.
- **Security:** GCP Hardening Agent (GoogleCloudPlatform/gcp-hardening-toolkit) — hardening blueprints and Terraform remediation.
- **Development and DevOps:** GitHub MCP Server (github/github-mcp-server, 30K stars) — GitHub's official MCP, and Web Quality Skills (addyosmani/web-quality-skills) — web-vitals and accessibility skill bundle.
- **AI and Agents:** claude-code-workflows (wshobson/agents, 35K stars) — cross-platform agent workflows reusable in Gemini CLI.
- **Web and Browser:** Apify Agent Skills (apify/agent-skills, 2K stars) — web-scraping Actor toolkit.

### Changed
- Header counts: CLI Extensions (curated) 120+ → 130+, version 1.0.1 → 1.0.2.
- Live registry total corrected from ~987 entries to ~783 entries (as of May 2026). The prior figure was sourced from an earlier registry snapshot; the registry has since pruned inactive entries.

### Notes
- Connected Apps surface: no net-new entries verified this week. Google Chat (added as a Workspace data source on March 25, 2026) is already covered by the Workspace umbrella entry. NotebookLM and Notebooks integration (April 8, 2026) is a Gemini-internal feature, not a separately toggleable Connected App.

---

## [1.0.1] — 2026-05-10

### Fixed
- Corrected 4 broken GitHub URLs caught by liveness check:
  - `gemini-cli-extensions/bigquery-conversational` → `bigquery-conversational-analytics` (correct repo name).
  - `gemini-cli-extensions/cloud-observability` → `gemini-cli-extensions/observability` (renamed).
  - `gemini-cli-extensions/cloud-assist` → `GoogleCloudPlatform/gemini-cloud-assist-mcp` (lives in the GoogleCloudPlatform org).
  - `googlemaps/platform-mcp` → `googlemaps/platform-ai` (correct repo name — Maps Platform Code Assist toolkit).

### Added
- ~50 additional official Google CLI extensions surfaced by completeness audit against the `gemini-cli-extensions` GitHub org (66 total repos in the org as of May 2026).
- New **Cloud and Infrastructure** entries: Cloud Run (CLI extension wrapper), GKE MCP Remote, Compute Engine, Cloud Storage, Cloud Resource Manager, Cloud Composer, Pub/Sub, Managed Kafka, Dataproc, Datastream, Database Migration Service.
- New **Databases and Data** entries: MCP Toolbox CLI variant, BigQuery Data Transfer Service, BigQuery Migration Service, generic PostgreSQL/MySQL/SQL Server, Spanner, AlloyDB Omni, Firestore (separate from Firestore Native), Memorystore for Redis, Memorystore for Valkey, Knowledge Catalog, Looker, Looker Conversational Analytics.
- New **Development and DevOps** entries: Angular, Web Accessibility, Android Management API, Firebase (Gemini CLI version), Workspace Dev Assist, Workspace Developer MCP, Vertex AI, Vertex AI Search, Customer Experience Agent Studio, Data Agent Kit Starter Pack, Developer Knowledge, Pay and Wallet Developer.
- Split **Observability and Security** into two sections: **Observability and SRE** (now includes Cloud Logging, Cloud Monitoring, SRE Extension, AlloyDB Observability, Cloud SQL *-Observability variants) and **Security** (added Google SecOps CLI extension separately from `google/mcp-security`).

### Changed
- TOC restructured to reflect Observability/Security split.
- Header counts: Connectors 70+ → 120+, Categories 14 → 15.

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

[Unreleased]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.2...HEAD
[1.0.2]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/rdmgator12/Gemini-Awesome-List-/releases/tag/v1.0.0
