# Cloned Microsoft & Azure Repositories

**Purpose:** Reference implementations and proven patterns from Microsoft for Azure AI Foundry agent development  
**Last Updated:** February 18, 2026 - 7:09 AM ET  
**Clone Date:** February 17, 2026

---

## 📦 Cloned Repositories Index

### Phase 1: Core Frameworks

#### 1. **agent-framework** ⭐ [microsoft/agent-framework](https://github.com/microsoft/agent-framework)
- **Version:** Latest (cloned with `--depth=1`)
- **Description:** Microsoft's unified framework for building AI agents
- **Key Patterns to Extract:**
  - Graph-based workflow orchestration
  - Multi-agent collaboration patterns
  - OpenTelemetry integration examples
  - Tool/function calling implementations
  - Thread management and serialization
- **Use in EVA:**
  - Base patterns for all agent implementations
  - Workflow orchestration for claim analysis
  - Tool integration patterns
- **Key Files:**
  - `src/agent_framework/` - Core framework code
  - `examples/` - Working examples
  - `docs/` - API documentation

#### 2. **Agent-Framework-Samples** ⭐ [microsoft/Agent-Framework-Samples](https://github.com/microsoft/Agent-Framework-Samples)
- **Version:** Latest
- **Description:** Comprehensive tutorials with 9 progressive chapters
- **Key Patterns to Extract:**
  - Chapter 1: Single agent basics
  - Chapter 2: Multi-agent orchestration (sequential, concurrent)
  - Chapter 3: RAG with file search
  - Chapter 4: MCP integration patterns
  - Chapter 5: Vision and multimodal agents
  - Chapter 6: Code interpreter usage
  - Chapter 7: Bing grounding tool
  - Chapter 8: Evaluation with DevUI
  - Chapter 9: Production deployment
- **Use in EVA:**
  - Learning resource for team onboarding
  - Template for multi-agent jurisprudence workflows
  - Evaluation pipeline patterns
- **Key Files:**
  - `01-*/` - Progressive tutorial chapters
  - `common/` - Shared utilities

#### 3. **prompty** ⭐ [microsoft/prompty](https://github.com/microsoft/prompty)
- **Version:** Latest
- **Description:** Standardized prompt asset format with VS Code extension
- **Key Patterns to Extract:**
  - .prompty file format specification
  - Dynamic template rendering
  - Model configuration switching
  - Integration with LangChain/Semantic Kernel
- **Use in EVA:**
  - Standardize prompt engineering across projects
  - Version control for prompts
  - Rapid prompt iteration workflow
- **Key Files:**
  - `prompty/` - Core library
  - `examples/` - Sample prompts
  - `schema/` - Prompty file schema

---

### Phase 2: RAG & Search Patterns

#### 4. **azure-search-openai-demo** ⭐ [Azure-Samples/azure-search-openai-demo](https://github.com/Azure-Samples/azure-search-openai-demo)
- **Version:** Latest
- **Description:** **THE** production RAG reference implementation
- **Key Patterns to Extract:**
  - Hybrid search (vector + keyword + semantic reranking)
  - Multi-turn chat with citations
  - Document ingestion pipeline
  - Evaluation framework with AI-assisted scoring
  - Authentication and authorization (ACL)
  - Speech input/output integration
- **Use in EVA:**
  - Primary reference for RAG pipeline architecture
  - Citation generation patterns
  - Document preprocessing strategies
  - Query rewriting techniques
- **Key Files:**
  - `app/backend/approaches/` - RAG approach implementations
  - `app/backend/prepdocs.py` - Document ingestion
  - `app/backend/approaches/chatreadretrieveread.py` - Main RAG pattern
  - `scripts/` - Deployment automation

#### 5. **contoso-chat** ⭐ [Azure-Samples/contoso-chat](https://github.com/Azure-Samples/contoso-chat)
- **Version:** Latest
- **Description:** End-to-end retail RAG copilot with full GenAIOps lifecycle
- **Key Patterns to Extract:**
  - Complete development workflow (ideate → evaluate → deploy)
  - Azure AI Foundry integration
  - Prompty usage in production
  - Evaluation pipeline automation
  - Container deployment to Azure Container Apps
  - Responsible AI practices
- **Use in EVA:**
  - GenAIOps workflow template
  - Evaluation pipeline inspiration
  - Deployment automation patterns
- **Key Files:**
  - `contoso_chat/` - Main application
  - `evaluate/` - Evaluation flows
  - `infra/` - Azure deployment (Bicep)

---

### Phase 3: MCP (Model Context Protocol)

