# Cross-Competitor Synthesis — Raw Notes

> Companion to [cross_competitor_synthesis.html](cross_competitor_synthesis.html).
>
> **Date:** 2026-05-15
> **Scope:** 7 competitors (Jira, Linear, ClickUp, monday, Notion, Plane, Asana) + QPM (TODO cells).

---

## Source documents

This synthesis draws from the 7 per-competitor research bundles already in this folder. For verbatim quotes, see each `*_raw_notes.md`.

| Competitor | HTML doc | Raw notes | Summary |
|---|---|---|---|
| Jira | [jira_ai_research.html](jira_ai_research.html) | (original) | — |
| Linear | [linear_ai_research.html](linear_ai_research.html) | [linear_ai_research_raw_notes.md](linear_ai_research_raw_notes.md) | [linear_ai_research_summary.md](linear_ai_research_summary.md) |
| ClickUp | [clickup_ai_research.html](clickup_ai_research.html) | [clickup_ai_research_raw_notes.md](clickup_ai_research_raw_notes.md) | [clickup_ai_research_summary.md](clickup_ai_research_summary.md) |
| monday | [monday_ai_research.html](monday_ai_research.html) | [monday_ai_research_raw_notes.md](monday_ai_research_raw_notes.md) | [monday_ai_research_summary.md](monday_ai_research_summary.md) |
| Notion | [notion_ai_research.html](notion_ai_research.html) | [notion_ai_research_raw_notes.md](notion_ai_research_raw_notes.md) | [notion_ai_research_summary.md](notion_ai_research_summary.md) |
| Plane | [plane_ai_research.html](plane_ai_research.html) | [plane_ai_research_raw_notes.md](plane_ai_research_raw_notes.md) | [plane_ai_research_summary.md](plane_ai_research_summary.md) |
| Asana | [asana_ai_research.html](asana_ai_research.html) | [asana_ai_research_raw_notes.md](asana_ai_research_raw_notes.md) | [asana_ai_research_summary.md](asana_ai_research_summary.md) |

---

## Feature samples per capability

Concrete examples of what each capability looks like in practice, plus standout per-competitor angles. Mirrors §03 "Feature samples per capability" section of the HTML.

### 01. Conversational assistant

**Common feature samples**
- Q&A over workspace data ("what's blocking the auth project?")
- Summarize long threads, comments, status updates
- Draft emails, status updates, project briefs
- Rewrite, translate, adjust tone
- Inline slash-commands in editors

**Notable per competitor**
- **Linear:** Ask in Cmd+K command bar — keyboard-first
- **Notion:** /ai inline; long-context transforms over whole docs
- **Asana:** Smart Status auto-pulls latest project state
- **Plane:** Ask mode runs on BYO Anthropic/OpenAI keys
- **ClickUp:** Brain² lives across tasks/docs/chat without switching context

### 02. Autonomous multi-step agents

**Common feature samples**
- Triage incoming work — label, assign, link duplicates
- Generate project plan from one-line brief
- Run reviews across an epic (security, compliance, scope)
- Auto-close stale issues; escalate blocked work
- Multi-step report generation across pages/projects

**Notable per competitor**
- **Linear:** Triage Intelligence auto-labels, routes, dedups (Mar 24, 2026)
- **Notion:** 20-minute autonomous research/report runs (Notion 3.0, Sep 2025)
- **Asana:** 21 prebuilt teammates — AI Project Manager, AI Sprint Planner, etc.
- **ClickUp:** Super Agents for end-to-end project setup
- **Plane:** Assign mode hands ticket to AI

### 03. No-code agent / workflow builder

**Common feature samples**
- Drag-drop canvas with AI nodes
- Trigger → AI action → outcome chains
- Template library
- Custom prompts + conditional logic
- Test/preview mode

**Notable per competitor**
- **Asana:** AI Studio — credit-metered
- **Plane:** Build mode + Agent Development Kit (developer-leaning)
- **Notion:** Custom Agents builder + Agent SDK + Notion Workers
- **monday:** Visual builder with AI block recipes
- **Linear:** deliberately absent — bets on external agents

### 04. Agent marketplace / prebuilts

**Common feature samples**
- Curated agent catalog by persona
- Third-party agent installation
- Per-agent pricing + billing
- Verified/certified badges
- Activity logs + performance metrics

