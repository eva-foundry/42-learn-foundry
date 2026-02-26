# 42-learn-foundry -- EVA Learning & Reference Repository

**Purpose:** Learning sandbox, external reference repos, and exploratory spikes.
            Patterns learned here are implemented in 29-foundry (production library).

**Relation:** 29-foundry is the production EVA Foundry Library.
              42-learn-foundry is study and exploration only.
              Nothing in this folder is imported by production EVA code.

**Created:** 2026-02-21

---

## Contents

| Directory | Contents | Source |
|-----------|----------|--------|
| `cloned-repos/` | 9 external Microsoft reference repos | Moved from 29-foundry 2026-02-21 |
| `notebooks/` | 4 tutorial Jupyter notebooks (quickstart, RAG, evaluation) | Moved from 29-foundry 2026-02-21 |
| `spikes/` | One-off exploratory scripts and notebooks | Naming: `YYYYMMDD-<topic>.py` or `.ipynb` |

---

## cloned-repos — Reference Repositories

| Repo | Source | Key patterns for EVA |
|------|--------|----------------------|
| `agent-framework/` | microsoft/agent-framework | Core agent patterns, graph orchestration |
| `Agent-Framework-Samples/` | microsoft/Agent-Framework-Samples | Progressive tutorials (chapters 1-9) |
| `azure-search-openai-demo/` | Azure-Samples/azure-search-openai-demo | RAG + hybrid search patterns |
| `contoso-chat/` | Azure-Samples/contoso-chat | Retail RAG reference |
| `contoso-creative-writer/` | Azure-Samples/contoso-creative-writer | Multi-agent writer pattern |
| `mcp/` | microsoft/mcp | MCP protocol specs |
| `mcp-for-beginners/` | microsoft/mcp-for-beginners | MCP tutorial |
| `multi-agent-accelerator/` | Azure-Samples/multi-agent-accelerator | Multi-agent patterns |
| `prompty/` | microsoft/prompty | Prompty format and tooling |
| `spec-to-agents/` | microsoft/spec-to-agents | Spec-driven agent generation |

---

## spikes/

Naming convention: `YYYYMMDD-<topic>.py` or `YYYYMMDD-<topic>.ipynb`

Each spike should include a comment header:
```
# Spike: <topic>
# Date: YYYY-MM-DD
# Informs: <29-foundry path or "none">
# Conclusion: <one line>
```