#### 6. **mcp** ⭐ [microsoft/mcp](https://github.com/microsoft/mcp)
- **Version:** Latest
- **Description:** Official Microsoft MCP server catalog
- **Key Patterns to Extract:**
  - Azure MCP Server implementation
  - Microsoft Foundry MCP (remote `https://mcp.ai.azure.com`)
  - Azure DevOps, AKS, GitHub MCP servers
  - Azure Fabric, SQL Server integrations
  - Microsoft Learn MCP
- **Use in EVA:**
  - Adapt Azure MCP servers for EI services
  - Create custom MCP for Cosmos DB, Blob Storage
  - Integrate with existing Azure resources
- **Key Files:**
  - `servers/src/azure/` - Azure service MCP implementations
  - `servers/src/foundry/` - Foundry MCP server
  - `schema/` - MCP protocol schemas

#### 7. **mcp-for-beginners** ⭐ [microsoft/mcp-for-beginners](https://github.com/microsoft/mcp-for-beginners)
- **Version:** Latest
- **Description:** Comprehensive MCP curriculum (cross-language)
- **Key Patterns to Extract:**
  - MCP server implementation patterns (Python, .NET)
  - Client integration examples
  - Tool definition patterns
  - Resource provider implementations
- **Use in EVA:**
  - Learning resource for MCP protocol
  - Template for building custom MCP servers
  - Testing and validation patterns
- **Key Files:**
  - `tutorials/` - Step-by-step guides
  - `examples/python/` - Python MCP examples
  - `examples/dotnet/` - .NET MCP examples

---

### Phase 4: Multi-Agent Orchestration

#### 8. **multi-agent-accelerator** ⭐ [microsoft/Multi-Agent-Custom-Automation-Engine-Solution-Accelerator](https://github.com/microsoft/Multi-Agent-Custom-Automation-Engine-Solution-Accelerator)
- **Version:** Latest
- **Description:** Production-ready multi-agent orchestration system
- **Key Patterns to Extract:**
  - Coordinator-centric star topology
  - 5 specialized agents for complex task coordination
  - Azure deployment automation (azd)
  - Cosmos DB for state management
  - Container Apps deployment
- **Use in EVA:**
  - Architecture for multi-agent claim analysis
  - Coordinator pattern for routing queries
  - Production deployment template
- **Key Files:**
  - `src/backend/` - Multi-agent orchestrator
  - `infra/` - Azure infrastructure (Bicep)
  - `docs/` - Architecture diagrams

#### 9. **spec-to-agents** ⭐ [microsoft/spec-to-agents](https://github.com/microsoft/spec-to-agents)
- **Version:** Latest
- **Description:** Event planning multi-agent workflow combining SK and AutoGen
- **Key Patterns to Extract:**
  - Human-in-the-loop workflow with `ctx.request_info()`
  - Service-managed threads (no manual history tracking)
  - Structured output routing with Pydantic
  - Tool integration (Bing Search, Weather API, Calendar)
- **Use in EVA:**
  - Human review patterns for sensitive claims
  - Structured output for eligibility decisions
  - External API integration patterns
- **Key Files:**
  - `src/agents/` - Agent implementations
  - `src/workflows/` - Workflow orchestration

#### 10. **contoso-creative-writer** ⭐ [Azure-Samples/contoso-creative-writer](https://github.com/Azure-Samples/contoso-creative-writer)
- **Version:** Latest
- **Description:** Multi-agent content creation with research, writing, editing agents
- **Key Patterns to Extract:**
  - Multi-agent collaboration workflow
  - Bing Grounding Tool integration
  - Azure AI Search for knowledge base
  - Agent specialization patterns (researcher, writer, editor)
  - Prompty usage across agents
- **Use in EVA:**
  - Template for specialized agents (PolicyAgent, PrecedentAgent, ValidatorAgent)
  - Research → Analysis → Validation workflow
  - Agent communication patterns
- **Key Files:**
  - `src/api/agents/` - Specialized agents
  - `src/api/orchestrator.py` - Agent coordination
  - `src/api/agents/*.prompty` - Agent prompts

---

## 🎯 Pattern Extraction Priority

### Priority 1: RAG Pipeline (Weeks 1-2)
Extract from:
1. `azure-search-openai-demo/app/backend/approaches/`
2. `contoso-chat/contoso_chat/`

**Goal:** Implement production-grade RAG for EI policy documents

