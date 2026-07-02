# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for new entries, PATCH for description/URL fixes.

## [Unreleased]

### Planned for v1.3.0
- Expand CLI Extensions coverage from ~140 curated → ~200 by pulling deeper from the [public registry](https://geminicli.com/extensions.json).
- Add per-extension star-count badges (mirroring how the registry ranks).
- Track Connected Apps surface renaming history in a dedicated mini-timeline — note the help center now nests Connected Apps settings under **Personal Intelligence** (per the June 29, 2026 personalized-image-creation launch), the fourth naming era after Extensions → Apps → Connected Apps.
- **📡 re-tag audit (PATCH cycle):** the v1.1.0 cloud-storage fix was one instance of a broad pattern — manifest verification shows ~15 Google extensions no longer declare `mcpServers` and now ship `skills/` dirs (dataproc, cloud-sql-* ×3, spanner, alloydb, alloydb-omni, oracledb, firestore-native, knowledge-catalog, looker, bigquery-data-analytics, code-review, conductor, sre, googleworkspace/cli, and others), while `nanobanana` and `clasp` report MCP the README doesn't tag. Dedicated pass needed; conversions predate June 26.
- Snapshot `extensions.json` at each sweep (repo or scratch archive) so registry deltas can be attributed — the +2 this window could not be identified without a prior snapshot.
- Curation candidates spotted outside the window (not provably new): `krakenfx/kraken-cli` (vendor-official Kraken trading CLI, 652★), `hyhmrright/brooks-lint` (code review grounded in 12 engineering books, 1.2K★), `davidmosiah/google-health-mcp` (npm-published Google Health API v4, 18★).

---

## [1.2.0] — 2026-07-02

### Added
- **Consumer Connected Apps — new Lifestyle section:** [Google Play](https://support.google.com/gemini/answer/17131257) (🅖 🤖) — find/install apps and make in-app or gift-card purchases from chat; Android-only, 18+, rolled out June 26, 2026. Mirrors the help center's new "Lifestyle apps" grouping; Instacart/OpenTable/Zillow stay under MCP-Connected Partner Apps per this list's architecture-first taxonomy.
- **MCP-Connected Partner Apps:** Zillow Rentals (🤝 📡) — rental search + tour booking, the first real-estate Connected App; Dropbox (🤝 📡) — file access/sharing via Spark, still rolling out. Both per Google's [June 30 Spark update](https://blog.google/innovation-and-ai/products/gemini-app/gemini-spark-updates-june-2026/).

### Changed
- Header counts: Connected Apps 32 → 35, Categories 17 → 18 (new **Lifestyle**), version 1.1.0 → 1.2.0.
- MCP-Connected Partner Apps intro: Google now supports **custom MCP servers** for Spark users (June 30) — the surface is no longer purely partnership-driven; Instacart/OpenTable graduated from Spark-only to the main help-center list.
- Live registry total: ~1,056 → 1,058 across all three README mentions (+2 in 6 days — growth has flattened vs prior cycles).

### Notes
- Spark's June 30 update also shipped a macOS beta (US Ultra, 18+) and Google Tasks/Keep support — both covered by the existing Workspace umbrella entry, no new entries.
- gemini-cli: v0.49.0 (June 25) shipped a skill-install path-traversal security fix (PR #27767); in-window releases were nightlies only. No new repos in the `gemini-cli-extensions` org since April.
- Zillow's site hard-blocks programmatic access (curl 403, crawl timeout) — liveness established via Google's own help center listing and Zillow's live press room.
- Skipped: `epoko77-ai/im-not-ai` (3.5K★ Korean-locale text humanizer) per the existing locale precedent.
- The v1.2.0 milestone previously reserved in [Unreleased] has been renumbered to v1.3.0; this release consumes 1.2.0 for the weekly sweep per the documented SemVer rule (MINOR for new entries).

---

## [1.1.0] — 2026-06-26

### Added
- **Consumer Connected Apps — new Business section:** [Google Business Profile](https://blog.google/innovation-and-ai/products/gemini-app/gemini-features-for-businesses/) (🅖) — connect a Business Profile so Gemini understands brand and customer data; analyze search/engagement performance, draft brand-voice review responses, update hours/posts. Announced June 10, 2026 ("Google for Brazil"); rolling out globally. The companion *Business notebooks* feature is a NotebookLM-style surface, not a separately toggleable Connected App — skipped per the NotebookLM precedent.
- **Consumer Connected Apps — Education:** [Google Classroom](https://classroom.google.com) (🅖) — `@Classroom` mention pattern; educators draft differentiated assignments and summarize submissions, students 18+ build study plans. Workspace for Education/Business accounts, English at launch; rollout completed ~June 18, 2026.
- **CLI Extensions — Security:** Chrome Enterprise Premium MCP (`google/chrome-enterprise-premium-mcp`, 🅖 📡) — official reference MCP for browser-security management (updated June 25, 2026). cnspec Agent Skills (`mondoohq/cnspec`, 🛠️ 🧠) — cloud-native security scanner exposed as MQL/policy skills.
- **CLI Extensions — Web and Browser:** Modern Web Guidance (`GoogleChrome/modern-web-guidance`, 🅖 🧠, 1.4K stars) — Chrome-team skill keeping coding agents current on web best practices.
- **CLI Extensions — AI and Agents:** gemini-kit (`nth5693/gemini-kit`, 🛠️ 📡 🧠) — 19 agents + 44 commands purpose-built for Gemini CLI. Maestro Orchestrate (`josstei/maestro-orchestrate`, 🛠️ 📡 🧠) — 39-specialist multi-agent orchestration with parallel subagents. Aware (`qodo-ai/open-aware`, 🛠️ 📡) — Qodo's deep code-research agent.

### Fixed
- **Cloud Storage** extension: repo renamed `gemini-cli-extensions/cloud-storage` → `gemini-cli-extensions/google-cloud-storage` (old URL still 301-redirects). It no longer ships an MCP server — re-tagged 📡 → 🧠 (skills bundle), per the live registry as of June 20, 2026.
- Registry total reconciled across the README: prose said ~891, body said ~783 — both corrected to ~1,056 (live `extensions.json` count, June 2026).

### Changed
- Header counts: Connected Apps 30 → 32, CLI Extensions (curated) 134+ → 140+, Categories 16 → 17 (new **Business** section), version 1.0.3 → 1.1.0.
- New top-level Consumer section: **Business**.
- Live registry total: ~891 (May) → ~1,056 (June) — +165 in ~5 weeks; growth is dominated by portable cross-agent *skills* entries.

### Notes
- Verified against Google's June 10 business-features blog post, the Workspace Classroom-in-Gemini rollout notes, the Connected Apps help center, and the live `geminicli.com/extensions.json` (1,056 entries).
- Skipped this cycle: the high-star registry churn was mostly portable cross-agent skill libraries (`DietrichGebert/ponytail`, `open-gsd/gsd-core`, `max-sixty/worktrunk`) and CN/locale forks (`jnMetaCode/superpowers-zh`, `wbh604/UZI-Skill`, `Jesseovo/last30days-skill-cn`) — not Gemini-specific enough for curation, consistent with prior cycles. *Business notebooks* (feature, not Connected App) also skipped.

---

## [1.0.3] — 2026-05-22

### Added
- **Consumer Connected Apps — Communication:** [Contacts](https://contacts.google.com) (🅖) — Google Contacts management via natural language. Per the [help center](https://support.google.com/gemini/answer/17100956), currently English-only and Gemini Spark-only at launch; works on web + mobile.
- **Consumer Connected Apps — new MCP-Connected Partner Apps section:** Canva, Instacart, OpenTable — per Google's [May 19, 2026 announcement](https://blog.google/innovation-and-ai/products/gemini-app/next-evolution-gemini-app/), partner-hosted MCP servers can now connect to the Consumer surface. Architecturally distinct from the prior closed/invitation-only Connected Apps pattern. Rolling out via Gemini Spark to U.S. Google AI Ultra subscribers; more partners "integrating now" per the blog.
- **CLI Extensions — AI and Agents:** Google Agents CLI (`google/agents-cli`, 2.5K stars) — official scaffolding/deploy CLI for Google ADK agents. last30days-skill (`mvanhorn/last30days-skill`, 26K stars) — multi-platform topic research across Reddit, X, YouTube, TikTok, Instagram, HN, Polymarket, and the web.
- **CLI Extensions — Development and DevOps:** SocratiCode (`giancarloerra/SocratiCode`, 2.7K stars) — codebase intelligence with hybrid semantic search and polyglot dependency graphs. Go Agent Skills (`samber/cc-skills-golang`, 1.8K stars) — production-ready Go agent skills.

### Changed
- Header counts: Connected Apps 26 → 30, CLI Extensions (curated) 130+ → 134+, Categories 15 → 16, version 1.0.2 → 1.0.3.
- Live registry total updated from ~783 → ~891 entries (+108 in 7 days — registry is in active growth, not pruning, this week).
- New top-level section under Consumer Connected Apps: **MCP-Connected Partner Apps**, capturing the new MCP-via-Spark partnership pattern.

### Notes
- Connected Apps count now 30: +1 Contacts + 3 Spark MCP partners (Canva, Instacart, OpenTable). All four new entries verified against the Connected Apps help center and the May 19, 2026 Gemini blog post.
- Per the blog, "a full list of more partners are integrating now" — anticipate further additions as Spark expands beyond U.S. Ultra beta.
- Skipped this cycle: `jnMetaCode/superpowers-zh` (Chinese localization of `obra/superpowers` — parent is already listed, localization adds little for the English-reading audience), `wbh604/UZI-Skill` (CN-only stock-analysis skill, too niche for general coverage).

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

[Unreleased]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.1.0...HEAD
[1.1.0]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.3...v1.1.0
[1.0.3]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.2...v1.0.3
[1.0.2]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/rdmgator12/Gemini-Awesome-List-/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/rdmgator12/Gemini-Awesome-List-/releases/tag/v1.0.0