**Notable per competitor**
- **monday:** Agentalent.ai — $2K/mo per agent (AWS+Anthropic, Mar 2026)
- **Asana:** 21 prebuilt teammates by job function
- **Linear:** Cursor/Codex/Devin/Replit as external agents via SDK
- **Plane:** Open-source agent marketplace
- **ClickUp:** Super Agents library

### 05. MCP server

**Common feature samples**
- Read tasks/projects/users via Claude/Cursor/Codex/IDE
- Write tasks (create, update, comment, move)
- Query workspace state with natural language
- Cross-tool agent workflows
- OAuth per-user permission scopes

**Notable per competitor**
- **Plane:** 55+ tools, HTTP + PAT + Stdio transports, open source
- **ClickUp:** omits delete tools by design
- **Notion:** permission inheritance preserved through MCP calls
- **Linear:** built for Claude/Cursor/Codex flows
- **Asana:** absent — only competitor without public MCP

### 06. Multi-model gateway / BYO keys

**Common feature samples**
- Pick model per task
- BYO API keys (Anthropic/OpenAI direct)
- Cost transparency per call/user/project
- Failover between providers
- Visible model picker in UI

**Notable per competitor**
- **ClickUp:** widest menu — Claude, GPT, Gemini, o3, MiniMax in Brain MAX
- **Plane:** BYO direct-to-provider Anthropic OR OpenAI
- **Linear:** deliberately single-model (Claude)
- **Asana:** orchestrated, not user-pickable
- **Notion:** GPT-5 + Claude, task-dependent routing

### 07. Memory / context substrate

**Common feature samples**
- AI references past project decisions without re-prompting
- Cross-project relationship awareness
- Persistent "memory" facts across sessions
- Inheritance from parent/child entities
- Permission-aware retrieval

**Notable per competitor**
- **Asana:** Work Graph® + Memory Associations (text-fact, deliberately not vector DB)
- **Notion:** pages-as-memory — natural moat from existing user docs
- **ClickUp:** ActionQuery via Qatalog ($25.4M acquisition)
- **monday:** mondayDB columnar substrate
- **Linear/Jira:** structured issue graph

### 08. Enterprise search (cross-tool)

**Common feature samples**
- Search across Slack/Gmail/Drive/GitHub/Jira simultaneously
- Permission-aware retrieval
- Citations linked to source
- Federated answers from multiple connectors
- Saved searches + alerts

**Notable per competitor**
- **Notion:** AI Connectors with permission inheritance — cleanest enterprise model
- **ClickUp:** Brain MAX (Qatalog ActionQuery)
- **Jira:** Rovo Search across Atlassian suite
- **Asana:** AI Connectors — OpenAI/Slack/Notion
- **Plane/Linear/monday:** workspace-scoped, limited

### 09. Slack / Teams AI intake

**Common feature samples**
- @mention to create tickets from chat
- Standup summaries into PM tool
- Notification triage
- Conversational task management in chat
- Cross-tool slash-commands

**Notable per competitor**
- **Plane:** @Plane in any channel, "AGI-like" framing, Claude Sonnet 4.0 (Nov 15, 2025)
- **Linear:** Linear Asks — intake → triage → ticket flow
- **ClickUp:** Brain in Slack with task context
- **Jira:** Rovo agents in Slack
- **monday/Notion/Asana:** standard integrations, less AI-native

### 10. Code / dev-tool intelligence

**Common feature samples**
- PR ↔ issue automatic linking
- Code-aware ticket summaries
- AI code review on linked PRs
- Test/regression suggestions from diff
- IDE plugins (VS Code, Cursor, JetBrains)

**Notable per competitor**
- **Linear:** Code Intelligence beta (May 14, 2026) + Cursor/Codex/Devin/Replit
- **ClickUp:** Codegen acq (Dec 23, 2025) at $10/10K credits
- **Plane:** GitHub native, dev DNA
- **Asana:** 3 Product/Eng teammates — narrow
- **monday/Notion:** weak

### 11. Governance / human-in-the-loop

**Common feature samples**
- Approval gates before consequential actions
- Audit log of AI actions
- Permission inheritance through AI retrieval
- AI citation/source linking
- Data exclusion zones
- Per-user/workspace AI on/off toggle

**Notable per competitor**
- **Asana:** every consequential action requires user approval ("context, checkpoints, controls")
- **Notion:** "Verify any page" — every AI answer cites a page
- **Plane:** "no prompt storage" + air-gap
- **ClickUp:** MCP omits delete tools
- **Jira:** Atlassian Trust Center + admin controls

