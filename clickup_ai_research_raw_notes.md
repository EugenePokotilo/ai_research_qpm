# ClickUp AI — Raw Research Notes

> Working notes collected for [clickup_ai_research.html](clickup_ai_research.html). Verbatim extracts from each source so you can dig deeper, verify quotes, or build follow-up docs without re-fetching.
>
> **Run date:** 2026-05-15
> **Method:** WebFetch + WebSearch. No ClickUp MCP / playwright access in this session.

---

## Table of contents

1. [clickup.com/brain — Brain² feature inventory](#1-clickupcombrain)
2. [clickup.com/brain/agents — Super Agents](#2-clickupcombrainagents)
3. [clickup.com/brain/max — Brain MAX](#3-clickupcombrainmax)
4. [clickup.com/brain/ai-notetaker — AI Notetaker](#4-clickupcombrainai-notetaker)
5. [clickup.com/brain/enterprise-search — Enterprise Search](#5-clickupcombrainenterprise-search)
6. [clickup.com/brain/ambient-agents — Ambient Agents](#6-clickupcombrainambient-agents)
7. [Changelog entries by date](#7-changelog-entries-by-date)
8. [MCP server — official + community](#8-mcp-server)
9. [Acquisitions — Qatalog (Nov 2025) + Codegen (Dec 2025)](#9-acquisitions)
10. [Pricing & plans](#10-pricing--plans)
11. [Community sentiment](#11-community-sentiment)
12. [Open questions / gaps](#12-open-questions--gaps)
13. [Recommended screenshots](#13-recommended-screenshots)

---

## 1. clickup.com/brain

### Brand evolution
- Old name: ClickUp Brain (since late 2023)
- Current marketing on page: **"Brain²"** (Brain 2.0)
- Headline: **"Your company's Brain"** / **"One AI to Replace them All"**
- Subhead: **"The AI that actually knows your work"**

### Feature inventory (with surface + pricing)

| Feature | What it does | Surface | Pricing |
|---|---|---|---|
| Brain² (Brain 2.0) | Central AI; understands workspace context across tasks, docs, chat, calendar, email, connected apps | Inline, @mention anywhere, sidebar, chat, desktop, mobile | $9/user/mo Brain AI |
| Super Agents | User-created AI teammates running autonomously | Workspace-wide; runs in background | $28/user/mo Everything AI for "Flexible"; consumes Super Credits |
| Ambient Intelligence / Ambient Agents | Proactively surfaces context, related tasks, suggestions | Inline | GA |
| Deep Search | Synthesizes sources, builds reports, creates visualizations from a single prompt | Brain chat | GA |
| Memory & Preferences | Learns style, role, workflows; carries forward across conversations. **Import memory from ChatGPT and Claude** | All Brain surfaces | GA |
| Every Model, One Brain (multi-model) | Toggle between **GPT-5.2, Claude Opus, Gemini, and more** | Brain Assistant chat | Premium models on Everything AI |
| Connected Apps (MCP) | Taps Google Drive, GitHub, Salesforce, more | Inline + agents | GA |
| AI Notetaker | Joins meetings, transcribes, summarizes, generates action items | Calendar attached, link-based | Part of Everything AI ($28) or add-on from $12 |
| Talk to Text / Voice to Text | "Never use your keyboard ever again" | Brain MAX mobile + desktop | $9/user/mo standalone add-on |
| Enterprise Search | Permission-aware search across 100+ apps | Inline + Ambient Agents | Everything AI |
| AI Automations & AI-powered Fields | Auto-computed task properties; AI in Automation steps | Tables, Lists, Automations | Consumes Super Credits |
| Brain MAX (Mobile + Desktop) | Voice-first, context-aware super-app | Standalone Mac/Win/iOS/Android + Chrome | Free download; queries limited on free |
| Coworker | "AI that anticipates your next move, and gets it done" | Inline | GA |
| Codegen / Real Code Execution | Writes and runs real code against workspace data | @Codegen mention; Automations | GA |

### Positioning copy (verbatim)
- **"Your company's Brain"**
- **"One AI to Replace them All"**
- **"The AI that actually knows your work"**
- "100% Win rate vs ChatGPT & Claude in blind evaluation"
- "1.1 days Saved per employee per week"
- **"86% Cost savings vs standalone AI tools"**
- "3x Faster task completion"
- "Brain² is available now. Free to start."

### Data / privacy stance (verbatim)
- **"No third-party data training"** — "We forbid third-party AI providers from training on your data."
- **"Zero third-party data retention"** — third-party AI providers cannot store user data
- **"Multi-model unified security"** — uniform permissions/privacy/security across all models
- Compliance: SOC 2, ISO 27001, GDPR, HIPAA (and ISO 42001 on /brain/ai-notetaker page)
- **Brain conversations are private to the user — admins cannot view them**

### Pricing table
| Tier | Price | Includes |
|---|---|---|
| Free | $0 | Try Brain before committing |
| Brain AI | **$9/user/month** | Unlimited Brain, all premium models, 1,500 AI Super Credits |
| Everything AI | **$28/user/month** | Adds Notetaker, AI Fields, Automations, Super Agents |

Brain conversations are unlimited on paid plans and **do not consume Super Credits**.

---

## 2. clickup.com/brain/agents

### Headline / Positioning
- **"THE WORLD'S ONLY HUMAN-LEVEL AI AGENTS"**
- "@mention, assign tasks, & message directly"
- Counter shown on page: **3,337,254 Tasks automated by Super Agents**

### Human powers (triggers)
1. **Assign** — "Delegate tasks to your AI agents just like you would to a human teammate"
2. **Message** — Natural chat for questions, feedback, updates
3. **Mention** — Tag agents anywhere in the workflow
4. **500+ Human Skills** — "Send emails, DM users, schedule events, and so much more"

### Superpowers (operational modes)
- **24/7** — work around the clock
- **Ambient** — work silently in background, anticipating needs
- **Automated** — handle repetitive tasks
- **Self-learning** — "Every interaction, job, and piece of human feedback improves Super Agents"

### Superintelligence
- **Infinite Memory** — "Recent memory, working memory, and long-term memory are automatically stored and recalled"
- **Infinite Knowledge** — full workspace sharing + connected tools with "real-time, permissions-aware knowledge syncing"

### Super Agent Builder (Studio)
- "The world's only infinite agent catalog"
- "Build the exact agent you need" — "Describe the job, and build the perfect agent. No technical skills required"
- **One prompt spins up an entire team** — goals, workflows, and frustrations get auto-delegated to multiple agents

### Agent categories
- PM Agents · Sales Agents · Coding Agents · Designer Agents · Certified Agents (marketplace)
- Org-chart examples: Designer Agent, Brand Agent, Executive Assistant (reporting to a human Head of Marketing)

### Sample of the 500+ skills (verbatim list from page)
write copy · analyze data · draft emails · track expenses · manage invoices · track keywords · schedule posts · run reports · brainstorm · create briefs · monitor trends · book meetings · set reminders · plan campaigns · edit copy · proofread · summarize · send messages · create dashboards · design mockups · debug code · review docs · tag assets · build decks · update styleguides · survey users · check links · fix errors · sync data · competitive analysis · automate tasks · create logos · optimize content · troubleshoot · write scripts · maintain wikis · conduct studies · compile data · prepare presentations · route tickets · archive files · edit videos · perform audits · resolve tickets · parse data · build forms · curate content · improve rankings · generate leads · write proposals · clean data · build manuals · prepare budgets · onboard users · test features · maintain records · verify info · merge contacts · backup data

### 7 capabilities (Superintelligence tabs)
1. **Memory** — episodic + agent preferences + short-term + long-term
2. **Knowledge** — vast databases + learning from every interaction
3. **Collaboration** — works with humans and other agents
4. **Skills** — "specialized tasks with precision and consistency"
5. **Autonomous** — independent decisions and actions
6. **Ambient** — runs quietly in background
7. **Feedback** — learns from outcomes

### Proprietary tech: BrainGPT
- **Optimized Orchestration** — "Route to the best models from intent"
- **Self-Learning** — continuous improvement
- **Human-level Memory** — Short, Long-Term, & Episodic
- **Sub-Agent Architecture** — multi-agent collaboration/delegation
- **Deep Research & Compression** — "Research optimally from compressed context"

### Workspace + integration layer
- **Agent Analytics** — measure productivity, monitor trends, spot top performers
- **Ambient Awareness** — context-aware Q&A
- **Live Intelligence** — captures decisions, people, insights, updates into knowledgebases
- **Infinite Knowledge** — real-time syncing with "world-class retrieval from fine-tuned embeddings"
- **Enterprise Connected Search from 50+ Apps** — logos: ClickUp, Gmail, Google Drive, Confluence, Slack, Dropbox, Salesforce, MS Teams, GitHub
- **Real-time 2-way syncing engine**

### Permissions & security model
- "Built on the same battle-tested user data model your team already uses"
- Agents can inherit implicit access, receive explicit permissions, or be granted access manually
- Controls span: Integrations, Sharing, Permissions
- **Audit everything** — every agent action logged (post comment, summarize, create task, assign, status change, update database, generate report, etc.) with timestamps and location
- **Zero data retention. Zero training.** — "More secure than using OpenAI, Gemini directly"
- **Reflection** — "execution loops that ensure Agents constantly reflect on work they're doing"

### Quotes from named executives
- **Jay Hack, CEO of Codegen → now ClickUp Head of AI:** "The holy grail of what enterprises are chasing - this is a game changer for work productivity."
- **Zeb Evans, ClickUp CEO:** "Our custom platform uses contextual engagement, orchestration, and fine-tuning to provide maximum human productivity."

### Super Fair Billing Policy
- "AI cost savings are passed through; sudden cost increases from new models are subsidized so credit usage stays stable."

---

## 3. clickup.com/brain/max

### Positioning
- **"One AI to Replace them All"**
- "Powered by Brain m1"
- Product Hunt's **#1 Product of the Week in both Productivity and AI categories**

### Claimed benefits
- **1.1 days** saved per week
- **4X faster** than typing
- **86% cost savings** vs replacing multiple subscriptions

### Platform availability
- **Brain MAX Desktop** (Mac & Windows)
- **Brain MAX Chrome** (extension)
- **iOS & Android** (mobile)
- **Talk to Text** (separate download)

### Voice / Talk to Text
- "Your voice is the fastest keyboard"
- Dictation at **~220 wpm vs ~45 wpm typing**
- "You do the talking, AI does the typing — and the editing!"
- Updates calendar, assigns tasks, sends messages, drafts Docs
- **@Mentions with context** — auto-connects, tags, notifies people
- **Personal vocabulary** — learns names, phrases, work-specific jargon

### Universal AI features
- **Universal Search** across connected apps for files, threads, and conversations
- **Universal AI** — chat with multiple premium models (Gemini, OpenAI, Claude, and Brain) without app-switching
- **Web search** with citations
- **Deep search** for research-style answers
- **AI generation** — images, tasks, messages, projects

### Pricing
- **Free forever. No credit card required** for download
- Free users have limited Brain MAX queries
- Paid users get expanded usage
- ClickUp AI customers enjoy unlimited queries
- Autopilot/Talk-to-Text customers enjoy unlimited Talk to Text
- Subject to Fair Use Policy

### Status
- GA (no beta label on Brain MAX itself)
- "Super Agents" feature marked "New"
- **VibeUp** marked "Soon" in nav

---

## 4. clickup.com/brain/ai-notetaker

### Supported meeting platforms
- "Join any call from anywhere in ClickUp"
- Specific platforms (Zoom, Teams, Google Meet) **not named** on page, but other docs/changelog show: link-based to any call, calendar-attached for scheduled meetings, SyncUps in-product calls

### What it captures
- **Searchable transcripts** with speaker attribution
- **Smart summaries** in TL;DR form
- **Video recordings** delivered to private Docs
- **Action items** auto-converted to assigned tasks
- **Decisions + topics** stored in Brain memory

### Pricing
- $12/mo (60 hours), $19/mo, $18/mo, $16.99/mo, $15/mo shown on comparison row
- ClickUp positions itself as "the best price on the market"
- Free tier implied by "Get Started. It's free" CTAs

### Surfaces / Integration
- **Docs**: Private Docs receive transcripts, video, summaries
- **Tasks**: Action items become assigned tasks automatically
- **Chat**: Aggregated answers from all meeting notes
- **Brain**: "I can ask Brain about any of my meetings"

### Privacy
- GDPR, **HIPAA**, SOC 2, **ISO 42001** compliant
- "No third-party data training" + "Zero third-party data retention"

---

## 5. clickup.com/brain/enterprise-search

### Connected apps named on page
- Google Drive
- Notion
- Slack
- Gmail

Quote: *"From Drive and Notion to Slack and Gmail - every app, connected and searchable from one place."*

### MCP info (per this page)
- **No information about MCP server, integration, or endpoints** on this page. MCP details come from changelog + help center articles instead.

### Indexing
- "Brain indexes content frequently, so your searches are up to the minute."
- No specifics on storage location or data residency

### What it can search across
- "Pulls from tasks, docs, chats, and meetings to give the full picture."
- "Ambient Agents tap into every doc, task, message, and app to deliver trusted, real-time responses."

### Privacy
- "We forbid third-party AI providers from training on your data."
- "We don't allow third-party AI providers to store any of your data."
- Compliance: GDPR, ISO 42001, HIPAA, AICPA SOC 2

---

## 6. clickup.com/brain/ambient-agents

### Positioning
- "AI that works on your behalf"
- "Always in context, always on"

### Specific agent types
- **Live Answers Agent** — "Listens for questions and automatically gives rich answers with complete context"
- **Live Intelligence Agent** — "Surfaces real-time insights, makes actionable recommendations, and keeps workspace context up-to-date"
- **General Ambient behavior** — "Agents respond to team questions, generate weekly updates, and more—automatically. Built by ClickUp experts."
- "100s more" pre-built variants

### Where they surface
- Inside ClickUp chats and conversations (auto-answering questions)
- In workspace updates and standups
- Across connected tools — "work with data from your Google Drive, GitHub, Salesforce, and 20+ other apps"

### Difference from Super Agents
- **Ambient Agents** are pre-built by ClickUp experts, run passively/continuously ("always on"), react to events
- **Super Agents** are user-built (or template-derived), triggered explicitly, autonomous task execution

### No-code builder (3 steps)
1. **Choose your prompt**
2. **Choose your context** (specific resources or apps)
3. **Choose your AI tools** (create, manage, summarize, etc.)

---

## 7. Changelog entries by date

### May 5, 2026 — Release Notes 4.04
- **Brain Goes Mobile (iOS & Android):** Revamped Brain works throughout the mobile app via a floating button; supports dictation; syncs conversations across devices
- **AI Notetaker — Meeting Notes Your Way:** New toggles to "keep the recording, transcript, or just the summary" via Calendar settings → AI Notetaker
- **ClickUp inside ChatGPT:** Install from ChatGPT's App Store; surfaces tasks/updates/priorities in conversation, grounded in live ClickUp data. All plans.
- **Super Agents & Brain enhancements:**
  - Agents handle reminders end-to-end (create, summarize, update, complete)
  - Can run on hourly schedules with guardrails against overlapping runs
  - Auto-DM new managers a rundown
  - Instructions/tools/tone editable via DM, @mention, or task comment without using Agent Builder
- **ClickUp in Cursor:** Install in Cursor via OAuth. Search tasks, Docs, comments and create/update via NL prompts. All plans.

### April 8, 2026 — Release Notes 4.03
- **Google Drive Automations:** Auto-create folders/Docs when ClickUp tasks are created; alert team in ClickUp when new Drive files are added (AI-adjacent)
- Workload grouping, invited-user team assignment

### February 24, 2026 — Release Notes 4.02
- **AI auto-classification of Task Types:** Use AI to auto-classify task types and keep them "clean and consistent" in List/Table views
- **AI Notetaker via link:** Send AI Notetaker to any call (including ad-hoc) using just a link
- **Pin to top of Workspace** for one-click access

### January 29, 2026 — Super Agents: Release Notes Takeover (4.1)
- Full launch of **Super Agents™** as "personalized AI teammates"
- Available on ClickUp 4.0 for any Workspace with AI enabled
- **Human-like collaboration:** @mention, assign tasks, or DM agents
- **500+ skills:** email, scheduling, reporting, image generation; schedulable or automation-triggered
- **Infinite knowledge and memory:** Adapt to preferences, remember tasks, store decisions in editable docs
- **Super Agent Builder:** Guided step-by-step creation
- **Security/permissions:** Default to public Workspace data; real-time audit logs; admin granular controls

### January 15, 2026 — Super Agents AMA on Reddit
- AMA on Jan 22, 10am–12pm PST at r/ClickUp
- Hosted by Senior PM Michael Van Doorn

### December 22, 2025 — Introducing Super Agents™
- Initial launch — "first human-like AI agents that live inside ClickUp"
- Capabilities: see tasks/docs/chats/meetings/schedules together
- Run workflows 24/7 (triage, scheduling, reporting, emailing)
- Accept @mentions, assignments, DMs, schedules, triggers
- Powered by new agent architecture (BrainGPT)
- Available immediately to everyone

### December 12, 2025 — 4.0 Release Notes Takeover
- **AI-Powered Planner:** Powered by ClickUp Brain — auto-blocks focus time, shows teammate availability, one-click meeting scheduling, multi-time-zone support
- **Teams Hub:** One-click AI-generated standups
- **My Tasks:** AI StandUps + Autopilot Agents on Personal List page

### December 10, 2025 — "To our incredible community" (Zeb Evans keynote)
- **Calendar & AI Notetaker** highlighted
- **AI Agents** framed as "your AI workforce that handles tasks across your entire workspace"

### December 5, 2025 — Release Notes 3.64
- **Gmail ↔ Brain AI:** Connect Gmail to Brain for email intelligence (prioritizing, summarizing)
- **Codegen Agent:** Tag @Codegen or assign it to a task; it gathers context, writes production-ready code, opens a PR. Also available in Automations.
- **Real-time AI Usage Dashboard:** Members, Admins, Owners can track AI credits — usage, remaining balance, trends

---

## 8. MCP server

### Official ClickUp MCP server
- **URL:** `https://mcp.clickup.com/mcp`
- **Status:** Public beta, available on all plans
- **Auth:** OAuth ONLY — "you cannot authenticate using your own API keys or Auth access tokens"
- **Admin gate:** In Team / Enterprise / Edu workspaces, only owners and admins can configure MCP servers
- **Safety constraint:** "For the time being, ClickUp hasn't added any deletion tools as a safety measure"

### Rate limits (without Everything AI add-on)
- **Free Forever Plan:** 50 calls / 24 hours
- **Unlimited Plan and above:** 300 calls / 24 hours
- Everything AI customers get higher limits

### Setup config (Cursor, Claude, VS Code, ChatGPT)
```json
{
  "mcpServers": {
    "ClickUp": {
      "command": "npx",
      "args": ["-y", "mcp-remote", "https://mcp.clickup.com/mcp"]
    }
  }
}
```

### Tool coverage (from official + community refs)
- Tasks (create, update, list, comment)
- Lists, Folders, Spaces
- Docs (read, edit)
- Sprints & cycles
- Checklists
- Tags
- Time tracking
- Files / attachments
- Chat messages
- Custom fields read
- **⚠ NO deletion tools** (intentional safety)

### Example prompts published by ClickUp
- "Create a task for this bug we're working on."
- "Find all my incomplete tasks due this week."
- "List all milestones in the Product Launch project."
- "How many hours has the team spent on clients this month?"

### Community alternatives

**taazkareem/clickup-mcp-server (most popular):**
```json
{
  "mcpServers": {
    "ClickUp": {
      "command": "npx",
      "args": ["-y", "@taazkareem/clickup-mcp-server@latest"],
      "env": {
        "CLICKUP_API_KEY": "your-api-key",
        "CLICKUP_TEAM_ID": "your-team-id",
        "CLICKUP_MCP_LICENSE_KEY": "your-license-key"
      }
    }
  }
}
```
- API-key auth, local execution
- Complete API coverage including delete
- Filter flags for read-only or task-focused agents
- Also offers HTTP transport for Claude Code: `claude mcp add --transport http ClickUp https://clickup-mcp.taazkareem.com/mcp --header "X-License-Key: your-license-key"`

**Nazruden community server:**
```json
{
  "mcpServers": {
    "clickup": {
      "command": "npx",
      "args": ["@nazruden/clickup-server"],
      "env": {
        "CLICKUP_PERSONAL_TOKEN": "your_personal_api_token_here"
      }
    }
  }
}
```
- Personal Token auth (from "My Settings" > "Apps")
- Smithery install: `npx -y @smithery/cli install @Nazruden/clickup-mcp-server --client claude`

### Official docs URLs
- https://developer.clickup.com/docs/connect-an-ai-assistant-to-clickups-mcp-server
- https://developer.clickup.com/docs/connect-an-ai-assistant-to-clickups-mcp-server-1
- https://help.clickup.com/hc/en-us/articles/33335772678423-What-is-ClickUp-MCP

---

## 9. Acquisitions

### Qatalog acquisition (November 12, 2025)
- **Source:** BusinessWire
- **Price:** Terms undisclosed; Qatalog had raised **$25.4M** (BusinessWire) / $26M (other sources)
- **Investors who funded Qatalog:** founding members of Indeed, Salesforce, Slack and Zoom; executives from SAP, Workday, Google
- **Customers pre-acquisition:** Nvidia, Twitter, Airbnb
- **Tech acquired:** **ActionQuery AI** — permission-aware, no-index search engine
- **Integration scope:** "more than 100 connected enterprise applications"
- **Completion:** Deal closed Q1 2025; announcement deferred to Nov 2025
- **Strategic fit:** "Power AI agents with full business context, enable automated workflows informed by every conversation and document, deliver real-time insights without leaving ClickUp"

**Quote — Zeb Evans:**
> "Software is finally converging, and it's about time. With Qatalog, we're not just adding another feature, we're unlocking the next level of AI transformation. True AI is only possible when it has 100% context."

**Quote — Gaurav Agarwal (ClickUp COO):**
> "We have admired Qatalog from afar for a while. They have been at the forefront of really trying to build modern work software: beautifully designed, great product marketing and really great user experiences delivered seamlessly."

### Codegen acquisition (December 23, 2025)
- **Source:** BusinessWire
- **Price:** Terms undisclosed; ClickUp valuation cited as **$4B**
- **Leadership move:** **Jay Hack** (Codegen founder & CEO) → **Head of AI at ClickUp**
- **Codegen pre-acquisition:** AI-powered code generation, autonomous PRs (Cursor competitor)
- **Tech acquired:** BrainGPT-style orchestration, sub-agent architecture, episodic memory
- **Standalone product sunset:** **January 16, 2026**

**Quote — Jay Hack:**
> "The bottleneck to agents transforming how work is done is no longer AI capabilities, it's context. ClickUp is the only platform that houses all of a company's plans, docs, and goals in one place. By combining Codegen's agentic technology with ClickUp's unified workspace, we're not just building a smarter coding tool; we're building a Super Agent workforce that scales infinitely across software engineering, product management, sales, enterprise workflows, and beyond."

**Quote — Zeb Evans:**
> "The future isn't about humans adapting to AI, it's about AI adapting to humans. By bringing Codegen's world-class team and technology together with ClickUp Super Agents, we're realizing the promise of truly intelligent digital coworkers. Super Agents don't just automate. They understand, remember, and act with context, unlocking a new era of productivity where anyone can build and scale work systems without writing a single line of code."

### Market context (per BusinessWire)
- 2025 surge in AI coding startup acquisitions: Google acquired Windsurf and Cognition; Anthropic acquired Bun; Cursor acquired Graphite
- ClickUp pitched as directly challenging Atlassian (Jira) and Notion

---

## 10. Pricing & plans

### Annual yearly pricing
- **Free Forever** — $0
- **Brain AI** — $9/user/mo (monthly: $18)
- **Everything AI** — $28/user/mo (monthly: $68)

### Feature availability by tier

**Free Forever:**
Trial access to Brain Assistant, Web Search, AI Writing, @Brain, Project Summaries, Super Agents, Ambient Answers, Autopilot Agents, AI Fields, AI Cards, AI Assign, AI Prioritize, AI Time Blocking, Image Generation, Talk to Text, Enterprise Search, AI Notetaker

**Brain AI ($9/user/mo):**
- Full access: Brain Assistant, Web Search & Research, Foundational AI Models, AI Writing, @Brain, Project Summaries & Updates
- **"Standard"** level: Super Agents, Ambient Answers, Autopilot Agents, AI Fields, AI Cards, AI Assign, AI Prioritize, AI Time Blocking, Image Generation
- Trial only: Talk to Text, Enterprise Search, AI Notetaker, Premium Reasoning Models, Brain MAX

**Everything AI ($28/user/mo):**
- Brain MAX desktop app
- Premium Reasoning Models (labeled "$200 Value")
- **"Flexible"** Super Agents
- **Unlimited:** Ambient Answers, Autopilot Agents, AI Fields, AI Cards, AI Assign, AI Prioritize, AI Time Blocking, Image Generation, Talk to Text, Enterprise Search, AI Notetaker

### AI Super Credits
- **$10 / 10,000 credits**
- Consumed by: Super Agents, AI Fields, Image Gen, "and more"
- Super Agent rate shown as **$0.01** per credit

### Optional Add-Ons
- **Talk to Text:** $9/user/mo — unlimited voice dictation
- **AI Notetaker:** from $12/mo for 60 hours/month — recording + summaries + transcripts + action items
- **AI Live Training Workshop:** $400 one-time, 2-hour session

### Notes
- **Codegen:** Not separately priced (bundled into the AI tiers)
- **VibeUp:** Listed as "Soon" — no pricing
- **Super Fair Billing policy:** Cost savings passed through; rate increases "gradual and transparent"
- Usage subject to Fair Use Policy

---

## 11. Community sentiment

### Adoption metrics ClickUp publishes
- **$300M ARR** as of Sep 2025
- **20M+ users**
- **AI sales 400% YoY** through 2025
- **AI usage 800% YoY** through 2025
- **3.3M+ tasks automated** by Super Agents (live counter on /brain/agents)
- **86% claimed cost savings** vs standalone AI tools
- **100% win rate vs ChatGPT & Claude** in blind evaluation (ClickUp's own benchmark)
- **IPO plans:** CFO Dan Zhang said in Sep 2025 — "may wait until market conditions improve"

### ZenPilot review (Mar 2026, largest ClickUp Solutions Partner, 200+ workspaces)
> "If you're already on ClickUp, upgrade to 4.0. You'll need to migrate here in early 2026 anyway. Use the 'soft launch' settings to roll it out to yourself first, then your team in phases. If you're evaluating ClickUp for the first time, this is the best version of the platform they've ever shipped. The convergence vision — tasks, chat, docs, AI all in one place — actually works now."

**Concrete productivity wins reported:**
- **Engineering:** Bug triage agent monitors incoming issues, auto-assigns based on component tags and current workload, posts a daily blocker digest. Saves leads 30–45 minutes of triage per day on active sprints.
- **Marketing:** Campaign status agent pulls task completion rates every Friday, generates a client-ready summary, flags deliverables at risk — without account managers compiling manually.

### Performance history acknowledged
- "The self-reported 40% load-time improvement on workspaces with 1,000+ tasks is a direct response to the performance-at-scale complaints that dominated G2 and Reddit threads in 2022 and 2023."

### WorkManagementHub critique (May 2026)
- **Data quality dependency:** "Agents reporting on project health are useless if tasks lack due dates, assignees, or status updates. Deploying agents before fixing team data discipline accelerates the wrong behaviors."
- **Audit complexity:** "Agents with write permissions intermix agent and human actions in activity logs. ClickUp's Activity log helps, but compliance-sensitive teams should configure agents conservatively until audit tooling matures."
- **Cross-system failure handling:** "Agents executing multi-system workflows (Salesforce → ClickUp → Slack) may fail non-obviously if one integration breaks. Build monitoring into any cross-system workflow from the start."

### Vellum critique (2026)
- "Locked to ClickUp. Super Agents operate inside ClickUp's platform. If your work happens outside ClickUp (local files, email, other apps), the agents can't reach it."

### Pricing friction (multi-source complaint)
- "ClickUp's AI features are offered as a separate add-on. ClickUp Brain, AI Notetaker, Super Agents, and other AI-powered workflows are not automatically included in the base plans. In practice, this means you choose a plan first, and then add ClickUp AI if you want access to its AI features."

### Open user request flagged on feedback board
- "@mention SuperAgents 🚫" — users want to @mention Super Agents within Doc comments
- Use case: triggering a Personal Meeting Coach on AI Meeting Notes Documents
- ClickUp staff confirmed early 2026 they're actively working on it

### Bottom line
1. Power users + partners: bullish (ZenPilot, WorkManagementHub)
2. Independent reviewers: flag AI add-on pricing + ecosystem lock-in
3. Competitors: emphasize agents can't reach work outside ClickUp
4. Feedback boards: enthusiasm + active requests for missing integrations (Doc @mentions, etc.)

---

## 12. Open questions / gaps

1. **Codegen vs @Codegen current status** — Standalone Codegen sunset Jan 16, 2026. Is `@Codegen` still the active brand inside ClickUp, or has it been merged into generic Super Agents? Worth verifying in a live workspace.
2. **VibeUp** — listed as "Soon" in nav. Likely a vibe-coding / Lovable competitor. No public details.
3. **SyncUps support details** — the in-product video call product. How does it differ from a Zoom-equivalent technically? No deep dive fetched.
4. **Brain MAX vs Brain in-app** — what features specifically differ? Brand m1 is mentioned as Brain MAX engine; is base Brain also on m1 or different?
5. **"Foundational AI Models" naming on Brain AI tier** — unclear which exact models are in the lower tier. GPT-4o mini? Claude Haiku? Gemini Flash?
6. **ISO 42001 certification scope** — first PM tool to loudly mention ISO 42001 (AI management standard). Worth a deeper look for QPM's own potential certification path.
7. **AI Notetaker platform support** — Zoom/Teams/Meet not named on the page explicitly. Worth verifying.
8. **Agent Marketplace (Certified Agents)** — categories shown on /brain/agents include "Certified Agents." Is there a public marketplace? Pricing for marketplace agents?
9. **MCP tool surface complete list** — official docs don't enumerate tools. Best to capture from a live MCP client connection.
10. **Hourly schedule limits** — May 2026 enabled hourly Super Agent schedules with "guardrails against overlapping runs." What are the actual limits?
11. **Codegen tech inside Super Agents** — the framing "Codegen technology powers Super Agents" vs "BrainGPT" — is BrainGPT the new branding for the Codegen stack, or distinct?
12. **r/ClickUp threads** — search didn't surface direct Reddit threads. Worth a direct site:reddit.com search.

---

## 13. Recommended screenshots

If you can capture from your live ClickUp workspace:

1. **Brain Assistant chat panel** — full chat surface with model toggle visible
2. **@Brain mention in task editor** — Writing actions menu
3. **AI Notetaker output Doc** — transcript + summary + action items
4. **Super Agent Builder (Studio)** — natural-language agent creation flow
5. **Super Agent in action** — agent posting in a task or chat
6. **AI Usage Dashboard** — credit consumption + trends
7. **Audit log** — agent action filter
8. **Brain MAX desktop app** — home screen with Talk to Text
9. **Brain MAX Chrome extension** — in-tab summarize action
10. **Talk to Text in action** — voice input on mobile
11. **Enterprise Search query** — cross-app result panel
12. **Ambient Agent (Live Answers) responding in chat**
13. **AI-Powered Planner** — auto-blocked focus time on calendar
14. **AI Fields configuration** — custom AI-computed column
15. **MCP Server setup screen** in Cursor or Claude.ai showing ClickUp tools list
16. **ChatGPT App Store** — ClickUp app install screen (May 2026)
17. **ClickUp in Cursor** — OAuth flow + tools listing

---

*Last updated: 2026-05-15 — companion to `clickup_ai_research.html`.*
