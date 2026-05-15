# Asana AI — Raw Research Notes

> Working notes collected for [asana_ai_research.html](asana_ai_research.html). Verbatim extracts from each source.
>
> **Run date:** 2026-05-15
> **Method:** WebFetch + WebSearch. No Asana MCP / playwright access in this session.

---

## Table of contents

1. [asana.com/product/ai — AI overview](#1-asanacomproductai)
2. [asana.com/product/ai/ai-teammates — Teammates](#2-asanacomproductaiai-teammates)
3. [Work Graph + Memory architecture](#3-work-graph--memory-architecture)
4. [asana.com/whats-new — Winter 2026 release](#4-asanacomwhats-new)
5. [Earnings + financial context](#5-earnings--financial-context)
6. [Pricing + AI Studio credits](#6-pricing--ai-studio-credits)
7. [Asana Gov + public sector](#7-asana-gov)
8. [Open questions / gaps](#8-open-questions--gaps)
9. [Recommended screenshots](#9-recommended-screenshots)

---

## 1. asana.com/product/ai

### Marketing positioning (verbatim)
- "AI that works for you" — "Let AI take on busywork so your teams can focus on strategic work."
- "AI that works where you do" — embeds AI where teams already work, no separate tools.
- "AI you can actually trust" — "transparent, controlled, and secure."
- Top tagline: "Human + AI collaboration that moves work forward"
- "Asana AI works with your teams, delivering results with the full context of your business and goals."

### AI Features

**AI Teammates**
- "Drive marketing campaigns, manage IT tickets, support operations, and more."
- Available ("ready to get started when you are")
- Pricing: not stated on the page; sales-led

**AI Studio**
- "Design AI-powered workflows to handle routine tasks—no code required."
- Available on Starter, Advanced, Enterprise, Enterprise+ plans
- Requires admin enablement in admin console

**Smart Workflow Gallery**
- "Prebuilt workflows designed with best practices in mind" that teams can tailor

**Smart Assists**
- "AI that surfaces insights and keeps projects on track"

**AI Connectors**
- "The bridge between your big ideas and the work that brings them to life"
- Lets users kick off projects from external AI apps
- Logos: OpenAI, Slack, Notion

### Features NOT on this page
- Work Graph, smart fields, AI risk reports, Asana Gov are not detailed on /product/ai
- Specific AI model names not disclosed (page refers to "AI partners" plurally)
- "context, checkpoints, controls" phrasing does NOT appear verbatim on this page (it's used in earnings/PR copy)

### Data / Privacy (verbatim bullets)
- "Our AI partners do not use customer data to train their models"
- "Our AI partners are required to delete customer data after each query"
- "Your teams are always in the loop, empowering them to guide AI in the right moments"
- "Access to data is restricted through precise controls and permissions"

### FAQ-level privacy details
- AI follows Asana's permissioning model (AI accesses only what users can access)
- "Asana's AI partners currently have servers located in the US."
- AI partner identities are referenced via a linked help article rather than disclosed on-page

### Pricing
- "Asana AI is available on all paid tiers."
- AI Studio specifically requires Starter, Advanced, Enterprise, or Enterprise+

### Customer logos
Figma · TOMS · Clear Channel · GoodRx · Anthropic · Morningstar (featured case study, Belinda Hardman, Director of Program Management)

---

## 2. asana.com/product/ai/ai-teammates

### Positioning (verbatim)
- "Collaborative AI agents built for teams (not individuals)"
- "Take on complex work to deliver outcomes and collaborate with your team — just like a real teammate would."

### 21 Prebuilt AI Teammates

**Marketing (7):**
1. **Campaign Brief Writer** — Skills: Goal Alignment, Context Extraction, Brief Architecture
2. **Brand Auditor** — Voice Governance, Artifact Auditing, Messaging Compliance
3. **Launch Planner** — Roadmap Syncing, GTM Sequencing, Dependency Mapping
4. **Copywriter** — Drafts marketing copy in brand voice
5. **Competitive Market Researcher** — Summarizes market data into comparisons
6. **Content Localization Manager** — Translates while preserving brand voice
7. **Creative Spec Writer** — Custom workflow automation

**Operations & PMO (6):**
1. **Pricing Strategist** — Analyzes past deals to recommend pricing
2. **Status Reporter** — Turns updates into executive-ready reports
3. **Business Case Builder** — Creates ROI-backed business cases
4. **Decision Tracker** — Searchable record of key decisions
5. **Workflow Optimizer** — Finds bottlenecks, suggests fixes
6. **Data Quality Manager** — Cleans missing data and formatting

**IT (5):**
1. **IT Support Specialist** — Answers IT questions from internal docs
2. **Trend Analyst** — Spots patterns in support tickets
3. **Compliance Specialist** — Reviews docs against regulatory standards
4. **Onboarding Assistant** — Answers new hire questions
5. **Vendor Evaluator** — Reviews vendor proposals against requirements

**Product & Engineering (3 listed + Time Tracker mentioned in customer story):**
1. **Spec Reviewer** — Audits product specs for gaps
2. **Bug Investigator** — Technical triage, Pattern recognition, Blocker tracking
3. **Sprint Coach** — Agile orchestration, Velocity tracking, Productivity analysis
4. **Time Tracker** — (featured in Living Spaces customer story)

> Note: "21 prebuilt" total is what marketing claims. The breakdown adds to 21 (7+6+5+3) — Time Tracker may be a Product/Eng one or counted separately.

**Custom Teammate option:** Available in every category — no coding required.

### Integrations
Microsoft Word, Google Docs, Microsoft Excel, Google Sheets, Google Drive, SharePoint

### Key capabilities (verbatim)
- "Progress never stops: spot risks, find solutions, and keep your teams running around the clock"
- "Team-aware: Learn from past projects so you don't re-explain context"
- "Transparent: show their work and stay within permissions your team sets"

### Setup (3 steps)
1. **Describe the role** — "Select a prebuilt teammate or create your own—no coding required"
2. **Connect to projects** — "Add to projects so it understands team work within set permissions"
3. **Assign tasks** — "Treat like any team member"

### Governance & Security
- Inherit existing Asana enterprise-grade access controls
- Never elevate access beyond user permissions
- Must be "explicitly added to private projects and tasks"
- Control who can create, modify, share, and teach each teammate
- "Neither Asana nor our AI partners use customer data to train AI models"
- AI partners delete data after each interaction

### Customer results (verbatim quotes)
- **Morningstar** (Laura Kohl, CIO): "It completed weeks of complex research in hours."
- **KW Automotive** (Kea Brun): "saved me 2-3 hours of work"
- **Living Spaces** (Matt Odom): Time Tracker teammate fixed calculations that "would have taken us days to do manually"
- **Asana's own security team**: "10–15x the coverage across the software development lifecycle"
- **Asana marketing ops**: Cut post-offsite project reviews "from 4 hours to 45 minutes"

### Pricing/plan
- Available as an **add-on to Starter, Advanced, Enterprise, and Enterprise+ plans**
- Specific pricing not listed — sales-led

### AI Teammates vs AI Studio (verbatim)
"AI Studio automates repeatable work at scale, while AI Teammates take on collaborative, complex tasks." Designed to work together.

### Distinction from chatbots (verbatim)
Chatbots "respond to prompts in isolated conversations" — AI Teammates "analyze project context, collaborate with teams, and help complete tasks directly within shared projects."

---

## 3. Work Graph + Memory architecture

### Work Graph definition (verbatim)
- "Similar to Facebook's Social Graph but specifically for workplace productivity"
- "A collection of historical relationships and context across an organization's teams, work, and workflows"
- Encodes every task, project, goal, and conversation within a web of relationships: who owns it, who's collaborating, what it contributes to, what depends on it

### Core architectural decision (verbatim)
> "When they started building AI agents, the question became — what if the AI operated within this same structure — instead of inventing a separate context model for the AI, they let it participate in the collaboration model already built. This is the core conceptual model behind AI Teammates: wherever possible, their capabilities match those of a human user within an organization."

### How context flows to a Teammate
1. **Immediate task context** — when assigned, Teammate receives context about that task + all immediately connected work: parent project, related goals, dependencies, collaborators
2. **Broader graph search** — Teammate can "search across the broader work graph, pulling in relevant tasks, projects, goals, and people based on what's useful"
3. **Shared multi-user context** — multiple people interact with same Teammate on shared work; Teammate accumulates working knowledge across collaborators and initiatives
4. **Graph-native reasoning** — "Because the work graph already captures how teams coordinate, the Teammate can reason about work the way a collaborator does"

### Memory system architecture

**Why text-fact memory (not vector DB)?**
> "Asana started here rather than with a vector database or knowledge graph because they wanted to understand what a tight feedback loop could achieve before investing in heavier infrastructure. What they found is that the loop does most of the heavy lifting."

**Memory Associations (verbatim):**
> "Whenever a memory is created, Asana creates 'Memory Associations,' essentially references to the Work Graph objects that the memory is about or relevant to. In their data model, memory is a concrete object with content, metadata, and associations. A Memory Association captures a Work Graph Object that the memory is about or relevant to. This allows them to explicitly contextualize a memory in the broader Work Graph, rather than having memories be untethered."

**Two retrieval lanes:**
- Broad working set of likely-relevant knowledge (default)
- Contextual retrieval during execution: "When a Teammate reads a specific task, project, or other object, it also receives memories associated with that object"

### Governance, human-in-the-loop (verbatim)
- "Claude cannot act autonomously within Asana — every consequential action requires explicit user approval"
- "AI actions — from drafting project plans to summarizing risks — has a human in the loop to course correct, check quality, and ultimately give final sign-off"
- "Users review and approve before tasks are created and projects are built"

### Inspectable memory (verbatim)
- "Users should be able to view the memories a Teammate holds, and delete memories that may be inaccurate or stale"
- "When a Teammate executes, the system can show which memories were passed into the execution context and which were created over the course of the execution"
- "Instead of asking 'why did the AI do that?' in the abstract, a user can trace the behavior back to a specific learned instruction, resource memory, or associated context object"

### Strategic framing (verbatim, from Claude launch)
> "An LLM in isolation is context-starved. It knows how to write, but it doesn't know your business — your goals, your knowledge, your specific approvals, or your historical relationships. Asana provides the scaffolding — the Work Graph data model — that grounds those external models in the reality of how your company actually operates."

> "Asana AI Teammates — built on the Work Graph, so they understand who is doing what, by when, and why — can flag that three teams are behind on dependencies for a launch and draft a mitigation plan."

### Production results (verbatim)
- 200+ organizations in beta program
- **93% of AI Teammates were granted full edit access, not view or comment only**
- Teams finished work 2× faster
- Tasks managed by collaborative AI Teammates: 3.2× more likely to have a clear owner, 2.6× more likely to have a defined deadline
- At launch: 21 out-of-the-box agents for Marketing, IT, Ops + no-code custom builder

---

## 4. asana.com/whats-new

### Winter 2026 Release (Q4 • FEB)

**1. Prebuilt AI Teammates**
- "Accelerate complex work with prebuilt AI Teammates"
- Includes: Campaign Brief Writer, Workflow Optimizer, Compliance Specialist, and more
- Marketing-focused gallery: Competitive Market Researcher, Creative Spec Writer, Launch Planner, Copywriter, and Campaign Brief Drafter

**2. AI Studio + Slack Integration**
- "Automate intake and manage work requests directly from Slack with AI Studio."

**3. Smart Fields / Custom Fields for Goals**
- "Organize, track, and report on goals more effectively with improved custom fields for goals."
- "Capture and report on robust data across projects with expanded custom field limits."

**4. Portfolio-Based Project Access**
- "Standardize project setup and permissions using shared project access with portfolios."

**5. Rule Builder Enhancements (Automation)**
- "Manage complex rule logic more easily with enhancements in the rule builder."
- "Duplicate existing rules" within and across projects

**6. AI Model Selection**
- "Build rules that work best for you using the automatic AI model selection."

**7. Asana Gov**
- "Stay secure and compliant with Asana Gov"
- For government agencies needing compliance, scalability, and easy implementation

### Not in Winter 2026 release on the page
- Smart Workflow Gallery (separately featured)
- Work Graph (it's a substrate, not a feature)
- AI risk reports (separately featured)
- No prior quarterly releases (Fall 2025, Summer 2025) detailed

---

## 5. Earnings + financial context

### Q4 FY26 earnings (March 2026)

**Dan Rogers (CEO) quotes:**
- "FY26 was a year of meaningful progress as we advanced Asana into a multi-product platform and strengthened our position as the foundational system of action layer for the Agentic Enterprise."
- "The expected launch of AI Teammates later this quarter marks the next phase of our AI platform, embedding agents directly into the coordinated flow of work."
- Asana launched AI Studio and introduced AI teammates "as part of a strategy aimed at what he called the 'agentic enterprise,' where humans and AI agents coordinate together"

**GA timeline locked in:**
- AI Teammates onboarded **more than 200 customers into a beta program**
- Generally available to **sales-led customers by end of Q1 FY27**
- **Self-serve customers in the second half of the year (H2 FY27)**

**FY27 guidance (locked-in numbers):**
- **$850M–$858M revenue** target
- **≥9.5% non-GAAP operating margin**
- **AI products targeting 15% of net new ARR**
- **AI Teammates reaching general availability for sales-led customers by end Q1 FY27**
- **$200M in active buyback capacity**

### Q3 FY26 earnings (December 2025)

**Dan Rogers quotes:**
- "Q3 revenues were $201 million, growing 9% year-over-year, exceeding the high end of our guidance"
- AI Teammates announced as "collaborative agents with the context, checkpoints and controls to execute complex tasks alongside humans, boosting team velocity and work quality"
- "Early customer adoption of AI Studio and AI teammates contributed to record-high retention, helped with renewal conversations, and drove productivity gains"
- Beta feedback and new customer expansions noted as positive indicators
- Raised full-year revenue and operating income guidance

### Stock context
- **ASAN down ~50% in 2026** (per TIKR / public analyst coverage)
- **Down ~92% from all-time highs**
- Market pricing in AI-disruption risk — assumes startups replace Asana with AI-native PM
- AI Studio + AI Teammates GA is the catalyst for re-rating

### Q3 FY26 detail (UC Today + Seeking Alpha context)
- Earnings exceeded forecasts despite surprise executive resignations
- Raised FY 2026 guidance amid 9% revenue growth

### Early customer results from earnings call
- **Morningstar** completed two-week tasks in 10–12 hours using AI teammates
- Management launched 12 AI teammates at one point — prebuilt collaborative agents for engineering, IT, marketing, operations, and PMO (later expanded to 21)

### Initial GA communication (September 2025)
- Initially communicated: "general availability for all AI Studio users will follow at the start of 2026"
- AI teammates with its own credit allocation separate from existing AI Studio rules
- Timeline later refined to Q1 FY27 (sales-led) and H2 FY27 (self-serve)

---

## 6. Pricing + AI Studio credits

### Base plan tiers (2026)
| Plan | Price | What's included |
|---|---|---|
| Personal | Free | No AI |
| Starter | $10.99/user/mo annual ($13.49 monthly) | AI Studio Basic + 50K credits/mo, Timeline, automation |
| Advanced | $24.99/user/mo annual ($30.49 monthly) | + portfolios, Goals, analytics |
| Enterprise / Enterprise+ | Custom (sales-led) | Full AI suite + AI Teammates GA at Q1 FY27 + AI Studio Pro |
| Asana Gov | Custom (sales-led) | US gov cloud, Winter 2026 release |

### AI Studio tiers
| Tier | Credits | Pricing | Available on |
|---|---|---|---|
| Basic (included) | Rate-limited; Starter gets 50K/mo | Bundled in plan | Starter+ |
| Plus (add-on) | **100K credits/month** | ~$150/seat/mo (per forum) | Advanced+ |
| Pro (sales-led) | **5M credits/quarter** | Custom, annual billing | Enterprise+ |

### How credits work
- "AI Studio Basic provides included access to AI Studio to explore how AI can help take on routine, manual work (includes rate limits)"
- Credits are sold as add-ons; pricing depends on plan
- "Credit consumption depends on which model (OpenAI GPT vs Anthropic Claude) is selected for each workflow"
- "Asana describes credits as being derived from the token volume processed by the selected model"
- "Different models consume credits at different rates"
- "Plus is sold as a fixed-price add-on that includes 100K credits per month"
- "Pro is a sales-led tier that includes 5M credits per quarter"

### Real-world credit burn (community-reported)
- "Each person uses 200K credits per month" — exceeds AI Studio Plus's 100K monthly inclusion
- "When credits run out, AI Studio rules can stop working — the smart layer simply goes dark until the meter resets or you top up, which is why teams end up having to monitor usage once AI Studio becomes operational"

### Multi-model support (verbatim)
- "Asana explicitly supports both OpenAI and Anthropic models (so, GPT-family and Claude-family options), and credit multipliers vary by model"
- Winter 2026 release: "Build rules that work best for you using the automatic AI model selection"

### Strategic takeaway (per analysts)
- "Starter sells 'automation' as table stakes; AI Studio sells 'smart automation' as a metered utility, with plan-tiered capacity and paid top-ups"
- "Because credit consumption depends on which model (OpenAI GPT vs. Anthropic Claude) is selected for each workflow, teams running AI Studio at scale should benchmark model choice against credit burn rates"

---

## 7. Asana Gov

### Winter 2026 launch
- Announced as part of Winter 2026 release (Feb 2026)
- "Stay secure and compliant with Asana Gov"
- "Positioned for government agencies needing compliance, scalability, and easy implementation"

### What's NOT publicly disclosed
- Specific FedRAMP impact level (Low / Moderate / High)
- DoD Impact Level (IL2 / IL4 / IL5)
- StateRAMP authorization status
- Data residency specifics for government tenants

### Federal AI context (relevant to Asana Gov positioning)
- White House released National Policy Framework for AI on March 20, 2026 (non-binding)
- NIST AI Risk Management Framework "rapidly becoming the de facto standard"
- GSA published AI compliance plan
- State-level AI legislation accelerating — 45 states introduced 1,561 AI-related bills as of March 2026
- Multiple compliance-grade state laws have effective dates in 2026

### Strategic implication
- Asana Gov + AI Teammates = the play for Fortune 500 + government AI workflow transformation
- Where Plane targets regulated via self-host OSS, Asana targets regulated via vendor-cloud certification + governance posture

---

## 8. Open questions / gaps

1. **Asana MCP server** — conspicuously absent from /product/ai. Every other PM competitor (Linear, ClickUp, monday, Notion, Plane, Jira) has a named MCP endpoint. Worth verifying with a live workspace whether Asana has shipped one or plans to.
2. **Asana Gov FedRAMP/DoD certification level** — not publicly disclosed at the marketing-page level. Worth a procurement-channel inquiry.
3. **AI Teammates Q1 FY27 GA confirmation** — projected for ≈ May 2026. Watch Q1 FY27 earnings (≈ Aug 2026) for the confirmation event.
4. **Self-serve GA timing in H2 FY27** — exact month not announced. "Second half of the year" is the management framing.
5. **Specific model versions in use** — Asana cites Claude and GPT but no public confirmation of Claude Sonnet 4.5 vs 4.7 or GPT-5 vs 5.2.
6. **Where does the 21 number come from?** — Marketing says 21 prebuilts. My count (7 Marketing + 6 Ops/PMO + 5 IT + 3 Product/Eng + Time Tracker) = 22. Possibly Time Tracker is one of the named Product/Eng ones or Asana counts differently.
7. **Asana Forum + Help Center release notes** — couldn't retrieve full content from the help center (CSS error / nav-only page). Discourse forum JSON at /58.json + /59.json would be the way to get monthly release notes in detail.
8. **Custom Teammate pricing** — unclear whether custom Teammates consume different credit rates than prebuilts.
9. **Credit consumption per Teammate run** — no public rate card. "Variable based on model + token volume" is what we have.
10. **Anthropic as customer logo** — Anthropic is listed on /product/ai as an Asana customer. Worth a follow-up on what they specifically use Asana AI for (a strong reference signal).
11. **Long-term roadmap beyond AI Teammates** — Dan Rogers' "Agentic Enterprise" framing suggests more coming. What's next after Teammates GA?
12. **MS Copilot integration** — referenced in the original AI PM Competitor Research file as a Q1 2026 feature; not surfaced in current /product/ai content. Status?

---

## 9. Recommended screenshots

If you can capture from a live Asana workspace:

1. **AI Studio canvas** — building a triage workflow with AI nodes
2. **AI Studio credit dashboard** — usage by workflow in admin console
3. **AI Studio model selection** dropdown showing OpenAI/Anthropic toggle
4. **AI Teammates library** — the 21 prebuilts browse view
5. **AI Teammate role description** — e.g. Campaign Brief Writer with Skills listed
6. **AI Teammate connecting to a project** — permission scope setup
7. **AI Teammate executing** — the human-approval gate before consequential actions
8. **Memory inspection panel** — viewing what a Teammate has learned
9. **Memory Association** — a memory linked to specific Work Graph objects
10. **AI risk report** in a portfolio
11. **Smart Workflow Gallery** — prebuilt templates browse
12. **Asana Gov** sign-in / interface (if accessible)
13. **Slack AI Studio integration** — automating intake from Slack
14. **Custom Teammate builder** — no-code role creation flow
15. **Custom fields for Goals** — Winter 2026 release surface
16. **Rule duplication** in rule builder
17. **AI Connectors** setup — kicking off Asana project from OpenAI/Notion/Slack

---

*Last updated: 2026-05-15 — companion to `asana_ai_research.html`.*