### 12. Self-hosted / air-gapped

**Common feature samples**
- Docker/K8s deployment
- BYO LLM endpoint
- No outbound calls (full air-gap)
- Customer-controlled data residency
- Full AI feature parity with cloud

**Notable per competitor**
- **Plane:** only one with full AI parity self-hosted — Fortune 10, Lithuania, France
- **Jira:** Data Center legacy on-prem, AI limited
- **Others:** no self-host

### 13. Pricing model (AI bundling)

**Common feature samples**
- Flat AI in higher seat tier
- Per-credit metering for autonomous work
- Quarterly credit quotas by tier
- Per-agent monthly fees (marketplace)
- BYO keys = customer pays provider direct

**Notable per competitor**
- **Linear:** cleanest — AI bundled, no separate SKU
- **Asana:** quarterly quotas (50K/100K/5M per tier) — enterprise forecasting
- **monday:** $0.01/credit — most usage-flexible
- **ClickUp:** hybrid add-on + credits — most complex
- **Plane:** AI every plan + BYO keys for self-host

### 14. Open source

**Common feature samples**
- Public GitHub repo
- Community contributions
- Forkable codebase
- Permissive / source-available license
- Public roadmap

**Notable per competitor**
- **Plane:** github.com/makeplane/plane — only OSS competitor
- **All others:** closed-source SaaS

---

## Capability matrix — raw data (14 rows × 7 competitors)

The data underlying §03 of the HTML, in tabular form for downstream filtering/import.

### Row 1 — Conversational assistant

| Competitor | Feature name | First delivered | Tech enabler |
|---|---|---|---|
| Jira | Atlassian Intelligence | 2024 GA | LLM via Bedrock + OpenAI |
| Linear | Linear Ask | 2024 | RAG over workspace |
| ClickUp | ClickUp Brain → Brain² | 2023 (Brain² rebrand 2025) | Multi-model |
| monday | AI Blocks → Sidekick | 2023 (Sidekick 2026) | Multi-model gateway |
| Notion | Notion AI | 2023 | GPT + Claude |
| Plane | Plane AI — Ask mode | Nov 2025 | BYO Anthropic/OpenAI |
| Asana | Asana AI (Smart Fields, summaries) | 2023+ | OpenAI + Anthropic |

### Row 2 — Autonomous multi-step agents

| Competitor | Feature name | First delivered | Tech enabler |
|---|---|---|---|
| Jira | Rovo Agents | 2024 | Atlassian Intelligence agent platform |
| Linear | Linear Agent (Agent Sessions API) | Mar 24, 2026 | Agent Interaction SDK + Anthropic |
| ClickUp | Super Agents | Dec 22, 2025 | Brain² + ActionQuery (Qatalog) |
| monday | Sidekick/Vibe/Agents triad | 2025-2026 | AI Platform Gateway |
| Notion | Notion Agent (20-min autonomous) | Sep 18, 2025 (Notion 3.0) | GPT-5 |
| Plane | Plane AI — Assign mode | Nov 2025 | Agent SDK |
| Asana | AI Teammates (21 prebuilts) | Beta Jun 2024, GA Q1 FY27 (≈ May 2026) | Multi-LLM + Work Graph + Memory |

### Row 3 — No-code agent / workflow builder

| Competitor | Feature name | First delivered |
|---|---|---|
| Jira | Rovo Studio | 2024 |
| Linear | — | N/A — bets on external agents instead |
| ClickUp | Brain MAX / Custom Agents | 2025 |
| monday | AI Agent builder | 2026 |
| Notion | Custom Agents | Feb 24, 2026 beta |
| Plane | Plane AI Build mode + Agent Development Kit | Nov 2025 |
| Asana | AI Studio | 2024 |

### Row 4 — Agent marketplace / prebuilts

| Competitor | Feature name | Notable | First delivered |
|---|---|---|---|
| Jira | Atlassian Marketplace | Legacy | legacy |
| Linear | External agents via SDK (Cursor/Codex/Devin/Replit) | Curated partner list | 2026 |
| ClickUp | Super Agents library | In-product | 2025 |
| monday | Agentalent.ai | AWS + Anthropic; $2K/mo per agent | Mar 23, 2026 |
| Notion | Custom Agents catalog | Credit-priced | 2026 |
| Plane | Agent Marketplace | OSS-friendly | 2025 |
| Asana | 21 prebuilt AI Teammates (7 Marketing, 6 Ops/PMO, 5 IT, 3 Product/Eng) | Curated | 2026 |

