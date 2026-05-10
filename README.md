# Awesome Gemini Extensions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![Last Commit](https://img.shields.io/github/last-commit/rdmgator12/Gemini-Awesome-List-)](https://github.com/rdmgator12/Gemini-Awesome-List-/commits/main)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com/rdmgator12/Gemini-Awesome-List-/)

> A curated directory of every extension and connected app available across Gemini's two integration surfaces — the consumer Gemini app (`gemini.google.com`) and the developer-side **Gemini CLI** — organized by category with descriptions and use cases.

**Last updated:** May 10, 2026 · **Connected Apps:** 26 · **CLI Extensions (curated):** 120+ · **Categories:** 15 · **Version:** [1.0.1](CHANGELOG.md)

---

## About

Gemini has two distinct extension surfaces, and they don't share an SDK:

1. **Consumer Connected Apps** — Google-curated integrations available in the Gemini chat at [gemini.google.com](https://gemini.google.com/apps). Originally called *Extensions* (2024), then *Apps* (early 2025), now **Connected Apps** (Oct 2025). Closed list — no third-party developer SDK; entries are partnership/invitation-driven. As of Oct 2025, public-info services like Maps, Flights, Hotels, YouTube, and Search are auto-invoked from natural prompts and no longer require the `@AppName` mention pattern.
2. **Gemini CLI Extensions** — open developer ecosystem for [Gemini CLI](https://github.com/google-gemini/gemini-cli), Google's terminal CLI for Gemini. Each extension is a directory with a `gemini-extension.json` manifest that can ship MCP servers, context files, hooks, skills, and custom slash commands. The authoritative public registry lives at **[geminicli.com/extensions.json](https://geminicli.com/extensions.json)** with ~987 entries ranked by GitHub stars (May 2026).

This list curates both surfaces. The Consumer side is enumerated exhaustively. The CLI side is too large to mirror entry-for-entry — we curate **all official Google extensions** plus the highest-signal third-party ones; the registry remains the canonical full source.

For more information, see the [Gemini CLI extensions reference](https://github.com/google-gemini/gemini-cli/blob/main/docs/extensions/reference.md), the [Gemini CLI extensions codelab](https://codelabs.developers.google.com/getting-started-gemini-cli-extensions), and the [Connected Apps help center](https://support.google.com/gemini/answer/13695044).

> This is an independent, community-maintained list. Not affiliated with, endorsed by, or sponsored by Google LLC. "Gemini," "Google," and related marks are the property of Google LLC. Each extension is the property of its respective owner.

---

## Legend

- 🅖 — Built or maintained by Google
- 🤝 — Official partner / OEM
- 🛠️ — Community-built (third-party)
- 📡 — Ships an MCP server
- 🧠 — Ships skills (portable to/from Anthropic skills via [skill-porter](https://github.com/jduncan-rva/skill-porter))
- 🤖 — Android-only (Connected Apps surface)

---

## Contents

### Consumer Connected Apps
- [Productivity (Workspace)](#productivity-workspace)
- [Communication](#communication)
- [Media and Entertainment](#media-and-entertainment)
- [Smart Home and Device Control](#smart-home-and-device-control)
- [Education](#education)
- [Developer Tools (Consumer)](#developer-tools-consumer)
- [OEM Partner Apps](#oem-partner-apps)
- [Auto-invoked Public-info Services](#auto-invoked-public-info-services)

### Gemini CLI Extensions
- [Cloud and Infrastructure](#cloud-and-infrastructure)
- [Databases and Data](#databases-and-data)
- [Development and DevOps](#development-and-devops)
- [Observability and SRE](#observability-and-sre)
- [Security](#security)
- [Productivity and Communication (CLI)](#productivity-and-communication-cli)
- [AI and Agents](#ai-and-agents)
- [Web and Browser](#web-and-browser)

### Project Files
- [Contributing](#contributing)
- [Related](#related)
- [License](#license)

---

# Consumer Connected Apps

Toggleable integrations in the Gemini chat at [gemini.google.com/apps](https://gemini.google.com/apps). Closed list — no public SDK.

## Productivity (Workspace)

- 🅖 [Google Workspace](https://support.google.com/gemini/answer/15229592) - Umbrella connector covering Gmail, Calendar, Drive, Docs, Sheets, Slides, Keep, Tasks, Chat, and Meet. *Use case: Drafting emails grounded in thread history, summarizing Drive folders, generating slide decks from Docs content, scheduling around existing Calendar commitments.*

## Communication

- 🅖 🤖 [Messages](https://support.google.com/gemini/answer/13695044) - Default Android SMS client. *Use case: Sending and summarizing text messages from natural-language prompts on Android.*
- 🅖 🤖 [Phone](https://support.google.com/gemini/answer/13695044) - Default Android dialer. *Use case: Initiating and managing calls without leaving the assistant.*
- 🤝 🤖 [WhatsApp](https://support.google.com/gemini/answer/13695044) - Send and read WhatsApp messages on Android. *Use case: Conversational message drafting and inbox triage in WhatsApp from Gemini.*

## Media and Entertainment

- 🅖 [Google Photos](https://support.google.com/gemini/answer/13695044) - Search and surface photos by content, date, location. *Use case: Pulling memories by description ("photos from Sarah's birthday last fall"), generating captions, finding receipts buried in screenshots.*
- 🅖 [YouTube Music](https://support.google.com/gemini/answer/13695044) - Play, queue, and recommend tracks. *Use case: Soundtrack for a focus block, exploring an artist's catalog, building playlists from a vibe description.*
- 🤝 [Spotify](https://support.google.com/gemini/answer/13695044) - Play, queue, and recommend tracks. *Use case: Same as YouTube Music for Spotify subscribers — playlist building, recommendations, playback control.*

## Smart Home and Device Control

- 🅖 [Google Home](https://support.google.com/gemini/answer/13695044) - Control smart-home devices, routines, and scenes. *Use case: Adjusting lights/thermostat/locks via natural language, querying device state, kicking off routines.*
- 🅖 🤖 [Utilities](https://support.google.com/gemini/answer/13695044) - Android system controls (timers, alarms, settings). *Use case: Setting timers and alarms, toggling Wi-Fi/Bluetooth/Do Not Disturb from chat.*

## Education

- 🤝 [OpenStax](https://openstax.org) - Free, peer-reviewed open educational resources from Rice University. *Use case: Pulling textbook content for tutoring sessions, citing OpenStax material in study workflows.*

## Developer Tools (Consumer)

- 🤝 [GitHub](https://github.com) - Search and act on repositories from the Gemini chat. *Use case: Repository search, summarizing PR threads, generating commit messages from diffs without leaving Gemini.*

## OEM Partner Apps

Pre-loaded on partner devices; surface depends on OEM and Android build.

- 🤝 🤖 [Samsung Calendar](https://www.samsung.com) - Native Samsung calendar (Galaxy devices). *Use case: Native scheduling on Samsung phones.*
- 🤝 🤖 [Samsung Notes](https://www.samsung.com) - Native Samsung notes app. *Use case: Drafting and searching Samsung Notes from chat.*
- 🤝 🤖 [Samsung Reminder](https://www.samsung.com) - Samsung reminder app. *Use case: Setting reminders on Galaxy devices via natural language.*
- 🤝 🤖 [Samsung Gallery](https://www.samsung.com) - Native photo gallery. *Use case: Searching and managing photos in Samsung Gallery.*
- 🤝 🤖 [OPPO Calendar](https://www.oppo.com) - Native OPPO calendar. *Use case: Scheduling on OPPO devices.*
- 🤝 🤖 [OPPO Notes](https://www.oppo.com) - Native OPPO notes. *Use case: Notes capture and retrieval on OPPO.*
- 🤝 🤖 [OnePlus Notes](https://www.oneplus.com) - Native OnePlus notes. *Use case: Notes on OnePlus devices.*
- 🤝 🤖 [OnePlus Mind Space](https://www.oneplus.com) - OnePlus's structured-thought capture surface. *Use case: Idea capture and organization on OnePlus.*
- 🤝 🤖 [HONOR Calendar](https://www.hihonor.com) - Native HONOR calendar. *Use case: Scheduling on HONOR devices.*
- 🤝 🤖 [HONOR Notes](https://www.hihonor.com) - Native HONOR notes. *Use case: Notes capture on HONOR.*
- 🤝 🤖 [Xiaomi Calendar](https://www.mi.com) - Native Xiaomi calendar. *Use case: Scheduling on Xiaomi/Redmi devices.*
- 🤝 🤖 [Xiaomi Notes](https://www.mi.com) - Native Xiaomi notes. *Use case: Notes capture on Xiaomi/Redmi.*
- 🤝 🤖 [vivo Notes](https://www.vivo.com) - Native vivo notes. *Use case: Notes capture on vivo devices.*
- 🤝 🤖 [TECNO Calendar](https://www.tecno-mobile.com) - Native TECNO calendar. *Use case: Scheduling on TECNO devices.*
- 🤝 🤖 [TECNO Notepad](https://www.tecno-mobile.com) - Native TECNO notepad. *Use case: Notes capture on TECNO.*

## Auto-invoked Public-info Services

These don't require toggling and don't appear in the Connected Apps list — they're invoked automatically from natural prompts as of Oct 2025.

- 🅖 [Google Search (incl. AI Mode)](https://www.google.com) - Web search and AI Overviews. *Use case: Grounded answers from the live web; cited synthesis.*
- 🅖 [Google Maps](https://www.google.com/maps) - Places, directions, transit, and local info. *Use case: Routing, business lookup, location-based recommendations.*
- 🅖 [Google Flights](https://www.google.com/travel/flights) - Flight search and price tracking. *Use case: Itinerary research, fare alerts, multi-city planning.*
- 🅖 [Google Hotels](https://www.google.com/travel/hotels) - Hotel search and reviews. *Use case: Stay research grounded in availability and price.*
- 🅖 [YouTube](https://www.youtube.com) - Video search, summaries, and clip retrieval. *Use case: Pulling tutorial content, summarizing long videos, finding moments inside videos.*
- 🅖 [Google Shopping](https://shopping.google.com) - Product search and price comparison. *Use case: Product research grounded in current pricing and availability.*
- 🅖 [Google News](https://news.google.com) - News search across publishers. *Use case: Current-events synthesis with source attribution.*

---

# Gemini CLI Extensions

Open developer ecosystem. Browse the full ~987-entry public registry at **[geminicli.com/extensions](https://geminicli.com/extensions/)** or the parseable feed at **[geminicli.com/extensions.json](https://geminicli.com/extensions.json)**. Below is a curated subset.

## Cloud and Infrastructure

- 🅖 📡 [gcloud](https://github.com/gemini-cli-extensions/gcloud) - Google Cloud CLI surface. *Use case: Querying GCP project state, managing resources, scripted deploys via natural language.*
- 🅖 📡 [Cloud Run](https://github.com/GoogleCloudPlatform/cloud-run-mcp) - Serverless container deploys on Cloud Run. *Use case: Deploying services, querying revisions, debugging traffic splits.*
- 🅖 📡 [Cloud Run (Gemini CLI extension)](https://github.com/gemini-cli-extensions/cloud-run) - Cloud Run extension wrapper. *Use case: Same Cloud Run scope, packaged as a Gemini CLI extension.*
- 🅖 📡 [GKE MCP](https://github.com/GoogleCloudPlatform/gke-mcp) - Google Kubernetes Engine management. *Use case: Cluster operations, pod debugging, deployment automation on GKE.*
- 🅖 📡 [GKE MCP Remote](https://github.com/gemini-cli-extensions/gke-mcp-remote) - Remote-mode GKE MCP variant. *Use case: GKE ops without local kubeconfig — works against a remote MCP endpoint.*
- 🅖 📡 [Compute Engine](https://github.com/gemini-cli-extensions/compute-engine) - GCE virtual machines. *Use case: VM lifecycle (start/stop/resize), instance group ops, image and disk management.*
- 🅖 📡 [Cloud Storage](https://github.com/gemini-cli-extensions/cloud-storage) - GCS object storage. *Use case: Bucket ops, object inspection, ACL/IAM checks.*
- 🅖 📡 [Cloud Resource Manager](https://github.com/gemini-cli-extensions/cloud-resource-manager) - Project, folder, and org hierarchy management. *Use case: Cross-project queries, IAM hierarchy inspection, project lifecycle ops.*
- 🅖 📡 [Cloud Composer](https://github.com/gemini-cli-extensions/cloud-composer) - Managed Apache Airflow on GCP. *Use case: DAG inspection, task triage, environment management.*
- 🅖 📡 [Pub/Sub](https://github.com/gemini-cli-extensions/pubsub) - Google Cloud Pub/Sub messaging. *Use case: Topic/subscription admin, message replay, dead-letter inspection.*
- 🅖 📡 [Managed Kafka](https://github.com/gemini-cli-extensions/managed-kafka) - Google's managed Kafka service. *Use case: Cluster admin, topic ops, consumer-group debugging.*
- 🅖 📡 [Dataproc](https://github.com/gemini-cli-extensions/dataproc) - Managed Spark/Hadoop on GCP. *Use case: Cluster lifecycle, job submission, batch analytics.*
- 🅖 📡 [Datastream](https://github.com/gemini-cli-extensions/datastream) - Managed CDC and replication. *Use case: Stream config, replication monitoring, source/destination admin.*
- 🅖 📡 [Database Migration Service](https://github.com/gemini-cli-extensions/database-migration-service) - GCP Database Migration Service. *Use case: Migration job authoring, status checks, cutover planning.*
- 🅖 📡 [Gemini Cloud Assist](https://github.com/GoogleCloudPlatform/gemini-cloud-assist-mcp) - Investigation-driven GCP operations assistant. *Use case: Create investigations, add observations, run analysis on GCP resources via natural language.*
- 🛠️ 📡 [Azure Skills](https://github.com/microsoft/azure-skills) - Microsoft Azure operations. *Use case: Azure resource management from the CLI.*
- 🛠️ 📡 [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-MCP) - Tencent CloudBase. *Use case: Tencent Cloud development workflows.*
- 🛠️ 📡 [Alibaba Cloud ACK MCP](https://github.com/aliyun/alibabacloud-ack-mcp-server) - Alibaba Container Service for Kubernetes. *Use case: Alibaba Cloud k8s operations.*
- 🛠️ 📡 [Terraform MCP](https://github.com/hashicorp/terraform-mcp-server) - HashiCorp Terraform. *Use case: IaC plan/apply workflows, state inspection, module lookup.*
- 🛠️ 📡 [Kubernetes MCP](https://github.com/Flux159/mcp-server-kubernetes) - Generic kubectl wrapper. *Use case: Cluster ops outside GKE-specific tooling.*

## Databases and Data

- 🅖 📡 [MCP Toolbox for Databases](https://github.com/googleapis/mcp-toolbox) - Unified DB connector covering 30+ data sources. *Use case: Querying heterogeneous databases through one toolbox.*
- 🅖 📡 [MCP Toolbox (CLI extension)](https://github.com/gemini-cli-extensions/mcp-toolbox) - DB tooling abstraction layer for Gemini CLI. *Use case: Multi-DB MCP convenience wrapper.*
- 🅖 📡 [BigQuery Data Analytics](https://github.com/gemini-cli-extensions/bigquery-data-analytics) - SQL analytics on BigQuery. *Use case: Ad-hoc analytics, query authoring grounded in schema.*
- 🅖 📡 [BigQuery Conversational Analytics](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics) - Natural-language → SQL on BigQuery. *Use case: Non-SQL users querying BigQuery; rapid analyst loops.*
- 🅖 📡 [BigQuery Data Transfer Service](https://github.com/gemini-cli-extensions/bigquery-data-transfer-service) - Scheduled data transfers into BigQuery. *Use case: Configure recurring loads from SaaS sources, monitor transfer runs.*
- 🅖 📡 [BigQuery Migration Service](https://github.com/gemini-cli-extensions/bigquery-migration-service) - Translate and migrate workloads to BigQuery. *Use case: SQL translation from Teradata/Redshift/Snowflake/etc., migration planning.*
- 🅖 📡 [Cloud SQL — PostgreSQL](https://github.com/gemini-cli-extensions/cloud-sql-postgresql) - Postgres on Cloud SQL. *Use case: Schema introspection and queries against managed Postgres.*
- 🅖 📡 [Cloud SQL — MySQL](https://github.com/gemini-cli-extensions/cloud-sql-mysql) - MySQL on Cloud SQL. *Use case: MySQL admin and queries.*
- 🅖 📡 [Cloud SQL — SQL Server](https://github.com/gemini-cli-extensions/cloud-sql-sqlserver) - SQL Server on Cloud SQL. *Use case: SQL Server admin and queries.*
- 🅖 📡 [PostgreSQL (generic)](https://github.com/gemini-cli-extensions/postgres) - Generic Postgres connector. *Use case: Any Postgres instance (GCP or otherwise) — schema, queries, role inspection.*
- 🅖 📡 [MySQL (generic)](https://github.com/gemini-cli-extensions/mysql) - Generic MySQL connector. *Use case: Any MySQL instance — schema, queries, user admin.*
- 🅖 📡 [SQL Server (generic)](https://github.com/gemini-cli-extensions/sql-server) - Generic SQL Server connector. *Use case: Any SQL Server instance — schema, queries, T-SQL workflows.*
- 🅖 📡 [Oracle DB](https://github.com/gemini-cli-extensions/oracledb) - Oracle Database connector. *Use case: Oracle DB queries and metadata exploration.*
- 🅖 📡 [Spanner](https://github.com/gemini-cli-extensions/spanner) - Cloud Spanner globally distributed DB. *Use case: Strongly consistent multi-region queries, schema management.*
- 🅖 📡 [AlloyDB](https://github.com/gemini-cli-extensions/alloydb) - AlloyDB for Postgres (Google's HTAP managed DB). *Use case: Postgres-compatible HTAP workloads on GCP.*
- 🅖 📡 [AlloyDB Omni](https://github.com/gemini-cli-extensions/alloydb-omni) - Self-managed AlloyDB Omni. *Use case: AlloyDB workflows on the self-hosted variant.*
- 🅖 📡 [Firestore Native](https://github.com/gemini-cli-extensions/firestore-native) - Cloud Firestore in native mode. *Use case: NoSQL document operations on Firestore.*
- 🅖 📡 [Firestore](https://github.com/gemini-cli-extensions/firestore) - Cloud Firestore (Datastore-mode + native). *Use case: Document store operations across both Firestore modes.*
- 🅖 📡 [Memorystore for Redis](https://github.com/gemini-cli-extensions/memorystore-for-redis) - Managed Redis on GCP. *Use case: Cache and session-store admin on Memorystore.*
- 🅖 📡 [Memorystore for Valkey](https://github.com/gemini-cli-extensions/memorystore-for-valkey) - Managed Valkey on GCP. *Use case: Open-source Redis-fork managed service ops.*
- 🅖 📡 [Knowledge Catalog](https://github.com/gemini-cli-extensions/knowledge-catalog) - Data discovery and governance via Knowledge Catalog. *Use case: Data asset search, lineage inspection, governance workflows.*
- 🅖 📡 [Data Commons](https://github.com/gemini-cli-extensions/datacommons) - Public statistical datasets via Data Commons. *Use case: Demographic, economic, and environmental research from a unified knowledge graph.*
- 🅖 📡 [Looker](https://github.com/gemini-cli-extensions/looker) - Looker BI integration. *Use case: Querying Looker explores, accessing dashboards, building data workflows.*
- 🅖 📡 [Looker Conversational Analytics](https://github.com/gemini-cli-extensions/looker-conversational-analytics) - Natural-language analytics on Looker. *Use case: Self-service BI without writing LookML — ask in English, get visualizations.*
- 🛠️ 📡 [Redis MCP](https://github.com/redis/mcp-redis) - Redis (caching/state). *Use case: Inspecting keys, debugging eviction, cache analytics.*
- 🛠️ 📡 [MongoDB Agent Skills](https://github.com/mongodb/agent-skills) - MongoDB operations. *Use case: Document queries, schema design, aggregation pipelines.*
- 🛠️ 📡 [Neo4j MCP](https://github.com/neo4j-contrib/mcp-neo4j) - Neo4j graph database. *Use case: Cypher query authoring, graph traversal exploration.*
- 🛠️ 📡 [Pinecone MCP](https://github.com/pinecone-io/pinecone-mcp) - Pinecone vector database. *Use case: Vector index inspection, query tuning, RAG debugging.*
- 🛠️ 📡 [Milvus MCP](https://github.com/zilliztech/mcp-server-milvus) - Milvus vector database. *Use case: Open-source vector DB ops.*
- 🛠️ 📡 [Confluent MCP](https://github.com/confluentinc/mcp-confluent) - Apache Kafka via Confluent Cloud. *Use case: Topic admin, consumer-group debugging, stream introspection.*
- 🛠️ 📡 [Elasticsearch (Gemini CLI)](https://github.com/elastic/gemini-cli-elasticsearch) - Elasticsearch search and analytics. *Use case: Log query, search relevance tuning, observability dashboards.*

## Development and DevOps

- 🅖 [clasp (Apps Script)](https://github.com/google/clasp) - Google Apps Script dev tooling. *Use case: Apps Script project scaffolding and deploys.*
- 🅖 📡 [Code Review](https://github.com/gemini-cli-extensions/code-review) - AI-assisted code review extension. *Use case: Pre-PR review pass, regression flag, style enforcement.*
- 🅖 📡 [CI/CD](https://github.com/gemini-cli-extensions/cicd) - CI/CD workflow tooling. *Use case: Pipeline authoring and debugging.*
- 🅖 📡 [Conductor](https://github.com/gemini-cli-extensions/conductor) - Spec → plan → implement workflow. *Use case: Structured implementation flow from a spec doc.*
- 🅖 📡 [Flutter](https://github.com/gemini-cli-extensions/flutter) - Flutter mobile dev. *Use case: Flutter project scaffolding, widget building, debug.*
- 🅖 📡 [Angular](https://github.com/gemini-cli-extensions/angular) - Angular framework dev. *Use case: Angular project scaffolding, component generation, build/test workflows.*
- 🅖 📡 [Web Accessibility](https://github.com/gemini-cli-extensions/web-accessibility) - Automate finding and fixing web accessibility issues. *Use case: WCAG compliance scanning, ARIA fixes, accessibility-first review.*
- 🅖 📡 [Android Management API](https://github.com/gemini-cli-extensions/android-management-api) - Android device fleet management. *Use case: Enterprise Android admin, policy authoring, device enrollment.*
- 🅖 📡 [Firebase (Gemini CLI)](https://github.com/gemini-cli-extensions/firebase) - Firebase backend services CLI extension. *Use case: Firebase project ops in the CLI ecosystem.*
- 🅖 📡 [Firebase Agent Skills](https://github.com/firebase/agent-skills) - Firebase agent skills bundle. *Use case: Auth, Firestore, Functions, Hosting workflows via skills.*
- 🅖 📡 [Genkit](https://github.com/gemini-cli-extensions/genkit) - Google's GenAI app dev framework. *Use case: Building production GenAI apps with structured chains.*
- 🅖 📡 [Google Workspace CLI](https://github.com/googleworkspace/cli) - Workspace developer tooling. *Use case: Add-on development, Apps Script and CardKit workflows.*
- 🅖 📡 [Google Workspace Developer Tools](https://github.com/googleworkspace/developer-tools) - Broader Workspace dev surface. *Use case: Workspace add-on QA and deploy.*
- 🅖 📡 [Workspace Dev Assist](https://github.com/googleworkspace/dev-assist) - Workspace developer MCP server. *Use case: Inline help while building Workspace add-ons and apps.*
- 🅖 📡 [Workspace Developer MCP](https://github.com/googleworkspace/developer-mcp) - MCP server for Workspace developers. *Use case: Workspace API documentation, code samples, API key management.*
- 🅖 📡 [Stitch](https://github.com/gemini-cli-extensions/stitch) - UI generation extension. *Use case: Generating UI components from prompts.*
- 🅖 📡 [Vertex AI](https://github.com/gemini-cli-extensions/vertex) - Manage prompts and resources in Vertex AI. *Use case: Prompt management, model deployment, MLOps on Vertex.*
- 🅖 📡 [Vertex AI Search](https://github.com/gemini-cli-extensions/vertex-ai-search) - Vertex AI Search retrieval. *Use case: RAG pipelines grounded in Vertex AI Search indexes.*
- 🅖 📡 [Customer Experience Agent Studio](https://github.com/gemini-cli-extensions/customer-experience-agent-studio) - Build CCAI / customer-experience agents. *Use case: Conversational agent authoring for customer support flows.*
- 🅖 📡 [Data Agent Kit Starter Pack](https://github.com/gemini-cli-extensions/data-agent-kit-starter-pack) - Starter pack for data agents. *Use case: Reference scaffolding for building agentic data workflows.*
- 🅖 📡 [Developer Knowledge](https://github.com/gemini-cli-extensions/developer-knowledge) - Ask questions about Google APIs and services. *Use case: Inline API doc lookup, code-sample retrieval grounded in current Google docs.*
- 🅖 📡 [Pay and Wallet Developer](https://github.com/gemini-cli-extensions/pay-and-wallet-developer) - Google Pay and Wallet developer tooling. *Use case: Pay button integration, Wallet pass authoring, payment-flow scaffolding.*
- 🛠️ 📡 [Stripe AI](https://github.com/stripe/ai) - Stripe payments. *Use case: Payment flows, subscription management, dispute handling.*
- 🛠️ 📡 [Atlassian Rovo MCP](https://github.com/atlassian/atlassian-mcp-server) - Jira + Confluence (Atlassian's official MCP). *Use case: Issue triage, Confluence search, sprint planning from CLI.*
- 🛠️ 📡 [SonarQube MCP](https://github.com/SonarSource/sonarqube-mcp-server) - Code quality and static analysis. *Use case: Quality-gate inspection, technical-debt tracking.*
- 🛠️ 📡 [Auth0 MCP](https://github.com/auth0/auth0-mcp-server) - Auth0 identity platform. *Use case: Tenant config, user management, application scaffolding.*
- 🛠️ 📡 [Shopify AI Toolkit](https://github.com/Shopify/Shopify-AI-Toolkit) - Shopify e-commerce. *Use case: Product, order, and storefront operations.*
- 🛠️ 📡 [Monday MCP](https://github.com/mondaycom/mcp) - Monday.com project management. *Use case: Board ops, item updates, automation.*
- 🛠️ 📡 [Telnyx](https://github.com/team-telnyx/ai) - Telnyx voice/SMS/WebRTC. *Use case: Communications API workflows.*

## Observability and SRE

- 🅖 📡 [Cloud Logging](https://github.com/gemini-cli-extensions/cloud-logging) - Google Cloud Logging. *Use case: Log search, filter authoring, log-based metric setup.*
- 🅖 📡 [Cloud Monitoring](https://github.com/gemini-cli-extensions/cloud-monitoring) - Google Cloud Monitoring. *Use case: Metric exploration, alert policy authoring, dashboard inspection.*
- 🅖 📡 [SRE Extension](https://github.com/gemini-cli-extensions/sre) - Site Reliability Engineering toolkit for GCP investigations. *Use case: Incident triage, postmortem support, reliability workflows.*
- 🅖 📡 [AlloyDB Observability](https://github.com/gemini-cli-extensions/alloydb-observability) - AlloyDB monitoring metrics. *Use case: AlloyDB performance investigation via natural-language metric queries.*
- 🅖 📡 [Cloud SQL PostgreSQL Observability](https://github.com/gemini-cli-extensions/cloud-sql-postgresql-observability) - Cloud SQL Postgres monitoring. *Use case: Postgres performance investigation, query-level metrics.*
- 🅖 📡 [Cloud SQL MySQL Observability](https://github.com/gemini-cli-extensions/cloud-sql-mysql-observability) - Cloud SQL MySQL monitoring. *Use case: MySQL performance investigation, query metrics.*
- 🅖 📡 [Cloud SQL SQL Server Observability](https://github.com/gemini-cli-extensions/cloud-sql-sqlserver-observability) - Cloud SQL SQL Server monitoring. *Use case: SQL Server performance investigation, system metrics.*
- 🛠️ 📡 [Dynatrace MCP](https://github.com/dynatrace-oss/dynatrace-mcp) - Dynatrace observability. *Use case: APM and infrastructure monitoring queries.*
- 🛠️ 📡 [Grafana MCP](https://github.com/grafana/mcp-grafana) - Grafana dashboards and alerting. *Use case: Dashboard authoring, alert tuning, log correlation.*

## Security

- 🅖 📡 [Gemini CLI Security](https://github.com/gemini-cli-extensions/security) - Code security review. *Use case: Pre-merge security scan, SCA-style review of dependencies, vulnerability flagging in PRs.*
- 🅖 📡 [Google SecOps (CLI extension)](https://github.com/gemini-cli-extensions/google-secops) - Google SecOps OneMCP for the CLI. *Use case: Detection authoring, threat hunting, SOC workflows.*
- 🅖 📡 [MCP Security](https://github.com/google/mcp-security) - Google's broader security operations toolkit. *Use case: Cross-tool security ops via MCP.*
- 🛠️ 📡 [CrowdStrike Falcon MCP](https://github.com/CrowdStrike/falcon-mcp) - CrowdStrike Falcon EDR. *Use case: Endpoint detection queries, incident triage.*

## Productivity and Communication (CLI)

- 🅖 📡 [Google Workspace](https://github.com/gemini-cli-extensions/workspace) - Gmail/Drive/Docs/Sheets/Calendar/Slides/Tasks. *Use case: Same scope as the consumer Connected App, exposed via MCP for CLI workflows.*
- 🅖 📡 [Google Maps Platform Code Assist](https://github.com/googlemaps/platform-ai) - Maps Platform developer surface grounded in official docs and code samples. *Use case: Routes API, Places search, geocoding workflows — get code samples grounded in current docs without context-switching.*
- 🅖 📡 [Maps Grounding Lite](https://github.com/gemini-cli-extensions/maps-grounding-lite) - Lightweight Maps grounding for prompts. *Use case: Inline location grounding for queries that need maps context.*
- 🛠️ 📡 [Raindrop MCP](https://github.com/adeze/raindrop-mcp) - Raindrop.io bookmarks. *Use case: Bookmark search and organization.*

## AI and Agents

- 🅖 📡 [Jules](https://github.com/gemini-cli-extensions/jules) - Async coding agent. *Use case: Background coding tasks delegated from the CLI.*
- 🅖 📡 [Ralph](https://github.com/gemini-cli-extensions/ralph) - Ralph-loop pattern (named for the agent-loop methodology, not our Ralph). *Use case: Recursive self-improving execution loops.*
- 🅖 [Nano Banana](https://github.com/gemini-cli-extensions/nanobanana) - Image generation/editing. *Use case: Inline image creation and editing during CLI sessions.*
- 🅖 📡 [MCP Toolbox](https://github.com/gemini-cli-extensions/mcp-toolbox) - Database tooling abstraction layer. *Use case: Multi-DB MCP convenience wrapper.*
- 🛠️ 🧠 [Skill Porter](https://github.com/jduncan-rva/skill-porter) - Convert Claude Code skills ↔ Gemini CLI extensions. *Use case: Cross-platform reuse of Anthropic skills inside Gemini CLI and vice versa.*
- 🛠️ 🧠 [Superpowers](https://github.com/obra/superpowers) - Skills library (TDD, debug, refactor patterns). *Use case: Plug-and-play engineering discipline patterns.*
- 🛠️ [Caveman](https://github.com/JuliusBrussee/caveman) - Token compression. *Use case: Long-context optimization, cache-friendly prompt shaping.*
- 🛠️ 📡 [HuggingFace MCP](https://github.com/huggingface/hf-mcp-server) - HuggingFace Hub access. *Use case: Model discovery, dataset retrieval, Spaces interaction.*
- 🛠️ 🧠 [HuggingFace Skills](https://github.com/huggingface/skills) - HuggingFace skill bundles. *Use case: Curated workflows around HF models and datasets.*
- 🛠️ 📡 [ElevenLabs MCP](https://github.com/elevenlabs/elevenlabs-mcp) - Voice generation. *Use case: TTS and voice cloning workflows.*
- 🛠️ 📡 [NVIDIA cuOpt Skills](https://github.com/NVIDIA/cuopt) - GPU-accelerated optimization. *Use case: Logistics, routing, scheduling at scale.*
- 🛠️ 📡 [MATLAB Agentic Toolkit](https://github.com/matlab/matlab-agentic-toolkit) - MATLAB scientific compute. *Use case: Numerical workflows, control systems, signal processing.*
- 🛠️ 📡 [Qt AI Skills](https://github.com/TheQtCompanyRnD/agent-skills) - Qt cross-platform UI. *Use case: Qt application development.*

## Web and Browser

- 🅖 📡 [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) - Browser debugging via DevTools protocol. *Use case: DOM inspection, network log capture, performance traces during development.*
- 🛠️ 📡 [Browserbase MCP](https://github.com/browserbase/mcp-server-browserbase) - Headless browser automation. *Use case: Web automation, data extraction, form filling at scale.*
- 🛠️ 📡 [Desktop Commander](https://github.com/wonderwhy-er/DesktopCommanderMCP) - Local shell + filesystem access. *Use case: Mixed CLI + filesystem workflows on the user's machine.*
- 🛠️ 📡 [Exa MCP Server](https://github.com/exa-labs/exa-mcp-server) - Exa neural search. *Use case: High-recall web search, research workflows beyond Google Search.*
- 🛠️ 📡 [Context7](https://github.com/upstash/context7) - Live library documentation lookup. *Use case: Pulling up-to-date API docs into a coding session.*
- 🛠️ 📡 [Figma MCP](https://github.com/figma/mcp-server-guide) - Figma design files. *Use case: Reading Figma frames into a coding session, generating components from designs.*

---

## Contributing

Contributions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md) for the submission flow, the legend conventions, and the entry style guide. By contributing you agree to the [Code of Conduct](code-of-conduct.md).

The CLI side is large (~987 entries in the official registry). We curate the highest-signal extensions rather than mirroring the full registry. Strong third-party submissions welcome — include the GitHub repo URL, the extension's `gemini-extension.json` manifest path, and one specific use case.

## Related

- [Awesome List for Claude Connectors](https://github.com/rdmgator12/awesome-claude-connectors) — Sister directory tracking Anthropic's Claude Connectors Directory (375+ MCP integrations).
- [Awesome Perplexity Connectors](https://github.com/rdmgator12/Perplexity-Connectors-awesome-list-) — Sister directory tracking Perplexity Computer connectors.
- [Awesome ChatGPT Apps](https://github.com/rdmgator12/Chtgpt-Apps-Awesome-List) — Sister directory tracking ChatGPT Apps SDK.
- [Awesome MCP Servers](https://github.com/punkpeye/awesome-mcp-servers) — Broader directory of all known Model Context Protocol servers.
- [Gemini CLI Extensions Registry](https://geminicli.com/extensions/) — Authoritative public registry (browse UI).
- [Gemini CLI Extensions JSON feed](https://geminicli.com/extensions.json) — Parseable feed (~987 entries).
- [Gemini Connected Apps Help Center](https://support.google.com/gemini/answer/13695044) — Google's official Connected Apps documentation.
- [Gemini CLI repository](https://github.com/google-gemini/gemini-cli) — Source of the CLI itself.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Ralph D. Martello](https://github.com/rdmgator12) has waived all copyright and related or neighboring rights to this work.