### Priority 2: Multi-Agent Orchestration (Weeks 3-4)
Extract from:
1. `Agent-Framework-Samples/02-multi-agent/`
2. `contoso-creative-writer/src/api/agents/`
3. `multi-agent-accelerator/src/backend/`

**Goal:** Build multi-agent claim analysis workflow

### Priority 3: MCP Integration (Weeks 5-6)
Extract from:
1. `mcp/servers/src/azure/`
2. `mcp-for-beginners/examples/python/`

**Goal:** Expose Azure services (Search, Cosmos, Blob) via MCP

### Priority 4: Evaluation & Observability (Weeks 7-8)
Extract from:
1. `azure-search-openai-demo/scripts/` (evaluation)
2. `contoso-chat/evaluate/`
3. `Agent-Framework-Samples/08-evaluation/`

**Goal:** Automated quality assessment and tracing

---

## 📝 Usage Notes

### Extracting Patterns

When extracting code from these repositories:

1. **Adapt, don't copy blindly**
   - Repositories contain many features not needed for EVA
   - Extract core patterns and adapt to jurisprudence domain

2. **Preserve attribution**
   - Add comments indicating source repository
   - Link to original file in cloned repo

3. **Update dependencies**
   - Cloned repos may use older package versions
   - Update to versions in `../requirements.txt`

4. **Test thoroughly**
   - Patterns may assume specific Azure configurations
   - Validate with EVA's Azure resources

### Example Extraction

```python
# Extracted from: cloned-repos/azure-search-openai-demo/app/backend/approaches/chatreadretrieveread.py
# Original: https://github.com/Azure-Samples/azure-search-openai-demo
# Adapted for: EVA Jurisprudence policy search

from tools.search import AzureSearchClient
from tools.rag import RAGContextBuilder

class ChatReadRetrieveReadApproach:
    """
    Retrieve-Then-Read RAG approach adapted from azure-search-openai-demo.
    
    Flow: Query → Hybrid Search → Context Window → LLM → Response with Citations
    """
    # ... implementation ...
```

---

## 🔄 Update Strategy

### When to Re-clone

Re-clone repositories when:
- Microsoft releases major framework updates
- Breaking API changes announced
- Quarterly review of patterns (March, June, Sept, Dec)

### Preserving Local Changes

If you modify cloned repos for experimentation:
```bash
# Create a branch to preserve changes
cd cloned-repos/azure-search-openai-demo
git checkout -b eva-experiments
git commit -am "EVA-specific modifications"

# To update from upstream later:
git fetch origin
git checkout main
git pull origin main
```

---

## 📊 Repository Statistics

| Repository | Language | Stars | Last Update | Size |
|-----------|----------|-------|-------------|------|
| agent-framework | Python/.NET | 7.2k | Active | ~50 MB |
| Agent-Framework-Samples | Python | 188 | Active | ~20 MB |
| prompty | Python | 1.2k | Active | ~10 MB |
| azure-search-openai-demo | Python | 7.6k | Active | ~80 MB |
| contoso-chat | Python | 755 | Active | ~30 MB |
| mcp | Multiple | 2.6k | Active | ~40 MB |
| mcp-for-beginners | Multiple | 14.4k | Active | ~100 MB |
| multi-agent-accelerator | Python | 705 | Active | ~60 MB |
| spec-to-agents | Python | 73 | Active | ~15 MB |
| contoso-creative-writer | Python | 414 | Active | ~25 MB |

**Total Disk Space:** ~430 MB

---

## 🚫 What NOT to Extract

Avoid extracting:
- ❌ Infrastructure code (Bicep/Terraform) - EVA has its own infra
- ❌ Frontend UI code - EVA Faces handles UI separately
- ❌ Authentication flows - EVA has custom ESDC auth
- ❌ Deployment scripts - EVA uses own CI/CD
- ❌ Sample data - Use EI policy documents instead

**Extract ONLY:**
- ✅ Python agent patterns
- ✅ RAG pipeline logic
- ✅ Tool/function calling examples
- ✅ Evaluation frameworks
- ✅ Observability patterns
- ✅ Prompty templates

---

## 📚 Additional Resources

- **Microsoft Agent Framework Docs:** https://aka.ms/ai-agents-beginners/agent-framework
- **Azure AI Foundry Portal:** https://ai.azure.com
- **MCP Specification:** https://github.com/modelcontextprotocol/specification
- **Prompty Documentation:** https://prompty.ai

---

**Next Steps:**
1. Review each repository's README for overview
2. Explore Priority 1 patterns (RAG pipeline)
3. Create `../agent-framework/examples/` based on extracted patterns
4. Document extracted patterns in `../docs/`