### Row 5 — MCP server

| Competitor | Endpoint | Transport | Auth | OSS? |
|---|---|---|---|---|
| Jira | Atlassian Remote MCP | HTTP | OAuth | No |
| Linear | Linear MCP | HTTP | OAuth + PAT | No |
| ClickUp | `mcp.clickup.com/mcp` | HTTP | OAuth | No — omits delete tools |
| monday | `mcp.monday.com/mcp` | HTTP | OAuth | No |
| Notion | `mcp.notion.com/mcp` | HTTP | OAuth | No — permission inheritance |
| Plane | `mcp.plane.so/http/mcp` + Stdio | HTTP + PAT + Stdio | OAuth + PAT | **Yes — github.com/makeplane/plane-mcp-server, 55+ tools** |
| Asana | — | — | — | **NO public MCP** |

### Row 6 — Multi-model gateway / BYO keys

| Competitor | Models | Customer model picker? | BYO keys? |
|---|---|---|---|
| Jira | Bedrock + OpenAI | No | No |
| Linear | Claude (Anthropic) | No | No |
| ClickUp | Claude / GPT / Gemini / o3 / MiniMax | Yes (Brain MAX) | No |
| monday | Multi-model | Partial | No |
| Notion | GPT-5 + Claude | Limited | No |
| Plane | Anthropic OR OpenAI | Yes | **Yes — BYO direct provider** |
| Asana | OpenAI + Anthropic | No (orchestrated) | No |

### Row 7 — Memory / context substrate

| Competitor | Substrate | Type |
|---|---|---|
| Jira | Issue graph + Confluence pages | Relational + docs |
| Linear | Issue graph (structured tickets) | Relational |
| ClickUp | Brain Workspace + ActionQuery (Qatalog) | Hybrid |
| monday | mondayDB | Columnar DB |
| Notion | Pages-as-memory | Pages + linked databases — natural moat |
| Plane | Workspace context | Projects + docs |
| Asana | **Work Graph® + Memory Associations** | Relational graph + text-fact (deliberately not vector DB) |

### Row 8 — Enterprise search (cross-tool)

| Competitor | Feature | Notable |
|---|---|---|
| Jira | Rovo Search | Cross-Atlassian |
| Linear | — | Limited |
| ClickUp | Brain MAX (Qatalog acquisition) | $25.4M-funded Qatalog acq Nov 12, 2025 |
| monday | — | Limited |
| Notion | Enterprise Search + AI Connectors | Permission inheritance |
| Plane | Workspace-scoped | Limited |
| Asana | AI Connectors (OpenAI/Slack/Notion) | 2025 |

### Row 9 — Slack/Teams AI intake

| Competitor | Feature | Notable |
|---|---|---|
| Jira | AI in Slack via Rovo | 2024 |
| Linear | Linear Asks (Slack) | 2024 |
| ClickUp | Brain in Slack | 2024 |
| monday | Slack integration | Basic |
| Notion | Slack integration | Basic |
| Plane | @Plane in any channel | Nov 15, 2025, Claude Sonnet 4.0, "AGI-like" framing |
| Asana | Slack integration | Basic |

### Row 10 — Code / dev-tool intelligence

| Competitor | Feature | Notable |
|---|---|---|
| Jira | DX + Forge | Legacy |
| Linear | **Code Intelligence + external dev agents** | May 14, 2026 beta — Cursor/Codex/Devin/Replit |
| ClickUp | Codegen acq | Dec 23, 2025 — $10/10K credits |
| monday | — | Weak |
| Notion | — | Weak |
| Plane | GitHub integration | Dev-focused product DNA |
| Asana | 3 Product/Eng teammates | Narrow |

### Row 11 — Governance / HITL

| Competitor | Brand position |
|---|---|
| Jira | Atlassian Trust Center |
| Linear | Engineering-grade defaults |
| ClickUp | Workspace permissions + no-delete MCP |
| monday | Standard enterprise |
| Notion | **"Verify any page"** — AI citations |
| Plane | **"No prompt storage"** + air-gapped |
| Asana | **"Context, checkpoints, controls"** + Asana Gov — every consequential action requires user approval |

### Row 12 — Self-hosted / air-gapped

| Competitor | Self-host? | AI parity self-hosted? |
|---|---|---|
| Jira | Data Center (legacy) | Limited |
| Linear | No | N/A |
| ClickUp | No | N/A |
| monday | No | N/A |
| Notion | No | N/A |
| Plane | **Docker / K8s / air-gapped** | **Full AI parity** |
| Asana | No | N/A |

