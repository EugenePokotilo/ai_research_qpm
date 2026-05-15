# monday.com AI — Raw Research Notes

> Working notes collected for [monday_ai_research.html](monday_ai_research.html). Verbatim extracts from each source so you can dig deeper, verify quotes, or build follow-up docs without re-fetching.
>
> **Run date:** 2026-05-15
> **Method:** WebFetch + WebSearch. No monday MCP / playwright access in this session.

---

## Table of contents

1. [monday.com/w/ai — current AI feature inventory](#1-mondaycomwai)
2. [monday.com/whats-new — historical updates](#2-mondaycomwhats-new)
3. [Developer changelogs (apps + API)](#3-developer-changelogs)
4. [monday MCP](#4-monday-mcp)
5. ["All In on AI" IR press release (May 6, 2026)](#5-all-in-on-ai-may-6-2026)
6. [Agentalent.ai launch (Mar 23, 2026)](#6-agentalentai-mar-23-2026)
7. [Q4 2025 earnings call metrics](#7-q4-2025-earnings)
8. [AI Credits pricing model](#8-ai-credits-pricing)
9. [Brand evolution map](#9-brand-evolution)
10. [Community sentiment](#10-community-sentiment)
11. [Open questions / gaps](#11-open-questions--gaps)
12. [Recommended screenshots](#12-recommended-screenshots)

---

## 1. monday.com/w/ai

### Brand strategy on the page
- Headline: **"Outpace everyone with the best AI work platform"**
- Sub: **"Exponential execution that scales your business impact and expands what your teams can deliver."**
- **"Get more work done with AI that's woven into your work"**
- **"Trusted by over 60% of the Fortune 500"**
- Recognition: **"Only work management platform to be recognized as a Leader in 3 Gartner® Magic Quadrant™ reports."**

### Current AI products

**1. monday sidekick**
- "Built-in personal AI assistant"
- "Context-aware AI assistant who thinks, recommends, and runs work for you at scale"
- Capabilities: creating boards · brainstorming · analyzing data · generating images · online research · writing docs · crafting ad copy · generating brand assets · summarizing ticket history · monitoring SLAs · building roadmaps
- Surface: Embedded throughout (sidebar/in-product)
- Status: GA

**2. monday vibe**
- "Build any business software in minutes" — "Reduce costs and clutter by replacing disconnected tools with custom apps"
- Examples: Presentation · Inventory app · Documentation page · Recruiting app · Time tracker · Event portal
- Surface: App builder interface with file upload
- Status: GA

**3. monday agents**
- "Unlimited workforce that amplifies your team's impact" — ready-made or custom
- Status: **Early Access** (request via form)
- Agent categories & examples:
  - **Operations**: Customer Support Agent, SLA Monitor Agent, Vendor Researcher, Process Automator
  - **Project**: Risk Analyzer, Task Coordinator, Meeting Scheduler, Follow-up Agent, PMO Agent
  - **Marketing**: RSVP Manager, Market Landscape Analyzer, Competitor Research Agent, Translator Agent, Asset Generator
  - **Sales (CRM expert)**: Lead Agent, Contact Duplicates Finder, Sales Agent, Meeting Summarizer
  - **Engineering**: Bug Prioritization Agent, Bug Reporter, Release Notes Agent, Coding Agent, PRD Agent, Sentiment Detector, Code Reviewer, Incident Resolver
- Custom agent components: **Knowledge · Integrations · Actions · 24/7 Autonomy · Guardrails**

**4. monday workflows (Agentic Workflows)**
- "Visually build, automate, and manage complex cross-functional processes with AI"
- Positioning: "Autonomous workflows that run work end to end"

**5. monday MCP**
- Listed under AI Resources

### AI-First Foundation Components
- **Open ecosystem**: APIs, "200+ integrations, and MCP"
- **Unified data**: Cross-department shared data layer
- **Infinite knowledge**: "AI learns from documents, workflows, historical data"
- **Any AI model**: Connects to "Claude, GPT, and Gemini"

### Surfaces table
| Surface | AI Feature |
|---|---|
| Sidebar/assistant | monday sidekick |
| Board / project views | Sidekick suggestions, agents (PMO, Risk Analyzer) |
| CRM | Sales agents, Meeting Summarizer, Lead Agent |
| Service/IT | SLA Monitor, Incident Resolver |
| Dev | Coding Agent, Bug Reporter, PRD Agent |
| Automation/workflow builder | Agentic workflows |
| App builder | monday vibe |

### Data, Privacy & Trust
- Dedicated **AI Trust Center** linked in nav
- Compliance: **GDPR, SOC 2 (AICPA), ISO, HIPAA**
- "Enterprise-grade AI infrastructure with built-in protection and security, data privacy, governance, permissions, and compliance"
- Guardrails: "Stay in control with guardrails and full transparency into every action"
- Agent autonomy: "AI agents act without time, volume, or language constraints"

### Brand names NOT found on /w/ai
The following from the old 2024 deck were **not mentioned** on the current page:
- monday AI (generic — superseded)
- monday magic (still in changelog history)
- Sidekick Skills (still in changelog, but not on /w/ai)
- Digital Workers / Digital Workforce (replaced by "monday agents")
- AI Blocks (still ships — just no longer the headline brand)
- AI Service Agent (now an Operations Agent category)
- SDR Expert (subsumed under Sales agents)
- Agent Marketplace (now branded "Agentalent.ai")

### Pricing on /w/ai
- No AI credits model disclosed on this page
- "No credit card needed ✦ Unlimited time on Free plan"
- Pricing CTA links to `/pricing`

---

## 2. monday.com/whats-new

> Note: page is partly JS-rendered with pagination ("1 / 8 Next"). Below is what was extractable.

### May 2025
- **May 12** — Reach all portal users with Portal Announcements (monday service): Post banners at top of portal
- **May 7** — Auto sync ticket requester info from Active Directory (monday service)
- **May 6** — Clean up unused labels in managed columns (platform)

### April 2025
- **Apr 27** — See full picture with List View unmapped columns
- **Apr 7** — Workspace exclusions for data retention

### March 2025
- **Mar 30** — **Control AI spend with AI governance with user limits**: "Set per-user AI credit limits in the admin panel to control budgets, monitor usage with threshold warnings."
- **Mar 30** — **Sidekick Skills Marketplace**: "Discover and activate AI-powered skills from the Sidekick Skills Marketplace to act across your entire tech stack."
- **Mar 30** — **monday vibe board expansion**: "Connect additional boards to live vibe apps without rebuilding."
- **Mar 26** — Scheduled cleaning activity log: Audit trail for archived/deleted boards
- **Mar 25** — Microsoft Teams user messaging
- **Mar 22** — **Create professional marketing images with monday sidekick**: "Generate high-quality marketing images using monday sidekick."
- **Mar 15** — **WorkCanvas native visual canvas**: "AI-powered collaborative canvas that syncs live with your boards."

### December 2024
- **Dec 23** — Batch dependencies (work management)

### November 2024
- **Nov 6** — **Autopilot Hub**: "Get full visibility into everything that's automated in your organization with the new Autopilot Hub."

### October 2024
- **Oct 22** — **monday VSCode extension**: Gives "AI richer context to deliver more accurate, relevant code suggestions."
- **Oct 8** — WorkCanvas Data Layers

### July 2024
- **Jul 28** — **AI portfolio report** (work management): "Create executive-level reports with key insights into portfolio progress and risks at the click of a button."
- **Jul 8** — **monday magic**: "Describe your workflow in a prompt and get a ready-to-use monday.com solution — no setup, no developers."

### June 2024
- **Jun 23** — **AI board previews**: "Use AI-powered board preview to see board content at a glance."
- **Jun 19** — **Auto-resolve tickets with AI** (service): "AI copilot responds to routine requests; You control when AI replies - just choose the confidence level it must reach."
- Other automation block items: Move item to board · Find connected subitem · Update subitem action · Trigger workflows with Salesforce objects · Update Item & Subitem blocks · File automation · Convert Text to Number/Date blocks

### May 2024
- **May 25** — **Gain control over AI usage**: "Admins can track usage levels and restrict features by team to support security and governance."
- **May 20** — **AI suggestions for daily standups** (dev): "AI-driven task summaries and next-step recommendations."
- **May 20** — Managed Column
- **May 19** — **Clarity of AI results in each cell**: Feedback on AI outputs to refine prompts
- **May 15** — **Prompt preview of AI Blocks**: Easier access to AI prompts when setting up AI columns
- **May 14** — **AI Hub**: "Your one-stop solution for discovering AI features on monday.com" with personalized recommendations
- **May 13** — **Track AI Credits usage**: View who created automations and analyze workflows with historic data
- **May 8** — Scheduled Updates

### Featured/Announcement (undated highlights on page)
- **Connect AI agents and apps to monday.com (MCP)**: "Seamlessly connect AI agents and apps to your account."
- **AI Blocks are now open to everyone**: "Easily add AI to your workflows with ready-made AI actions."
- **monday service out of beta**: "Empower any team to deliver efficient service at scale with powerful AI capabilities."

---

## 3. Developer changelogs

### Apps changelog (developer.monday.com/apps/changelog) — page 1 of 18

**Feb 25, 2026 — New feature-level lifecycle event subscriptions**
- Granular control over "which events your app listens to, where they're delivered, and whether each event is handled synchronously or asynchronously"
- Managed via dedicated GraphQL API

**Jan 26, 2026 — Automation Infrastructure Migration (Deprecated)**
- "monday is consolidating all automation feature creation into a single workflows-based infrastructure powering the new automation builder, monday workflows, and monday sidekick."
- Apps using legacy "Integration for sentence builder" feature must migrate by **April 30, 2026**
- Existing automations keep running; self-service migration wizard provided

**Jan 16, 2026 — Build skills for monday sidekick**
- Developers can build **Sidekick skill app features**
- "Define custom actions triggered by natural-language requests in monday sidekick"
- Users invoke app actions conversationally "without navigating menus, configuring automations, or switching tools"

### API changelog (developer.monday.com/api-reference/changelog)

**April 2, 2026 — Four AI-flavored queries shipped same day:**

1. **`notetaker_meetings`** — "paginated meetings with completed recordings that the current user can view, including summaries, topics, action items, transcripts, and participants." Filter by IDs, search text, or access level: `OWN`, `SHARED_WITH_ME`, `SHARED_WITH_ACCOUNT`, `ALL`.

2. **`knowledge_base_search`** — "an AI-powered search across knowledge base snippets and returns an LLM-generated answer along with the raw source snippets."

3. **`ask_developer_docs`** — "returns an AI-generated answer based on the apps documentation, along with a `conversation_id` you can use for follow-up queries."

4. **`BlockEvent` automation loop fields** — new fields:
   - `iterator_id` (ID) — "The iterator identifier if the block is part of a loop"
   - `current_iteration` (Int) — "The current iteration number within the loop"
   - `max_iterations` (Int) — "The total configured iterations for the loop"

**Apr 19, 2026 — UserKindFilter enum**
- Added `AI_PLATFORM_AGENT_API_USER` kind — referenced but entry itself not about AI features

---

## 4. monday MCP

### Server
- **URL:** `https://mcp.monday.com/mcp`
- **Marketplace install:** [auth.monday.com/marketplace/listing/10000806/monday-mcp](https://auth.monday.com/marketplace/listing/10000806/monday-mcp)
- **Plan availability:** All monday.com plans
- **Cost:** No additional cost for monday MCP itself ("you may incur costs from the tool you use to run MCP actions")
- **Auth:** Per-user OAuth. "Each user individually authorizes MCP via OAuth. MCP only has access to the data that you, as an individual user, can access in monday.com."
- **Security:** TLS encryption + OAuth standard + monday permission model. "Admins can limit access to specific workspaces, and assistants can only perform actions their connected user is already permitted to do."
- **Privacy:** "Only you and your AI assistant can see the data exchanged through MCP. monday.com does not review or access the content of your conversations."

### Supported AI clients (one-click connectors)

| AI Tool | How | Plan requirement |
|---|---|---|
| **Claude (Anthropic)** | Official connector directory | Pro / Max / Team / Enterprise plans (web/desktop/mobile) |
| **ChatGPT (OpenAI)** | Settings → Connectors → Advanced (developer mode) | ChatGPT Plus or Pro |
| **Cursor** | Verified plugin — installs MCP server automatically | — |
| **Microsoft Copilot Studio** | Native connector — add monday MCP as tool to any Copilot Studio agent | — |
| **Mistral Le Chat** | MCP-compatible | — |

### Two modes

- **Platform MCP** (default) — workspace automation tools
- **Apps MCP** (developer mode) — apps framework tools, via npm `@mondaydotcomorg/monday-api-mcp` with `--mode apps` flag

### Use cases monday publishes
- **Project reporting** — sprint summaries, team performance reports, deadline tracking from monday dev sprints
- **Smart task management** — convert meeting notes into structured items, assign, update statuses
- **Cross-team visibility** — "What's blocking the launch?" across Product, Marketing, RevOps
- **Operational workflows** — incidents, support requests, ops checklists
- **CRM workflows** — create leads/deals, update pipeline stages

### Tools exposed (incomplete inventory — full list at support.monday.com 32364501317906 which returned 403)
- Boards (create, read, modify)
- Items (CRUD)
- Columns (create, update, manage)
- Updates / comments
- Users / teams
- Workspaces
- Notetaker meetings query (Apr 2026)
- knowledge_base_search (AI search across knowledge snippets)
- ask_developer_docs (Apr 2026)
- Project / sprint queries (dev product)
- CRM operations (leads, deals, pipelines)

### Documentation URLs
- Main landing: https://monday.com/w/mcp
- Get started: https://support.monday.com/hc/en-us/articles/28588158981266-Get-started-with-monday-MCP
- Available tools: https://support.monday.com/hc/en-us/articles/32364501317906-monday-MCP-available-tools
- Apps mode developer doc: https://developer.monday.com/apps/docs/monday-apps-mcp
- Launch announcement: https://developer.monday.com/apps/changelog/introducing-the-mondaycom-mcp-integration
- Client setup guides (Claude/ChatGPT/Cursor/Copilot): all under support.monday.com

---

## 5. "All In on AI" — May 6, 2026

- **Source:** BusinessWire / monday.com IR (NASDAQ: MNDY)
- **Date:** May 6, 2026
- **Location:** New York & Tel Aviv

### Key positioning
- "monday.com has transitioned from a work management platform to an 'AI Work Platform'"
- "The most significant change in company history"
- "AI agents working alongside humans, configurable by team members without technical expertise"

### Executive quotes

**Roy Mann, co-founder & co-CEO:**
- "monday.com is now a place where people and agents work side by side."
- "The real measure of a platform isn't what it does — it's what it lets people do."

**Eran Zinman, co-founder & co-CEO:**
- "This is the biggest change in the history of our company, and we're going all-in on the new vision."
- (On 250K customers) "We owe them more than another AI feature."
- "We have re-architectured the core of our platform around a single belief that work should be orchestrated between humans and AI agents at scale from a single system of record."

### AI capabilities native monday.com agents can do
- Draft campaigns
- Qualify leads
- Close support tickets
- Onboard new hires
- Process purchase requests
- Operate 24/7 under human supervision

### Traction
- **250,000 customers** worldwide

### Industry context cited (Deloitte data)
- Enterprises have broadened AI access by 50%
- Only 25% have moved 40%+ of experiments into production
- Just 34% of companies use AI to deeply transform their businesses

### Partnerships & one-click connectors
- **Anthropic's Claude**
- **Microsoft 365 Copilot**
- **OpenAI's ChatGPT**

### Additional products launched
- **AI Platform Gateway** — access to multiple LLMs
- **monday vibe** — new AI-powered development tools
- **Redesigned mobile app** — Sidekick + agents unified

### Media contact
Tiffani Gibson, Sr. Communications Manager — tiffanigi@monday.com

---

## 6. Agentalent.ai — Mar 23, 2026

- **Source:** BusinessWire / IR
- **Date:** March 23, 2026
- **Source product unit:** **monday agent labs** (incubation engine for agentic work)

### What it is
- "A managed marketplace where enterprises can discover, evaluate, and hire AI agents for defined business roles"
- First launch from monday agent labs
- Two-sided model:
  - **Enterprise side:** post roles, review qualified agents, select based on task fit
  - **Developer side:** onboarding, contract management, billing, qualification process

### Qualification process
- Agents undergo authentication, authorization, and qualification before being introduced to organizations
- Companies can test performance before adoption
- "Introduces greater accountability into enterprise AI deployment"

### Built with
- **AWS + Anthropic**
- "Leveraging the most advanced frontier models, which handle highly complex agent workloads and are built specifically for the enterprise"

### Early adopters
- **Enterprise customers:** Wix, Mesh Payments
- **Partner ecosystem exploring agent roles:** Matrix, Ness Xebia, Devoteam, Impresoft Engage, Demicon
- Roles being explored: marketing, campaign execution, operational workflows

### Roy Mann quote (Mar 23)
> "Every company will soon have a blended workforce of humans and AI agents. As organizations face both talent gaps and the challenge of adopting AI, Agentalent.ai helps companies define roles, evaluate capability, and onboard AI agents alongside human teams using processes they already understand. As these agents become increasingly capable of operational work, I invite every company to open its ideal AI position and let us help find the right match."

### Constellation Research analysis
- Pricing "appears to range from $2,000 a month and up"
- 17 agents available at launch
- "It's likely to be the first of many similar efforts and quite possible that enterprise software vendors will start to resemble AI employment agencies"

---

## 7. Q4 2025 earnings

### Revenue numbers
- **FY2025 revenue: $1.232 billion** — **27% growth**
- **Q4 2025 revenue: $334 million** — **25% growth**

### AI traction metrics announced on earnings
- **monday vibe = fastest product in monday history to $1M ARR**
- **77M+ Monday Blocks actions powered**
- **500K+ Sidekick user messages processed**
- "Early beta users of AI agents are blown away by its capabilities"

### Pricing model
- New seats credit pricing structure for new customers
- Consumption-based pricing aligned with AI value
- "As AI agents take on more work across organizations, revenue expands naturally without requiring additional seat purchases"
- Existing customers can opt in to new model
- Enterprise customers receive complementary AI packages
- New customers: "two vectors of expansion — seats + AI credit consumption"

---

## 8. AI Credits pricing model

### Credit unit
- **1 AI Credit = $0.01** (one cent)

### Plan-level minimums (effective May 6, 2026 for new customers)
| Plan | Min. monthly credits | Credit options |
|---|---|---|
| Basic | 1,000 | 1,000 only ($10/mo) |
| Standard | 2,000 | 2,000 / 4,000 / 8,000 |
| Pro | 3,000 | 3,000 / 4,000 / 8,000 / 20,000 |
| Enterprise | — | Contact sales |

### Consumption rules
- **AI Blocks** — per action
- **monday sidekick** — per message **over the daily cap** (credit consumption starts May 20, 2026)
- **monday vibe** — per message
- **monday agents** — varies based on complexity (credit consumption starts June 8, 2026)
- **Image generation** — per image

### Free / no-credit features
- AI Sidekick conversations under the daily cap
- monday magic workspace generation
- Formula Builder (AI)
- Docs Assistant
- Deal Insights
- Risk Insights

### Sidekick tier mapping
| Plan | Sidekick tier | Notes |
|---|---|---|
| Free / Basic | NOT included | Basic gets AI credits for blocks / columns only |
| Standard ($12/seat) | Sidekick **(lite)** | Limited daily cap, credits over cap |
| Pro ($19/seat) | Sidekick **(lite)**, higher cap | Same features, more headroom |
| Enterprise | Sidekick **(plus)** | Up to 500 messages/user/day on Plus add-on; full assistant capabilities |

### Hard usage caps
- "Hard usage caps stop new AI actions when credits run out"
- "Existing automations keep running" (no service breakage on cap hit)

---

## 9. Brand evolution

| 2024–early 2025 | Post May 6, 2026 |
|---|---|
| AI Blocks | (still exists; no longer the headline brand) |
| monday magic | (still exists; not on /w/ai homepage; subsumed by Sidekick chat) |
| AI Hub | (deprecated UX; discovery moved to /w/ai) |
| Digital Workforce / Digital Workers | **monday agents** |
| SDR Expert agent | (Sales agents category in monday agents) |
| AI Service Agent | (Operations agents category) |
| Autopilot Hub | (subsumed by monday workflows) |
| AI Service copilot | (Service category in monday agents) |
| — | **monday sidekick** (new product line — May 2024 onwards) |
| — | **monday vibe** (new product line — 2025 onwards) |
| — | **monday workflows** (new infra — 2026) |
| — | **monday MCP** (new — 2025/2026) |
| — | **AI Platform Gateway** (new — May 6, 2026) |
| — | **Agentalent.ai** (new — March 23, 2026) |

---

## 10. Community sentiment

### Positive
**Nubia Magazine (review, 2026):**
> "AI features are useful but inconsistent. Sidekick is excellent at summarizing long boards and meeting notes. The AI workflow builder genuinely speeds things up. The risk insights feature in the portfolio view added real value."

### Pricing pain (multiple sources)

**Nubia Magazine (continued):**
> "AI credits run out faster than expected, and the per user AI credit limits introduced in 2026 mean that heavy users will frequently hit a wall and need to wait or upgrade."

**Mondaywiki:**
> "The change to non-renewable free AI credits, a new usage model where actions use 8 times as many AI credits and super expensive 'starter' AI Add-on Pricing Plans."

**TaskRhino:**
> "monday.com pricing is transparent for core Work Management plans, but watch for these potential add-ons: – Extra storage (~$5/month per 50GB) – Additional AI credits (variable pricing)"

### Key features praised
- monday vibe: most-cited differentiator, no direct competitor
- AI Blocks: "make AI accessible to non-technical users without needing prompt engineering"
- Risk insights, Deal insights, Docs Assistant: still free, widely praised
- Sidekick image generation (Mar 2026)

### What doesn't cost credits (mitigates some friction)
- Formula Builder, Docs Assistant, Deal Insights, Risk Insights — free
- monday magic — free
- Sidekick conversations under daily cap — free
- Hard caps don't break existing automations

---

## 11. Open questions / gaps

1. **ISO 42001 certification** — not explicitly named on /w/ai (ClickUp/Notion lead here). Worth checking AI Trust Center directly.
2. **Full monday MCP tool inventory** — support article 32364501317906 returned 403. Best to capture from a live MCP client.
3. **AI Platform Gateway architecture** — vendor docs sparse. How does intent routing work? Public details limited.
4. **monday vibe technical details** — built on mondayDB but no details on which models generate the apps. Anthropic-heavy guess given Agentalent partnership.
5. **Notetaker product** — Apr 2026 API exposed `notetaker_meetings` query but the in-product Notetaker feature wasn't on /w/ai. Is it Sidekick-driven or a separate product like ClickUp's AI Notetaker?
6. **Existing customer migration** — when do existing customers' AI credits become mandatory? "Existing customers can opt in to new model" — what's the timeline?
7. **monday agent labs scope** — Agentalent was the first launch. What's next from the lab?
8. **Sidekick Plus add-on tiers** — 500 msgs/day cited; full add-on tier table not captured.
9. **Skills marketplace developer revenue model** — how do Skill builders monetise?
10. **VSCode extension current status** — Oct 2024 launch; no further updates in window I fetched.
11. **WorkCanvas integration** — Mar 2025 native canvas; how does it fit with the new pillar story?
12. **Pre-May-2024 changelog** — earliest changelog entry I captured was May 8, 2024. Magic launched in July 2024 per /whats-new. Earlier AI work (image gen?) not captured.

---

## 12. Recommended screenshots

If you can capture from your live monday.com workspace:

1. **Sidekick floating assistant** on a board view
2. **Sidekick Skills Marketplace** with Gmail/Slack/Calendar skill installs
3. **monday vibe app builder** showing a generated app from a prompt
4. **monday agents catalogue** (pre-built agent gallery on Early Access page)
5. **Custom agent builder** with Knowledge + Integrations + Actions + Guardrails configuration
6. **monday workflows builder** with an AI-blocks workflow
7. **AI Block on a board column** (sentiment, classification, summarization)
8. **AI Credits usage dashboard** in admin panel
9. **AI governance per-user credit limits** in admin settings
10. **AI Trust Center** front page
11. **monday MCP setup screen** in Cursor or Claude.ai showing tools list
12. **Magic workflow generation** — describe-and-go example
13. **AI portfolio report** in monday work management
14. **AI Service Agent ticket auto-resolve** with confidence threshold settings
15. **Agentalent.ai marketplace** browse view (if accessible)
16. **AI Platform Gateway** (likely in admin / developer settings)
17. **Mobile app** showing Sidekick + agents unified view (May 6, 2026 redesign)

---

*Last updated: 2026-05-15 — companion to `monday_ai_research.html`.*
