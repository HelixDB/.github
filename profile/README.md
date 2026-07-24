<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HelixDB/helix-db/main/assets/full_logo_dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/HelixDB/helix-db/main/assets/full_logo_light.png">
  <img alt="HelixDB" src="https://raw.githubusercontent.com/HelixDB/helix-db/main/assets/full_logo_light.png" width="560">
</picture>

### The database for AI memory

Knowledge graphs, vectors, full-text search, and transactional application data in one Rust engine — built for agents, GraphRAG, and company brains.

[Website](https://helix-db.com) · [Documentation](https://docs.helix-db.com) · [Get started](https://docs.helix-db.com/cli/getting-started) · [Discord](https://discord.gg/2stgMPr5BD)

[![GitHub stars](https://img.shields.io/github/stars/HelixDB/helix-db?style=flat&logo=github&label=Stars)](https://github.com/HelixDB/helix-db)
[![Docs](https://img.shields.io/badge/docs-latest-5b5bd6)](https://docs.helix-db.com)
[![Discord](https://img.shields.io/discord/1354148209005559819?logo=discord&label=Discord)](https://discord.gg/2stgMPr5BD)

</div>

## Give your AI connected context

Vector search finds similar things. Graph traversal explains how they are connected. HelixDB combines both with BM25 full-text search and transactional application data, so your AI can retrieve richer context without stitching together multiple databases.

| Graph-native | Hybrid retrieval | Application-ready |
| --- | --- | --- |
| Model entities, relationships, and typed properties as a labeled property graph. | Combine graph traversal, approximate vector search, and BM25 in the same system. | Use full ACID transactions and type-safe SDKs for Rust, TypeScript, Go, and Python. |

## Start in minutes

```bash
# Install the CLI
curl -sSL "https://install.helix-db.com" | bash

# Create and run a local project (requires Docker or Podman)
mkdir my-helix-app && cd my-helix-app
helix init local
helix start dev

# Run the generated example query
helix query dev --file examples/request.json
```

Local instances start in memory for a fast development loop. Use `helix start dev --disk` when you want data to persist across restarts.

Want an agent to bootstrap the project? Run `helix chef` to scaffold HelixDB, seed starter data, install the Helix skills and docs integration, and hand the build to Codex, Claude Code, or OpenCode.

## Build with Helix

Author strongly typed queries in your application and send them directly to a running instance — no separate query deployment step.

- [Rust SDK](https://docs.helix-db.com/database/rust-project-setup)
- [TypeScript SDK](https://docs.helix-db.com/database/typescript-project-setup)
- [Go SDK](https://docs.helix-db.com/database/go-project-setup)
- [Python SDK](https://docs.helix-db.com/database/python-project-setup)
- [Querying guide](https://docs.helix-db.com/database/querying-guide/overview)

## Scale with Helix Cloud

Helix Cloud runs the graph, vector, and text engines on durable object storage. A gateway routes requests to a dedicated writer and horizontally scaling readers, while tiered memory and SSD caches keep hot data close to compute.

- Object storage is the durable system of record
- Readers auto-scale independently with query load
- Serializable transactions provide full ACID guarantees
- High-availability deployments span multiple gateways and database nodes

[Explore the architecture](https://docs.helix-db.com/database/architecture) · [Get started with Helix Cloud](https://helix-db.com/login)

## Explore the ecosystem

| Repository | What it is |
| --- | --- |
| [`helix-db`](https://github.com/HelixDB/helix-db) | The database engine, CLI, SDKs, and local development workflow. |
| [`graphify-v8`](https://github.com/HelixDB/graphify-v8) | Turn codebases, schemas, documents, and other sources into a queryable knowledge graph. |
| [`skills`](https://github.com/HelixDB/skills) | Agent skills for authoring, translating, and optimizing HelixDB queries. |

---

<div align="center">

**Just use Helix.**

[Star HelixDB](https://github.com/HelixDB/helix-db) · [Join the community](https://discord.gg/2stgMPr5BD) · [Follow on X](https://x.com/helixdb)

</div>