### Row 13 — Pricing model (AI bundling)

| Competitor | Seat | AI bundle | AI metering |
|---|---|---|---|
| Jira | Standard $7.53 / Premium $13.53 | Premium+ | Rovo agents metered |
| Linear | Basic $8 / Business $14 | Bundled | None |
| ClickUp | Unlimited $7 / Business $12 | Brain $7/user add-on | Codegen $10/10K credits |
| monday | Basic $9 / Standard $12 / Pro $19 | Sidekick/Vibe in tier | $0.01/credit |
| Notion | Plus $10 / Business $18 | Bundled (higher tiers) | Custom Agents $10/1000 credits |
| Plane | Pro $8 / Business $15 | **All plans, no upcharge** | BYO keys — pay provider direct |
| Asana | Starter $10.99 / Advanced $24.99 | Basic AI in tier | AI Studio: 50K Starter / 100K Plus / 5M Pro per quarter |

### Row 14 — Open source

| Competitor | OSS? |
|---|---|
| All except Plane | No |
| Plane | **Yes** — github.com/makeplane/plane |

---

## 12-month vectors — full notes

### Jira / Atlassian
- **Primary bet**: AI defends installed base via Rovo.
- **Recent commits**: Rovo Studio agent platform, deeper Atlassian Intelligence across Jira/Confluence/Loom/Compass, Forge as AI extensibility runtime.
- **Why**: 300K+ customer base under disruption pressure. AI is retention story.

### Linear
- **Primary bet**: Become the orchestration layer for AI dev agents. "Issue tracking is dead."
- **Recent commits**: Linear Agent (Mar 24, 2026), Code Intelligence beta (May 14, 2026), Agent Interaction SDK, external agent ecosystem (Cursor/Codex/Devin/Replit).
- **Why**: Karri Saarinen + Akshay Kothari thesis — Linear is the interface, not the runtime. Own the dev-agent interaction surface before someone else does.

### ClickUp
- **Primary bet**: AI work-OS by acquisition.
- **Recent commits**: Qatalog acquisition Nov 12, 2025 ($25.4M-funded) → ActionQuery enterprise search. Codegen acquisition Dec 23, 2025 → dev AI. Super Agents Dec 22, 2025. Brain MAX as multi-model gateway. Ambient Agents.
- **Why**: Zeb Evans is buying capabilities ClickUp can't build organically. Bet on customers wanting one tool, not seven.

### monday.com
- **Primary bet**: "All In on AI" repositioning. AI Work Platform brand.
- **Recent commits**: Sidekick/Vibe/Agents triad (May 6, 2026 repositioning). Agentalent.ai marketplace Mar 23, 2026 (AWS + Anthropic, $2K/mo per agent). AI Platform Gateway. $0.01/credit pricing.
- **Why**: Capture mid-market AI workflow spend. Marketplace economics as moat — customers + agent builders both on monday = defensible.

### Notion
- **Primary bet**: Workspace-as-memory + verify-any-page + Developer Platform 3.5.
- **Recent commits**: Notion 3.0 GPT-5 rebuild (Sep 18, 2025). 20-min autonomous Notion Agent. Custom Agents (Feb 24, 2026 beta) + $10/1000 credit pricing (May 4, 2026). Developer Platform 3.5 (May 13, 2026): External Agents API, Notion Workers, Agent SDK, CLI. OpenAI customer case study.
- **Why**: Own the workspace context substrate before others do. Pages-as-memory is the natural moat.

### Plane
- **Primary bet**: OSS + self-host + air-gap + BYO keys = the regulated/gov segment.
- **Recent commits**: Plane AI (Ask/Build/Assign modes, Nov 2025). Slack/Teams AI intake Nov 15, 2025 (Claude Sonnet 4.0). MCP open source (55+ tools). Plane Compose YAML Projects-as-Code. Prime CLI + God Mode. Fortune 10 + Government of Lithuania + République Française as proof points.
- **Why**: Vamsi Kurama's "steerable systems" thesis. Target the segment the other 6 cannot serve. $4M seed from OSS Capital sets the constraint.

