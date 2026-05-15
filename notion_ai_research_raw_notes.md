# Notion AI — Raw Research Notes

> Working notes collected for [notion_ai_research.html](notion_ai_research.html). Verbatim extracts from each source.
>
> **Run date:** 2026-05-15
> **Lens:** Notion as a Jira + Confluence equivalent (PM + wiki).
> **Method:** WebFetch + WebSearch. No Notion MCP / playwright access in this session.

---

## Table of contents

1. [notion.com/product/ai — feature inventory](#1-notioncomproductai)
2. [notion.com/releases — recent updates](#2-notioncomreleases)
3. [Notion 3.0 launch (Sep 18, 2025)](#3-notion-30-launch-sep-18-2025)
4. [Notion AI Meeting Notes](#4-notion-ai-meeting-notes)
5. [Notion MCP server](#5-notion-mcp-server)
6. [Pricing + Notion Credits](#6-pricing--notion-credits)
7. [Notion vs Confluence (wiki lens)](#7-notion-vs-confluence)
8. [Notion vs Jira (PM lens)](#8-notion-vs-jira)
9. [Developer Platform 3.5 (May 13, 2026)](#9-developer-platform-35)
10. [Community sentiment](#10-community-sentiment)
11. [Open questions / gaps](#11-open-questions--gaps)
12. [Recommended screenshots](#12-recommended-screenshots)

---

## 1. notion.com/product/ai

### Marketing positioning (verbatim)
- "Meet your 24/7 AI team"
- "Infinite minds, built for teamwork. Answer questions, prioritize tasks, and write reports—all while you sleep."
- "Custom Agents automate work that repeats."
- "Your Notion Agent can build, edit, and take action."
- "Enterprise Search finds answers across all your apps."
- "AI Meeting Notes gives your team perfect meeting memory."

### Features

**Notion Agent (personal)**
- "Does work for you. Completes complex, multi-step tasks using context from Notion, your connected apps, and the web."
- Surface: Chat-based agent; can "build, edit, and take action"
- "Anything you can do in Notion, your Notion Agent can do for you."
- Plan: Business+
- Status: GA

**Custom Agents**
- "AI agents handle repetitive tasks autonomously"
- Set up once with trigger/schedule; runs 24/7
- "Free to try, then $10 per 1,000 credits"
- Free through May 3, 2026; credits required starting May 4, 2026
- Plan: Business & Enterprise
- Status: GA

**AI Meeting Notes**
- Tagline: "Perfectly written by AI"
- "transcribe conversations, summarize key points, and surface insights automatically"
- "no bot needed"
- Plan: Business+
- Status: Beta

**Enterprise Search**
- "Search across Slack, Google Drive, GitHub & more—in seconds."
- Plan: Business+
- Status: **Beta**

**Research Mode**
- "Dive deep on a topic… to generate detailed reports and summaries."
- Status: GA

**AI Blocks (inline)**
- "Improve writing or generate drafts… directly in your pages."

**Autofill / Database AI**
- "auto-populate properties with Autofill, and write formulas for smarter workflows and automations"

**Notion AI Connectors**
- Used with Enterprise Search

### PM (Jira-like) capabilities
- Databases: "subtasks, dependencies, custom properties and more" (Free+)
- Projects product
- AI: create databases, autofill properties, write formulas
- Custom Agents can route tasks, share project updates
- Use cases: "Go from brainstorm to roadmap" · "Automate weekly reporting" · "Triage product feedback"

### Wiki (Confluence-like) capabilities
- Knowledge Base: "Centralize your knowledge"
- Docs: "Simple and powerful"
- **"Verify any page"**: "Add a verified badge to pages that are up to date. Appears in search results and AI citations."
- Private teamspaces
- Granular database permissions
- Use cases: "Onboard a new hire" · "Resolve support tickets in Slack"

### Multi-model claims
- "Model agnostic"
- "Switch any workflow to a different model or provider, without losing any context."
- /product/ai page does NOT name GPT-5, Claude, o3 specifically — those come from /pricing and OpenAI case study

### Data / Privacy stance
- "No training on your data" — contractual prohibitions with AI subprocessors
- **Zero data retention for Enterprise**
- **30-day retention for non-Enterprise**
- **HIPAA compliant for Enterprise**
- SOC 2 Type 2, ISO 27001, GDPR, CCPA
- "data is encrypted in-transit using TLS 1.2 or greater"

---

## 2. notion.com/releases

### May 13, 2026 — 3.5: Notion Developer Platform
- **External Agents API (Alpha):** Bring third-party agents (Claude, Codex, Decagon, custom-built) into Notion as orchestration layer
- **Database sync (Beta):** Pull data from any API source via Workers
- **Custom agent tools (Beta):** Deterministic code-based tools, "a fraction of the token cost"
- **Webhook triggers (Beta):** Any app can trigger Notion workflows
- **Notion Workers:** Hosted runtime sandbox; free during beta → Notion credits starting Aug 11, 2026
- **Notion CLI:** Command-line tool for devs and coding agents
- **Agent SDK (Alpha waitlist):** Embed Notion Agents inside other apps (CRM, MS Teams, Discord, Amplitude, Hex)
- **Connections tab:** Unified mgmt for personal/workspace connections, PATs, internal API connections
- **Agents "hall of fame":** Library of agent templates from Ramp, Clay, Vercel
- **Markdown API**
- **Notion MCP updates** — works with Meeting Notes/block comments; **91% more token-efficient** for creating/updating databases
- **Notion API:** Any member can build connections; workspace-scoped OAuth and PATs
- **Developer Portal & rebuilt Docs** with built-in AI assistant

### May 7, 2026 — Plan Mode
- For complex agent requests (bulk rewrites, database updates) agent now asks clarifying questions and builds a detailed plan before acting
- "Aiming to reduce drift in multi-step work"

### May 6, 2026 — New Custom Agent Directory
- Custom Agents have a dedicated section in your Library
- Browse workspace agents, pin favorites, create new ones
- Access via `Library` → `Agents`

### May 5, 2026 — New Custom Agent controls for admins
- "Following over a million Custom Agents created since the beta launch two months earlier"
- **Guardrails:** Restrict who can create agents; per-agent credit limits; Enterprise can set workspace-wide limits
- **Tracking:** Credits dashboard — usage by agent, spend trends, status, recent activity; admins can disable runaway agents
- **Built-in protections:** Email/in-app alerts near credit limits; agents pause when credits run out; fast-spending new agents auto-pause; member requests require admin approval

### May 1, 2026 — Custom Agents in private Slack channels
- "Custom Agents can now read and reply in private Slack channels they're invited to."
- Enable via `Settings` → `Notion AI` → `AI connectors` → `Enable access to private content`

### April 27, 2026 — Rollups as currency, percent, more
- Number formatting in rollups (USD, EUR, percent, etc.)
- Decimal places — useful for budget totals and conversion rates in PM databases without formulas

### April 17, 2026 — Mail & Calendar in settings
- Dedicated settings tab to connect calendar and inbox
- Once linked, Notion AI can schedule meetings and draft emails

### April 16, 2026 — Opus 4.7
- Anthropic's Claude Opus 4.7 integrated
- "Uses fewer tokens, makes 3x fewer tool errors, and handles complex workflows more reliably."

> Note: page truncates around Apr 16, 2026. Earlier releases would require fetching page/2.

---

## 3. Notion 3.0 launch (Sep 18, 2025)

**Source:** [notion.com/blog/introducing-notion-3-0](https://www.notion.com/blog/introducing-notion-3-0) + [OpenAI customer story](https://openai.com/index/notion/) + TechCrunch / Datamation / Reworked

### TL;DR from the launch post
- "Notion 3.0 is here: The biggest evolution of Notion yet, with Notion AI Agents at the center."
- "Agents can do everything a human can do in Notion"
- Personal Agents with custom instructions
- Custom Agents (coming soon — later shipped Feb 2026)
- "Database row permissions, new AI connectors and additional MCP integrations"

### Autonomous agent capabilities
- "Your Agent can do up to 20 minutes of autonomous work at a time across hundreds of pages at once."
- "Create docs, build databases, search across tools, and execute multi-step workflows."

### Architectural rewrite
- Per OpenAI case study: "Instead of patching their existing stack, Notion rebuilt it. They replaced task-specific prompt chains with a central reasoning model that coordinates modular sub-agents."
- "These agents can search across Notion, Slack, or the web; add to or edit databases; and synthesize responses using whatever tools the task requires."
- "As models advanced — and users began asking agents to complete entire workflows — Notion's team saw limits in their system architecture. The old pattern of prompting models to do isolated tasks was limiting the ceiling of what was capable on their platform. Agents needed to make decisions, orchestrate tools, and reason through ambiguity, and that shift required more than prompt engineering."

### Multi-model access named
- "AI models evolve quickly. With Notion, you don't pay extra for every model. The latest—like Claude Sonnet 4 and GPT-5—are already built in."
- Models cited across sources: **GPT-5, Claude Opus 4.1, o3, o1-mini, Claude Sonnet 4, MiniMax M2.5, Haiku 4.5, GPT-5.4 Mini, GPT-5.4 Nano, Claude Opus 4.7**

### Example use case quoted
- "compile customer feedback from Slack, Notion, and email into actionable insights"
- Agent researches across tools → synthesizes findings → creates structured database → notifies when done

### Capabilities & integrations
- "A personal Agent can take on a whole project, like building a launch plan, breaking it into tasks, assigning them, and even drafting docs to give the team a head start."
- "With databases, it works at a scale no person could—updating or creating hundreds of pages at once."
- Pulls context from: **Slack, Google Drive, GitHub, Microsoft Teams, plus the web**, all within user permissions

### Quotes
- **Akshay Kothari, co-founder (Notion 3.0 announcement post):**
  - "Notion 1.0 introduced a collaborative canvas for your docs and knowledge"
  - "Notion 2.0 brought databases and integrations"
  - "Notion 3.0 — we taught Notion AI to use those building blocks so your Agent can finish real work."
  - "This isn't an AI chatbot that makes generic suggestions."
  - "Before, Notion AI was great for quick answers and editing a single page."
  - "Context, collaboration, and now action—all in one place."

### Notes
- Ivan Zhao is the CEO; he's NOT quoted in the launch post (it's by Akshay Kothari). Marketing-side quotes from Ivan Zhao not found in this research.
- Independent confirmation of the 20-min spec from Reworked and Datamation on Sep 19, 2025.

---

## 4. Notion AI Meeting Notes

### Launch
- May 13, 2025 (Notion 2.51)
- TechCrunch coverage: "Notion takes on AI notetakers like Granola with its own transcription feature"

### Capabilities
- Captures system audio + microphone input
- Works with **Zoom, Google Meet, Microsoft Teams, Slack Huddles, FaceTime, YouTube videos, phone calls** — "no bots or extra software required"
- Speaker labeling (desktop app)
- Live transcription during call
- Add typed notes while AI transcribes
- AI summary on meeting end — key points, decisions, action items
- "Summaries adapt to meeting type — 1:1s, team syncs, client calls, brainstorms"
- Agent automation: assign extracted tasks with owners/priority/due dates; update project statuses

### Slack integration
- Auto-share meeting notes in Slack
- Enterprise Search lets you ask NL questions across all meeting transcripts

### Recent updates
- **November 2026 (Notion 3.1):** Transcript-linked summaries — jump to source for any takeaway
- Notion AI now searches Google + Notion Calendars — prep for upcoming meetings

### Output lands in
- **Docs:** Private Docs receive transcripts, video, summaries
- **Tasks:** Action items become assigned tasks
- **Chat:** Aggregated answers from all meeting notes
- **Brain (AI):** Searchable via Notion AI

### Pricing
- **Business+ only ($20/user/mo)** — NOT on Plus plan
- Marked beta on /product/ai-meeting-notes
- Subject to fair-use limits
- HIPAA on Enterprise

### Limitations (from reviewer feedback)
- "No speaker identification" (contradicts official docs — inconsistent rollout?)
- "No auto-join, no video, no timestamps, very limited structure or automation"
- "Not a serious meeting assistant" for high-stakes client calls
- Multilingual quality: "If the AI misunderstands something, there's no notification or confidence score"
- Best for solo users + internal team meetings already in Notion

### Privacy
- GDPR, HIPAA, SOC 2, ISO 42001 (per /product/ai-meeting-notes page — Notion does claim ISO 42001 here, which is notable)
- "No third-party data training" + "Zero third-party data retention"

---

## 5. Notion MCP server

### Official remote server
- **URL:** `https://mcp.notion.com/mcp`
- **Auth:** **User-based OAuth (no bearer tokens)** — "A user must complete the OAuth flow to authorize access, which may not be suitable for fully automated workflows or cloud-based coding agents that run without human interaction."
- **Permission scope:** "MCP tools act with your full Notion permissions—they can access everything you can access."
- **Plan availability:** Personal connection broadly available. **Admin governance is Enterprise-only.**
- **April 2026 update:** MCP works with Meeting Notes + block comments; **91% more token-efficient** for creating/updating databases (Notion 3.5)

### Setup snippets

**Cursor:**
```json
{ "mcpServers": { "notion": { "url": "https://mcp.notion.com/mcp" } } }
```

**Claude Desktop / older stdio clients via bridge:**
```json
{ "mcpServers": { "notion": { "command": "npx", "args": ["-y", "mcp-remote", "https://mcp.notion.com/mcp"] } } }
```

**Local open-source server (Notion API token):**
```json
{ "mcpServers": { "notionApi": { "command": "npx", "args": ["-y", "@notionhq/notion-mcp-server"], "env": { "NOTION_TOKEN": "ntn_****" } } } }
```
> Note: Notion may sunset the local MCP server repo. Issues/PRs not actively monitored.

### Supported clients
| Client | Setup | Plan req |
|---|---|---|
| Claude Desktop / Claude.ai | Settings → Connectors | Pro / Max / Team / Enterprise |
| Cursor | .cursor/mcp.json | — |
| ChatGPT Pro | Settings → Connectors → Advanced | Plus/Pro |
| Claude Code | Plugin: github.com/makenotion/claude-code-notion-plugin (bundles MCP + Skills + slash commands) | — |
| Any MCP-compliant tool | Tool's MCP config | — |

### MCP Governance (Enterprise only)
- Settings → Connections → Permissions tab → AI apps → "Restrict AI apps members can connect to" → "Only from approved list"
- "Notion blocks every call from any AI app or MCP client that is not on the approved list, so it is functionally blocked"
- "If any external AI apps are already connected to the Notion MCP, they will automatically be added to the approved list"
- Adding non-listed tools: workspace owner/admin connects first; tool then appears as option
- **Bulk reset:** "Disconnect All Users" button forces re-authentication
- Audit log: name-change events recorded; connection URL persists across renames

### Security caveats (per Strac DLP analysis)
- "By itself, the Notion MCP server is not secure for regulated data without an additional DLP layer."
- "The Notion MCP server honors the authorizing user's permissions but returns whatever that user can see, including PII, PHI, credentials, source code, and other regulated content."
- For regulated use: pair MCP with MCP-layer DLP control that inspects and redacts every tool response

### Documentation
- developers.notion.com/guides/mcp/get-started-with-mcp
- notion.com/help/notion-mcp
- github.com/makenotion/notion-mcp-server (local)
- github.com/makenotion/claude-code-notion-plugin

### Tool inventory
- Not fully published; full set inferred from API docs
- Includes: pages CRUD, databases CRUD (new "data sources" abstraction in API 2025-09-03), search, blocks, users, comments, file upload
- Version 2.0.0 of local server migrated to Notion API 2025-09-03 — "data sources as the primary abstraction for databases"

---

## 6. Pricing + Notion Credits

### Plan tiers (2026)
| Plan | Price | AI access |
|---|---|---|
| Free | $0 | Limited trial only |
| Plus | $10/user/mo (annual, $12 monthly) | Limited trial only |
| Business | **$20/user/mo (annual, $24 monthly)** | Full AI suite + Custom Agents (credits required) |
| Enterprise | Custom | Full + SCIM + audit + unlimited history + advanced security |

### Notion Credits (Custom Agents only)
- **$10 per 1,000 credits**
- Effective: **May 4, 2026** (Custom Agents went paid; were free during beta from Feb 24, 2026)
- "Monthly Notion credits cost $10 per 1,000 credits, are billed alongside your subscription, and are flexible to adjust each month based on your needs."
- "They're shared across the workspace and reset monthly."
- **No rollover**

### What consumes credits
- Custom Agents (only credit-consuming surface)
- "How much the agent reads · how many actions it takes · how often it runs"
- "Reading longer pages, searching more content, or scanning larger databases generally uses more credits"
- Simple Custom Agent run: "a fraction of a credit"
- Long multi-step run: "dozens of credits in one go"

### What DOESN'T consume credits
- Notion Agent (in-editor assistant + chat)
- Standard AI writing tools
- Database autofill
- Notion AI search
- AI Meeting Notes (fair-use limits apply)

### Hard caps & runaway protection
- "Hard usage caps stop new AI actions when credits run out"
- "Existing automations keep running"
- Email + in-app alerts near credit limits
- Agents auto-pause when credits run out
- Fast-spending new agents auto-pause

### Plan-tier AI access
- **Custom Agents:** Business + Enterprise only (Free + Plus excluded)
- **All other Notion AI:** Business + Enterprise (Free + Plus is trial only)

### Notion Workers (Dev Platform 3.5)
- Free during beta
- Moves to Notion Credits billing **Aug 11, 2026**

### Efficiency wins (Apr 2026 — Notion 3.4)
- Custom Agents 35-50% cheaper to run
- New lightweight models: **GPT-5.4 Mini, GPT-5.4 Nano, Haiku 4.5, MiniMax M2.5**
- Per-run credit consumption reduced **up to 10×**

### Cost watch-out
- "One team recently discovered they had consumed 150,000 credits in a single month — the equivalent of $1,500 at the new rate."
- Mitigation: per-agent credit limits (admin-set)

### Managing credits
- Settings → Access & billing → Notion credits
- "Add Notion credits" → choose amount (hundreds → thousands)
- "If you're on a Business or Enterprise plan and you run out of Notion credits, you'll still be able to use other AI features (like AI Meeting Notes and Notion Agent) up to the fair use limit."

---

## 7. Notion vs Confluence

### Where Notion wins
- Block-based composability (most reviewers prefer Notion UX)
- AI bundled in Business+ (vs Rovo activation pain)
- "Verify any page" → AI citation honor (no Confluence equivalent)
- Multi-model gateway (GPT-5 / Claude / o3 toggle)
- AI Meeting Notes bundled
- Cleaner onboarding

### Where Confluence wins
- Native Jira ↔ Confluence two-way sync — "doc never stale vs ticket"
- Indefinite version history on Standard plan (Notion: 30/90 days unless Enterprise)
- Atlassian Intelligence reasons across Jira + Confluence in unified context
- 20+ pre-built Rovo documentation agents (Notion has smaller library)
- Bundled with Atlassian suite — cheaper for existing customers

### Pricing comparison (2026)
- **Standard:** Notion Plus $10 vs Confluence Standard $6.05
- **Premium/Business:** Notion Business $18-20 vs Confluence Premium $11.55

### Architecture quote
> "Notion is a relational database wrapped in a flexible block-editor, while Confluence is a hierarchical document management system built on a rigid page-tree structure. If you need extreme flexibility to build custom project trackers, CRM pipelines, and internal websites within a single tool, you choose Notion. If you need a scalable, standardized knowledge base that natively integrates with Jira and guarantees indefinite data retention for compliance, you choose Confluence."

---

## 8. Notion vs Jira

### Where Notion wins
- One tool, one mental model
- AI 3.0 Agents can work across docs + task databases in single run
- Custom Agents on triggers (cheaper than Jira automation rules at small scale)
- Multi-model AI
- Database row-level permissions
- Better UX for non-engineering teams

### Where Jira wins (Notion CAN'T match)
- Native agile frameworks (sprint velocity, burndown)
- Complex issue-type hierarchies (Epic → Story → Sub-task)
- Deep Git integration
- JSM ticketing (SLA, queues, customer portal)
- Rovo Dev for engineering intelligence
- DORA metrics
- Established enterprise governance posture

### Migration verdict (from multi-source synthesis)
- "No. While Notion has excellent Kanban boards and timeline views for lightweight project management, it lacks native agile frameworks (like sprint velocity charts, deep Git integrations, and complex issue-type hierarchies). Software teams should use Jira for execution and Confluence (or Notion) for documentation."
- "Jira integration is weak. Notion doesn't natively connect to Jira. You can use Zapier to sync tickets or comments, but this isn't bidirectional or real-time."

### User sentiment (mixed)
- Positive: "Notion is great. It combines the project management features of Confluence and Jira in one environment."
- Critical: "Because Notion tries to be everything, it's a little bit of everything but it's still worse than any of its individual competitors (e.g. Trello/Jira is better for board use than Notion)."

### Decision matrix
| Team | Recommendation |
|---|---|
| Startup / SMB < 50 | Notion replaces both |
| SMB 50-150, mostly non-eng | Notion replaces both |
| Eng-heavy 50-200 | Hybrid: Notion wiki + Jira/Linear tickets, unified via Enterprise Search |
| Eng-heavy 200+ | Stay on Jira + Confluence |
| Regulated industry | Stay on Atlassian (or Notion Enterprise with care) |

---

## 9. Developer Platform 3.5 (May 13, 2026)

### Eight components shipped same day

1. **External Agents API (Alpha)** — Bring 3rd-party agents (Claude, Codex, Decagon, custom-built) into Notion as orchestration layer
2. **Database Sync (Beta)** — Pull data from any API source into Notion DBs via Workers
3. **Custom Agent Tools (Beta)** — Deterministic code-based tools, "fraction of token cost" vs prompting
4. **Webhook triggers (Beta)** — Any app can trigger Notion workflows
5. **Notion Workers (Beta)** — Hosted runtime sandbox; free during beta → credits Aug 11, 2026
6. **Notion CLI (GA)** — Command-line tool for devs AND coding agents
7. **Agent SDK (Alpha waitlist)** — Embed Notion Agents inside other apps (CRM, MS Teams, Discord, Amplitude, Hex)
8. **Connections tab (GA)** — Unified mgmt for connections, PATs, internal API connections

### Other 3.5 additions
- **Agents "Hall of Fame":** Templates from Ramp, Clay, Vercel
- **Markdown API**
- **MCP updates:** works with Meeting Notes + block comments; 91% more token-efficient for create/update DBs
- **Workspace-scoped OAuth and PATs** — any member can build connections
- **Developer Portal & rebuilt Docs** with built-in AI assistant

### Strategic positioning
- Notion explicitly building substrate for external agents — Linear-style "orchestration layer for the agent era"
- External Agents API = the bet that Notion becomes the standard environment for AI agents working on knowledge

---

## 10. Community sentiment

### Bullish
- AI 3.0 Agents "genuinely impressive for knowledge-heavy work"
- AI Meeting Notes: "feels like a native part of your workspace"
- Multi-model: "the reason I stayed"
- "Verify any page" widely praised by Confluence migrants
- 1M+ Custom Agents created in 2 months of beta

### Critical
- "Notion AI is incredible for docs; useless for tracking sprint velocity"
- Pricing friction since May 2025 — AI moved from Plus to Business plan
- Custom Agents credit costs surprise users ($1,500 in one month for one team)
- AI Meeting Notes not yet a "serious meeting assistant" — better-suited to internal team syncs than client-facing calls
- Multilingual quality issues

### Real-world quotes
- "Notion is great. It combines the project management features of Confluence and Jira in one environment. It's great for documenting how things work, how stuff was done, etc."
- "Because Notion tries to be everything, it's a little bit of everything but it's still worse than any of its individual competitors (e.g. Trello/Jira is better for board use than Notion)."

### Adoption stats
- Featured in OpenAI's GPT-5 customer story
- TechCrunch / The Verge / Datamation coverage at 3.0 launch
- 1M+ Custom Agents created since Feb 2026 beta
- Reference customers for agent templates: Ramp, Clay, Vercel

---

## 11. Open questions / gaps

1. **Pre-Apr 2026 release history** — releases page truncates at Apr 16, 2026 (paginated). Older releases would need page/2.
2. **Ivan Zhao quotes** — I couldn't find direct Ivan Zhao quotes from the 3.0 launch. Akshay Kothari (co-founder) is the on-record voice.
3. **Full MCP tool inventory** — Notion doesn't publish a complete tool list in marketing docs. Would need a live MCP client connection.
4. **Custom Agent rate per task** — only directional claims ("fraction of credit" to "dozens of credits"). No per-action rate card.
5. **ISO 42001 certification scope** — claimed on /product/ai-meeting-notes but not on the broader trust pages I fetched. Worth verifying full certification status.
6. **Agent SDK launch timing** — alpha waitlist; no firm GA date.
7. **Notion vs Linear Agent SDK comparison** — both shipped agent platforms in 2025-2026. How do the developer experiences compare in practice?
8. **Jira/Linear connector depth in Enterprise Search** — can the agent act on Jira/Linear data or only read? Need to verify in a live test.
9. **Q4 2025 / Q1 2026 revenue / adoption figures** — Notion is private; no public earnings to mine.
10. **Roadmap signals from Ivan Zhao directly** — would be high-value for the strategic vector section.

---

## 12. Recommended screenshots

If you can capture from a live Notion workspace:

1. **Notion Agent chat panel** with model picker visible
2. **Plan Mode** — agent showing clarifying questions before action
3. **Custom Agent Builder** screen (Library → Agents → Create)
4. **Custom Agent Directory** (Library → Agents)
5. **AI Meeting Notes** during a live capture
6. **AI Meeting Notes output** — Doc with transcript + summary + action items
7. **Enterprise Search** result spanning Notion + Slack + Drive + Jira
8. **"Verify any page"** badge + AI citation showing verified-source ranking
9. **Database Autofill** in action — agent filling status/priority/owner
10. **NL → Formula** conversion in a database
11. **AI Credits dashboard** — usage by agent, spend trends
12. **MCP Governance settings** (Enterprise) — approved AI apps list
13. **Notion MCP installed in Cursor** showing the tools list
14. **Notion Workers** runtime sandbox + code execution
15. **External Agents API** — Claude/Codex configured as Notion agent
16. **Notion CLI** in a terminal session
17. **Connections tab** — workspace + personal connections + PATs

---

*Last updated: 2026-05-15 — companion to `notion_ai_research.html`.*
