# Plane AI — Raw Research Notes

> Working notes collected for [plane_ai_research.html](plane_ai_research.html). Verbatim extracts from each source.
>
> **Run date:** 2026-05-15
> **Method:** WebFetch + WebSearch. No Plane MCP / playwright access in this session.

---

## Table of contents

1. [plane.so homepage — positioning](#1-planeso-homepage)
2. [plane.so/ai — Plane AI features](#2-planesoai)
3. [plane.so/changelog — release log](#3-planesochangelog)
4. [GitHub releases (OSS)](#4-github-releases-oss)
5. [Plane MCP server](#5-plane-mcp-server)
6. [Leadership + funding](#6-leadership--funding)
7. [Open questions / gaps](#7-open-questions--gaps)
8. [Recommended screenshots](#8-recommended-screenshots)

---

## 1. plane.so homepage

### Tagline + positioning
- "Project management and knowledge management for teams and agents"
- "Brings projects, docs, and AI-powered workflows into one unified workspace so teams and agents can plan, execute, and stay aligned."
- "Cloud, self-hosted and air-gapped ready."

### Migration claims (verbatim)
- "Two Fortune 10 companies chose Plane for their Jira migration."
- "Get out of Jira, Linear, ClickUp, Asana, or Monday without leaving your data behind."
- Dedicated comparison pages for Jira, Asana, Monday.com, Linear

### Customer stories
- **FortyAU** — replaced Monday + Trello
- **MinimalArt** — replaced ClickUp
- **VATES** — replaced "a Trello alternative"

### Migration program
- 3-week structured migration: discovery → parallel run → cutover

### Product surface — "Four products in one workspace"
1. **Projects** — "Project management that matches how your team works"
2. **Wiki** — "Documentation built in for tribal knowledge"
3. **Plane AI** — "AI that knows your work, not just your prompts"
4. **Desk** — Customer support (marked **Coming soon**) — "Customer support that lives where your work does"

### AI positioning
- "AI that works because it knows your context"
- "Plane was not retrofitted for AI, it was built around it."
- Three AI pillars:
  1. "Answers from across your workspace" (status/blockers/doc changes)
  2. "Agents that do the work for you" (triage/assign/track/ship)
  3. "Works where your team already talks" (Slack + MS Teams)

### Self-hosted positioning (verbatim)
- "Self-host without compromise, on-prem and air-gapped"
- "The only modern project management platform built for environments where you control every layer."

### Self-hosted tooling
- **Prime CLI** — install, configure, upgrade, backup, monitor
- **Docker and Kubernetes** with Helm charts
- BYO Postgres, Redis, S3-compatible storage
- **God Mode** admin panel — SMTP, auth, SSO, security, telemetry

### Plane Compose — Projects-as-Code
- YAML definitions versioned in Git
- Deployed from terminal
- "Every setting versioned, reviewed, and deployed from your terminal."

### Pricing tiers (referenced)
- **Pro**
- **Business** (CTA: "Try Plane Business for 14 days")
- **Enterprise**
- (Free tier also exists)
- `/pricing` page linked but not detailed in fetched content

### Core PM capabilities
- Views: "Board, Spreadsheet, List, Gantt"
- Cycles/sprints with burndown
- Initiatives and epics with rollup
- Workflows and approvals (no plugins required)
- Real-time dashboards
- Mobile apps (iOS, Android), Mac/Windows desktop

### Compliance & Enterprise
- SOC 2, ISO 27001, GDPR, CCPA "out of the box"
- SSO, SAML, LDAP
- Committed uptime SLA
- Public security portal: security.plane.so

### Customer logos
- Sony, Aramco, Dolby, Accenture, Amazon, Zerodha, Stark Bank, Mirador Therapeutics, Government of Lithuania, République Française

### Key marketing quotes
- "AI that knows your work, not just your prompts"
- "Four products in one workspace for your whole org"
- "Plane was not retrofitted for AI, it was built around it."
- "AI that works because it knows your context"
- "Self-host without compromise, on-prem and air-gapped"
- "Every setting versioned, reviewed, and deployed from your terminal."
- "Next-gen project management starts here"
- "Flexible features for every project, and all teams"
- "Enterprise-grade security, compliance, and control"

---

## 2. plane.so/ai

### Brand & positioning
- Product called **"Plane AI"** (no "Pi" abbreviation)
- Tagline: "The operating layer for agents and teams"
- Hero: "The workspace where agents and teams come to work"
- Frame: "THE AI WORK PLATFORM"
- Thesis: "The age of AI does not need more agents. It needs a place for agents to work."
- Differentiator: "most tools bolted AI on, while Plane was designed around it"

### Three headline capabilities
1. **Talk to build** — generates project structure, work items, and cycles from a prompt
2. **Ask to know** — natural-language queries against live workspace data
3. **Assign to ship** — @mention an agent on a work item to triage and progress it

### Automation features
- Duplicate detection against backlog before creation
- One-click summaries for cycles, projects, and initiatives
- AI-drafted briefs auto-attached as Pages
- Auto-triage: classify, label, assign, route
- In-editor block actions: summarize, rewrite, expand, translate

### Agent surfaces
- Agents as assignees on work items
- @mentions in comments, docs, threads
- Agent Development Kit + open-source MCP server
- Ship to Marketplace or keep internal

### Integrations
- Connectors: Slack, GitHub, GitLab, Sentry, others
- Open-source MCP server compatible with Claude, Cursor, others

### Self-hosted / infra
- Full parity between Cloud and self-hosted
- **BYO keys (OpenAI OR Anthropic)**
- Air-gapped option
- "No prompt storage, no training on customer data"

### Trust & compliance
- SOC 2, ISO 27001, GDPR, CCPA
- "99.99% API uptime. 100% on AI and Agents"
- SSO, SAML, LDAP, RBAC, audit logs

### Pricing
- "Ships on every plan" — included across tiers
- Credit-based consumption model, no per-seat AI fee
- Self-hosted customers pay their AI provider directly
- Plan pages referenced: Pro, Business, Enterprise

### Status
- Page does not label features GA/beta explicitly
- Everything presented as available ("what Plane AI can do today")

---

## 3. plane.so/changelog

### April 25, 2026 — Custom roles, granular access control, redesigned permissions
- "Custom roles for Enterprise" in redesigned permissions model
- (Borderline AI — included for completeness)

### March 16, 2026 — AI charts, column layouts, project labels
- "Explore data with interactive AI charts"
- Multi-column Pages
- Reusable Project labels

### February 28, 2026 — Archive epics, rich Initiative filters
- "Custom OAuth scopes for finer control over third-party app access" (relevant to integration/automation control)

### February 17, 2026 — Web search in Plane AI, Project Subscribers
- "Web search in Plane AI for real-time external context"
- Project Subscribers for automatic notifications
- New Workspace view layouts

### February 2, 2026 — Product tour, Try section, Plane AI updates
- Guided onboarding
- "Improvements to pages, forms, AI, and app performance"

### January 15, 2026 — Re-routing project updates to Slack + bulk imports
- "Tightens control over how work flows between Plane and Slack"
- "Smarter, context-aware AI interactions"
- Security hardening across auth, uploads, integrations

### December 23, 2025 — Intake ownership, AI context awareness, editor-to-work conversion
- "Plane AI that understands cycles, modules, and work items with Ask and Build modes"
- Editor upgrades: convert text → work items
- Embed linked document context

### November 15, 2025 — Plane AI with Slack support + Claude Sonnet 4.0 + React Router migration
- Plane AI gains Slack support
- "Runs on Claude Sonnet 4.0, and can turn answers into editable Pages"
- Web app migrated to React Router and Vite

> Note: No entries on this page reference **MCP, Pi, semantic search, agents** by those specific terms. Older entries (page 2+) may have more.

---

## 4. GitHub releases (OSS)

### v1.3.1 — May 14, 2026
- Improvements: scrollbar in keyboard shortcuts modal · skip role/use-case steps for self-hosted instances
- Security: ORM field injection prevention · workspace membership enforcement on V2 asset endpoints · filename sanitization against path traversal · webhook SSRF protection via `WEBHOOK_ALLOWED_IPS` allowlist
- **Intercom integration removed entirely**
- Dependency bumps (Django, axios, vite)
- No AI/agent/MCP/Slack features mentioned

### v1.3.0 — Apr 6, 2026
- "A cleaner, calmer Plane" visual/design refresh
- **Gitea Authentication support** added
- Project Summary external API, mention search debounce, timezone selection
- Ukrainian language support, expanded Russian, webhook translations
- No AI/agent/MCP/Slack features mentioned

### v1.2.3 — Mar 5, 2026
- Security only: webhook validation against reserved IPs

### v1.2.2 — Feb 23, 2026
- Security patch: API token rate limit validation, SSRF mitigation, member info disclosure fix, IDOR fixes
- Django 4.2.28, cryptography 46.0.5

### v1.2.1 — Dec 12, 2025
- Security: removed underlying Next.js dependencies

### v1.2.0 — Dec 11, 2025
- **Major migration: Next.js → React Router + Vite**
- New top navigation bar
- Global Search and Inbox
- "Power K, supercharged" — keyboard-driven command palette
- Triage state for Intake
- Magic code now 6-digit numeric
- Security: Next.js CVE-2025-66478, React CVE-2025-55182, Django 4.2.27

### v1.1.0 — Oct 23, 2025
- Richer filters across work items, epics, custom views
- MIME type detection for document uploads

### v1.0.0 — Sep 10, 2025
- GA release with new branding
- Turkish language support
- Email notifications enabled by default
- yarn → pnpm migration

### v0.28.0 — Jul 30, 2025
- Copy comment URLs
- Collapsible sidebar
- Emoji support via /emoji
- Page navigation pane (TOC, version history)
- Node 22, Python 3.12.10

### Observation
**Critical insight: AI/agent/MCP/Slack features are NOT shipped in the open-source releases.** The OSS releases focus on security, OSS-stack housekeeping (React Router migration), and i18n. AI features ship in the cloud product. This is the standard open-core pattern — OSS for the PM core, proprietary cloud for AI.

---

## 5. Plane MCP server

### Open source
- **GitHub:** github.com/makeplane/plane-mcp-server
- Available via npm + uvx

### Endpoints
- **Remote OAuth:** `https://mcp.plane.so/http/mcp`
- **Remote PAT (API key):** `https://mcp.plane.so/http/api-key/mcp`
- **Legacy SSE:** `https://mcp.plane.so/sse`
- **Self-hosted Stdio:** `uvx plane-mcp-server stdio`

### Authentication methods
1. **OAuth (browser)** — recommended for Plane Cloud
2. **PAT token in headers** — for CI/CD, automated workflows
3. **Stdio with env vars** — for self-hosted instances

### Self-hosted Stdio env vars
| Variable | Required | Purpose |
|---|---|---|
| `PLANE_API_KEY` | Yes | API key |
| `PLANE_WORKSPACE_SLUG` | Yes | Workspace slug |
| `PLANE_BASE_URL` | No | Defaults to `https://api.plane.so` |

### Prerequisites
- Remote: Node.js 22+ and npx
- Local Stdio: Python 3.10+ and uvx
- WSL users on Windows: prefix commands with `wsl`

### Tool count
**55+ tools** across multiple categories (per third-party Codersera review).

Categories include:
- Projects (list, create, manage)
- Work items (CRUD, search, comment, link)
- Cycles (list, create)
- Modules (list)
- Members (list, manage)
- States (manage)
- Labels (manage)
- Pages (create, update)
- Intake (list intake items)
- Views (project, workspace)
- Webhooks
- Workspace info

### Setup snippets

**Claude Desktop / Cursor / VSCode (OAuth):**
```json
{
  "mcpServers": {
    "plane": {
      "command": "npx",
      "args": ["mcp-remote@latest", "https://mcp.plane.so/http/mcp"]
    }
  }
}
```

**PAT token (CI/CD):**
```json
{
  "mcpServers": {
    "plane": {
      "command": "npx",
      "args": ["mcp-remote@latest", "https://mcp.plane.so/http/api-key/mcp"],
      "headers": {
        "Authorization": "Bearer <YOUR_API_KEY>",
        "X-Workspace-slug": "<YOUR_WORKSPACE_SLUG>"
      }
    }
  }
}
```

**Local Stdio (self-hosted):**
```json
{
  "mcpServers": {
    "plane": {
      "command": "uvx",
      "args": ["plane-mcp-server", "stdio"],
      "env": {
        "PLANE_API_KEY": "<YOUR_API_KEY>",
        "PLANE_WORKSPACE_SLUG": "<YOUR_WORKSPACE_SLUG>",
        "PLANE_BASE_URL": "https://your-plane-instance.com/api"
      }
    }
  }
}
```

**Windsurf (note `-y` flag):**
```json
{
  "mcpServers": {
    "plane": {
      "command": "npx",
      "args": ["-y", "mcp-remote@latest", "https://mcp.plane.so/http/mcp"]
    }
  }
}
```

**Zed (uses `context_servers`):**
```json
{
  "context_servers": {
    "plane": {
      "source": "custom",
      "command": "npx",
      "args": ["-y", "mcp-remote@latest", "https://mcp.plane.so/http/mcp"],
      "env": {}
    }
  }
}
```

### Supported AI clients (officially listed)
- Claude.ai (web/desktop, via Settings → Integrations → Add more)
- Claude Desktop
- Claude Code (via `claude mcp add-json`)
- Cursor
- VSCode (via `.vscode/mcp.json`)
- Windsurf (via Cascade → MCP servers)
- Zed

### Plane Web/Desktop app integration
- Open Settings → sidebar (web or desktop)
- Scroll to Integrations → Add more
- Enter Integration URL: `https://mcp.plane.so/http/mcp`
- Click Connect → OAuth flow

### Tool ceiling warning (per 2026 ecosystem context)
- "Cursor has a soft ceiling of roughly 40 active tools across all your MCP servers combined"
- Plane exposes 55+ tools — may need to scope which are active per project
- Even Claude Code: "past about 50 visible tools the model starts picking the wrong one"

### Example workflows
- "List all projects in my workspace" → `list_projects`
- "Create a bug in project WEB titled 'Fix login redirect loop' and assign it to me" → `get_me` then `create_work_item`
- "Search for work items related to 'authentication' across the workspace" → `search_work_items`

### Community alternative
- `kelvin6365/plane-mcp-server` exists as a community option
- Valid client options: claude, cline, windsurf, roo-cline, witsy, enconvo, cursor

### Documentation
- developers.plane.so/dev-tools/mcp-server
- developers.plane.so/dev-tools/mcp-server-claude-code
- Open source: github.com/makeplane/plane-mcp-server

### Troubleshooting
- For OAuth issues: `rm -rf ~/.mcp-auth` to clear cached tokens

---

## 6. Leadership + funding

### Founders
- **Vamsi Kurama** — Co-founder & CEO
- **Vihar Kurama** — Co-founder & COO

### Background (Vamsi Kurama)
- Before Plane: co-founded **Caravel** (AI + scale engineering consulting)
- Helped "dozens of startups and enterprises build and scale their tech businesses to millions of users"
- Also CTO of Soulpage IT Solutions

### Funding
- **Total: $4M (single round)**
- **Seed:** OSS Capital, closed April 24, 2024
- Investor type: OSS-specialist VC firm
- No public Series A as of May 2026

### Company facts (Tracxn, March 2026)
- **Founded: 2022**
- **HQ: Hyderabad, India**
- **92 employees** (Mar 2026)
- **Annual revenue: ₹17.4Cr (~$2M)** as of March 31, 2025
- Ranked 28th among 1,960 active competitors
- 11th in funding among competitors

### Adoption (per Kurama posts, Jan 2026)
- Users from **293 cities** across **107 countries** in January 2026 alone

### Vamsi Kurama on the funding round
> "This investment from OSS Capital is not just a financial boost but a strategic one, allowing us to accelerate our growth and innovate further."

### Vamsi Kurama on AI strategy (2026 vision)
> "Everyone in productivity and project management is talking about consolidation right now — bringing features together and calling it 'All-in-one.' Consolidation without connection doesn't work."

> "Organizations don't just need consolidated tools. They need steerable systems — a steerable system is one where humans and agents operate inside the same loop, where a change in intent propagates through workflows, decisions, and outcomes without friction."

> "This happens a thousand times a week inside every enterprise. Not in the boardroom but below it. The strategic calls are made once a quarter. The decisions that actually move the business get made every hour, by managers doing their best with whatever data they can grab in time. Most of the time, they're flying on instinct and hoping the dashboard catches up."

### Vamsi Kurama on OSS
> "The number one advantage of being open source is privacy and security. That our software can be hosted by our customers on their own infrastructure, with all the protections from the public internet, is a key driver for Plane's adoption."

---

## 7. Open questions / gaps

1. **Specific AI Credit rates on Plane Cloud** — not surfaced on /ai or /pricing in fetched content. Compare with monday's $0.01 and Notion's $10/1000.
2. **Agent Marketplace size** — referenced but no public count (vs monday's Agentalent 17-at-launch).
3. **Plane Compose technical depth** — referenced but no public YAML schema docs surfaced. May be alpha/beta.
4. **Agent Run lifecycle details** — mentioned on /ai but no developer docs explaining states/states diagram.
5. **Plane Desk launch date** — "Coming soon" but no firm target.
6. **MS Teams AI intake launch date** — "Coming soon" on /ai.
7. **Self-hosted Plane AI feature parity verification** — full parity claimed; would want to verify by trying both surfaces.
8. **Series A funding signals** — last round was Apr 2024 ($4M seed). Growth (92 employees, Fortune 10 wins) suggests next round is overdue. No public signal yet.
9. **Anthropic vs OpenAI default on cloud** — Nov 2025 changelog confirms Claude Sonnet 4.0 default. Has this changed since?
10. **The specific 55+ MCP tool list** — third-party reviews cite 55+ but I couldn't find a complete enumeration. Best captured from a live MCP client connection.
11. **Plane's response to credit-pricing model competitors** — monday's $0.01 credit + ClickUp's add-on tiers have created friction; how does Plane differentiate beyond BYO-keys?
12. **The full Slack AI intake feature set** — described as "AGI-like" but specific capabilities not enumerated.

---

## 8. Recommended screenshots

If you can capture from a live Plane workspace:

1. **Plane AI panel** — Ask mode answering a workspace question
2. **Plane AI panel** — Build mode generating project structure
3. **Agent assigned to a work item** — Assign mode in action
4. **Plane Compose YAML** — example project-as-code definition
5. **Prime CLI** running an install or upgrade command
6. **God Mode admin panel** showing AI provider key configuration
7. **Slack @Plane** creating a work item from a thread
8. **MCP integration** in Plane Settings → Integrations → Add more
9. **Plane MCP installed in Cursor** showing the 55+ tools list
10. **AI charts** on a dashboard (Mar 16, 2026)
11. **Editor block actions** — summarize/rewrite/expand/translate inline
12. **Custom OAuth scopes** configuration (Feb 28, 2026)
13. **Webhook security** settings (`WEBHOOK_ALLOWED_IPS` allowlist)
14. **Agent Development Kit** docs/example
15. **Air-gapped deployment** architecture diagram
16. **AI provider key BYO** configuration on self-hosted

---

*Last updated: 2026-05-15 — companion to `plane_ai_research.html`.*