### Asana
- **Primary bet**: AI Teammates GA Q1 FY27 as public-market rerating catalyst.
- **Recent commits**: 21 prebuilt AI Teammates (7 Marketing + 6 Ops/PMO + 5 IT + 3 Product/Eng). Sales-led GA Q1 FY27 (≈ May 2026); self-serve H2 FY27. AI Studio credit tiers. Work Graph + Memory Associations. Asana Gov Winter 2026.
- **Why**: ASAN stock down ~50% YTD, ~92% from ATH. FY27 guidance $850M-$858M with **15% net new ARR from AI products** locked in. Teammates GA at Q1 FY27 earnings (≈ Aug 2026) is the rerating moment.

---

## Dimension data — raw

### Pricing (May 2026 sticker prices, USD per seat/month, annual billing)

| Competitor | Free | Lower tier | Mid tier | Upper tier | Enterprise |
|---|---|---|---|---|---|
| Jira | Yes | Standard $7.53 | Premium $13.53 | — | Sales |
| Linear | Yes | Basic $8 | Business $14 | — | Sales |
| ClickUp | Yes | Unlimited $7 | Business $12 | Business+ $19 | Sales |
| monday | Yes | Basic $9 | Standard $12 | Pro $19 | Sales |
| Notion | Yes | Plus $10 | Business $18 | — | Sales |
| Plane | Yes | Pro $8 | Business $15 | — | Self-host |
| Asana | Personal Free | Starter $10.99 | Advanced $24.99 | — | Sales |

### MCP — full inventory

| Competitor | Endpoint | Transport | OSS | Special |
|---|---|---|---|---|
| Jira | Atlassian Remote MCP | HTTP | No | Cross-product context |
| Linear | Via developers.linear.app | HTTP | No | Designed for Claude/Cursor/Codex |
| ClickUp | mcp.clickup.com/mcp | HTTP | No | Omits delete tools |
| monday | mcp.monday.com/mcp | HTTP | No | Tied to Agentalent |
| Notion | mcp.notion.com/mcp | HTTP | No | Permission inheritance |
| Plane | mcp.plane.so/http/mcp + Stdio | HTTP + PAT + Stdio | **Yes** | 55+ tools, self-host transport |
| Asana | — | — | — | **Conspicuous absence** |

### Governance — phrases owned

- Asana: "context, checkpoints, controls"
- Notion: "verify any page" (AI citations)
- Plane: "no prompt storage" + air-gapped
- ClickUp: no-delete MCP tools (technical, not brand)
- Others: no distinctive phrase

### Model gateways — coverage

| Competitor | Claude | OpenAI | Gemini | Other | Customer-picker |
|---|---|---|---|---|---|
| Jira | ✓ | ✓ | — | — | No |
| Linear | ✓ (primary) | — | — | — | No |
| ClickUp | ✓ | ✓ | ✓ | o3, MiniMax | **Yes** |
| monday | ✓ | ✓ | — | Other | Partial |
| Notion | ✓ | ✓ (GPT-5) | — | — | Limited |
| Plane | ✓ | ✓ | — | — | **Yes (BYO)** |
| Asana | ✓ | ✓ | — | — | No |

---

## QPM TODO checklist

To complete the synthesis, fill these inputs:

- [ ] QPM feature inventory mapped to the 14 capability rows
- [ ] QPM 12-month roadmap with committed dates
- [ ] QPM target buyer segment (defender / repositioner / outlier)
- [ ] QPM pricing model intent (bundled / metered / hybrid)
- [ ] QPM data residency & self-host posture
- [ ] QPM governance brand candidate phrase
- [ ] QPM memory substrate decision (relational / vector / pages-as-memory / text-fact)
- [ ] QPM agent philosophy (runtime vs. interface)

---

## Sources used in this synthesis

All sources are aggregated from the 7 individual competitor research bundles. The HTML doc references those bundles directly; this raw-notes file captures the per-row data points for downstream import or filtering.

For verbatim source quotes (CEO statements, earnings call excerpts, changelog entries, X/Twitter posts, press releases), see:

- [jira_ai_research.html](jira_ai_research.html)
- [linear_ai_research_raw_notes.md](linear_ai_research_raw_notes.md)
- [clickup_ai_research_raw_notes.md](clickup_ai_research_raw_notes.md)
- [monday_ai_research_raw_notes.md](monday_ai_research_raw_notes.md)
- [notion_ai_research_raw_notes.md](notion_ai_research_raw_notes.md)
- [plane_ai_research_raw_notes.md](plane_ai_research_raw_notes.md)
- [asana_ai_research_raw_notes.md](asana_ai_research_raw_notes.md)
