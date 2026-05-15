# Linear AI — Raw Research Notes

> Working notes collected for [linear_ai_research.html](linear_ai_research.html). Verbatim extracts from each source so you can dig deeper, verify quotes, or build follow-up docs without re-fetching.
>
> **Run date:** 2026-05-15
> **Method:** WebFetch + WebSearch. No Linear MCP / playwright access in this session.

---

## Table of contents

1. [linear.app/ai — feature inventory](#1-linearappai)
2. [linear.app/changelog — AI entries timeline](#2-changelog-entries-by-date)
3. [linear.app/now — strategic blog posts](#3-blog--now-posts)
4. [Developer docs — Agents, MCP, AIG](#4-developer-docs)
5. ["Issue tracking is dead" manifesto (full extract)](#5-issue-tracking-is-dead-mar-24-2026)
6. ["Self-driving SaaS" essay (full extract)](#6-self-driving-saas-oct-22-2025)
7. ["How we built Triage Intelligence" (eng deep-dive)](#7-how-we-built-triage-intelligence-sep-3-2025)
8. ["Our approach to building the Agent Interaction SDK"](#8-our-approach-to-building-the-agent-interaction-sdk-aug-1-2025)
9. [Customer stories — adoption signals](#9-customer-stories)
10. [Press coverage + community signals](#10-press--community)
11. [Open questions / gaps to close](#11-open-questions--gaps-to-close)
12. [Recommended screenshots to capture](#12-recommended-screenshots-to-capture)

---

## 1. linear.app/ai

### Features listed on the AI overview page

| Feature | Verbatim description | Surface | Plan / Status (per page) |
|---|---|---|---|
| **Triage Intelligence** | "Proactively suggests and applies assignees, teams, labels, and projects based on the team's historical issue patterns. Also detects duplicates and links related work. Provides reasoning for each suggestion (e.g., why a particular assignee or project was recommended) with alternatives." | Inline within Triage view — "Suggestions" panel alongside the issue with "Accept suggestion" action | CTA links to `/settings/product-intelligence`; specific tier not stated on page |
| **Linear for Agents / AI Agents** | "Build and deploy AI agents that work alongside you as teammates" — for collaborative or fully delegated work, including code generation and technical tasks | Agents act as teammates on issues | "ready to deploy"; no beta label |
| **Custom Agents (via Linear API)** | "Build your own AI teammates with the Linear API," kept private or shared with the Linear community | Developer / API surface | Not labeled |
| **Linear MCP** | Connects Linear to external AI tools such as Cursor, Claude, and ChatGPT via Model Context Protocol | External AI clients (chat / IDE surfaces outside Linear) | Not labeled |
| **AI-powered Search (Semantic Search)** | Semantic search across titles, descriptions, customer feedback, support tickets | Search interface (inline) | Not labeled |
| **Pulse Updates** | "AI condenses project and initiative updates into a daily or weekly summary, delivered to inbox as text or an audio digest" | Inbox (text + audio digest) | Not labeled |

### Positioning copy (verbatim quotes)

- "AI workflows for modern product teams"
- "Streamline your product development with Linear's powerful AI workflows. Purpose-built to help product teams move faster."
- "Self-driving product operations" (Triage Intelligence headline)
- "Tribal knowledge, made actionable."
- "AI that works where you work" — "From finding the right issue to staying on top of updates, AI is part of every workflow in Linear."
- "It works quietly in the background, so you can focus on building."
- "Delegate and automate work with AI agents" / "Scale output."

> **Note:** The specific phrase "designed for workflows shared by humans and agents" does **not** appear verbatim on linear.app/ai (despite being widely reported in the existing AI PM competitor research). The closest framing is agents working "alongside you as teammates."

### Data / Privacy stance (verbatim)

Under "Enterprise-grade security":
- "Everything in Linear is designed to keep your work safe and secure."
- "Your information is never used to train AI models and remains secure at every step."

### Pricing / Credits

- No explicit credit system, token pricing, or per-seat AI pricing on this page.
- CTAs: "Contact sales," `/signup`, `/settings/product-intelligence` ("Get started").
- General `/pricing` link in nav.

---

## 2. Changelog entries by date

### May 14, 2026 — Code Intelligence
- "Code Intelligence gives Linear Agent controlled access to your codebase, turning repositories into shared product context your whole team can use."
- "Code Intelligence is now available in public beta for Business and Enterprise plans, and free to use during the beta period."

Related fixes/improvements:
- Agent: "Fixed an issue where the agent chat could not be closed while an attachment modal was open"
- Agent: "Fixed natural-language confirmations in Slack threads being recognized while awaiting approval, even without an `@Linear` mention"
- Agent: "Linear Agent can now resolve and unresolve comment threads, including in automation flows triggered in triage"
- Agents: "Users can now queue follow-up messages while an agent is still working, and they'll send when the current turn completes"
- Issues: "Added a delegation footer to issue cards in AI chat showing the agent name and live status"
- Issues: "Added an animated desktop tab indicator for issues and pull request reviews when a coding agent is actively working"
- MCP server: `save_project` no longer accepts issue-level label IDs; added Slack/Teams channel ID fields; added `initiative` and `cycle` parameters to `save_document`; "Unknown tool parameters now return a validation error instead of being silently dropped"

### April 30, 2026 — Releases
- "Generate release notes with Linear Agent based on included issues."
- "Pressing Esc to dismiss an invalid mention search in an agent session no longer leaves a stranded popover backdrop"
- "Fixed the copy table action in agent chat responses"
- "Fixed agent-generated content mixing placeholder and normal text when editing issues, documents, and projects created from templates"
- Linear Agent: "Added 'New agent chat' to the right click menu on the Create button in the sidebar"
- Linear Agent: "Linear agent is now able to work with issue drafts"
- MCP server: link handling improved so URLs "create rich attachments and trigger two-way sync instead of being stored as plain URL attachments"

### April 23, 2026 — Linear Agent MCP support
- "Linear Agent can now connect to your tools via MCP, giving it access to data and actions beyond your Linear workspace."
- Examples cited: Granola, Glean, Notion, PostHog
- "Admins can control access with allowlists and workspace-level MCP permissions."
- "Select text anywhere in Linear and press ⌘J to send it directly to the agent as context"
- "Agent chat now opens in a maximized overlay, so it feels like a natural extension of the toolbar chat instead of a separate page"

### April 16, 2026 — Linear for Microsoft Teams
- "Mention **@Linear** in any Microsoft Teams channel to turn your conversations into actionable work."
- "Custom coding tool integrations let you open issues in tools that aren't supported out of the box."
- "Now you can sync an issue to multiple Slack threads when there are multiple reports or requests for the same issue."
- Triage Intelligence: "Fixed label filters in Triage Intelligence settings not showing team-specific labels"
- MCP server: "Fixed an issue where MCP OAuth connections could disconnect after ~1 day"

### April 9, 2026 — Multi-level sub-teams
- Project/initiative comments: "capture meeting takeaways and mention @Linear to update docs, revise descriptions, and create issues"
- "You can now search past agent chats from the Cmd/CtrlK menu"
- "Agent no longer asks for confirmation on routine bulk updates of up to 5 issues"

### April 2, 2026 — Web forms for Linear Asks
- Submissions can be "routed with Triage Intelligence"
- "Linear Agent can now reorganize issue and project labels"
- "Dragging files anywhere onto the agent chat window now triggers file upload"
- "Chats can now be copied as markdown"
- "Added ability for Linear Agent to delete customers"
- "My Issues, Inbox, Reviews, Pulse, and team views can now be included as context for Linear Agent"
- "Improved recognition of natural-language delegation prompts in Slack (e.g. '@Linear work on this', '@Linear go')"
- Deeplinks: "Run a custom local script when opening issues in coding tools"
- Deeplinks: "'Copy as prompt' now respects the 'move issue to started status' preference"
- MCP server: OAuth flow fixes; added removing issue relationships; "Updated ChatGPT app client ID for search and fetch tools"; added `trashed` field

### March 24, 2026 — Introducing Linear Agent (🚀 MAJOR LAUNCH)
- "Linear Agent brings all of that context within reach."
- "Built directly into Linear, and accessible everywhere, Linear Agent understands your roadmap, issues, and code."
- "Linear Agent is powered by frontier language models and fully grounded in the context of your workspace."
- Skills: "When a conversation gets you to a good result, you can ask Linear to save it as a reusable skill."
- Automations: "You can also trigger agent workflows automatically when issues enter triage."
- Code Intelligence (preview): "extends Linear Agent's understanding to your codebase"
- Availability: "Linear Agent is now available in **public beta** for all teams."
- MCP server: added pagination to `list_comments`; initiatives now accept multiple parent initiatives
- Keyboard shortcuts: "Cmd/Ctrl J now opens Linear Agent"

### March 12, 2026 — UI refresh
- Added launchers for "Amp, Codex CLI, Devin, Factory, Lovable, Netlify Agent Runners, Warp, Windsurf"
- Mobile agent sessions: "After delegating an issue to an agent, open its session in the Linear mobile app to see realtime reasoning"
- "Linear Agent now respects the Slack channel's synced team context when fetching project updates"
- "Improved automatic issue self-assignment on move to started state for API-driven changes"
- "Fixed editor toolbar appearing below the agent session panel"

### February 26, 2026 — Deeplink to AI coding tools
- "You can now launch your preferred coding tool directly from a Linear issue, with a prefilled prompt that includes the issue ID and all relevant context"
- Supported: "Claude Code, Codex, Conductor, Cursor, GitHub Copilot, OpenCode, Replit, v0, Zed"
- "Prompt templates can also be customized to add standing instructions"
- Notion: "Create and update Linear issues and projects using Notion's new Custom Agents."
- "Fixed agent sessions remaining associated when an issue is archived, allowing them to be restored along with the issue"
- "Thought items in the session sheet now render as full rich text instead of a single truncated line"
- MCP server: added SLA status to issue responses; improved parent labels support; filter issues without assignee; "Combined `create_issue` and `update_issue` tools into a single `save_issue` tool"; project lookup by slug

### February 13, 2026 — Advanced filters
- "use _AI filter_ to describe what you're looking for in natural language"
- Gemini Enterprise: "Gemini Enterprise users can now create issues from Gemini, and access data from their existing issues and projects."
- "Linear Agent for Slack can now add images from a conversation to existing entities"
- Triage Intelligence: "Issue suggestions popover now shows created/completed timestamps to help identify older issues that may be less relevant"
- MCP server: "Added project resources to MCP responses"; "Added the ability to list project members"

### February 5, 2026 — Linear MCP for product management
- "We've expanded Linear's MCP server with support for initiatives, project milestones, and updates."
- New tools: create/edit initiatives, initiative updates, project milestones, project updates; manage project labels; image loading
- "Better tool docs reduce token usage"
- URL-based resource loading; `/sse` endpoint deprecated in favor of `/mcp`
- Email intake: "Email intake now handles emails with empty or missing subjects by generating AI-powered titles"
- API: OAuth app agents no longer auto-become delegated agent on status changes to Started/Done

### January 29, 2026 — Time in status
- MCP: `update_issue` allows `assignee` / `delegate` set to null; `update_project` allows `lead` set to null

### January 22, 2026 — Customize navigation in Linear Mobile
- **Linear Code Reviews (Private Beta):** "We've brought code reviews directly into Linear, with support for both traditional PR workflows and agents output."
- Agents: no assignment to inactive users; layout-shift fix; overflow fix for long inline code
- API/Agents: `AgentActivityWebhookPayload.userId` now non-nullable; `AgentSession.type` deprecated; new `user` object in webhook payload; new `issueRepositorySuggestions` query for "confidence-ranked list of repos associated with an issue or agent session"; `AgentSession.url` added
- MCP server: Issue relations support (blocking/related/duplicate); add/remove projects from initiatives; new `create_document` / `update_document` tools
- "Agent thoughts use full panel height"

### December 17, 2025 — Team owners
- **v0 by Vercel MCP connector:** Pull context from Linear into v0 for prototypes/dashboards
- Agents: Visual improvements to "better surface responses, highlight associated pull requests, and automatically collapse agent thoughts after work completes"
- API/Agents: New `promptContext` field on `AgentSessionEvent` "created" webhooks containing issue details, comments, and guidance
- MCP server: Add/remove issues from project milestones; labels include group info; project icon/color in `create_project` / `update_project`; optional team filtering on `list_users`

### December 11, 2025 — Linear agent for Intercom, Zendesk, Gong
- "The Linear agent can now handle the tedious work of turning customer conversations into actionable issues."
- Gong: "fully self-driving issue creation workflow to customer calls"
- Triage intelligence: "duplicate requests are automatically merged into existing issues"
- Linear agent in Slack workflows: Agent can now be invoked by automated steps in Workflow Builder
- Warp agent: Delegate issues to Warp agent; it "will create a plan and start working on implementing it"

### December 4, 2025 — OpenAI Codex agent
- "OpenAI Codex users can now delegate issues directly to the Codex agent without leaving Linear."
- Codex chooses repo, answers codebase questions, fixes bugs, handles triage
- Supports parallel execution across multiple issues; inbox notifications on completion / input needed
- Agents: Archiving an agent's only session on an issue removes that agent as delegated; agent session links unfurl in Slack
- Security: New setting to control who can modify workspace-level agent guidance prompts
- Fixes: Webhook payload stripping image attachments fixed; private team webhooks not firing for agents fixed

### November 20, 2025 — Form templates
- **Figma Make connector:** "Access Linear issues, projects, and documents from Figma Make"; all MCP server tools accessible via connector

### November 13, 2025 — Pulse on mobile
- Datadog integration: Auto-create Linear issues from Datadog monitor notifications

### October 28, 2025 — GitHub Copilot agent
- "GitHub Copilot users can now work with the GitHub Copilot agent directly within Linear."
- Delegate or @mention; agent uses full issue context to open a draft PR
- Track delegated issues via My Issues or custom views with `Agent = GitHub Copilot` filter

### October 23, 2025 — Linear agent for Slack
- "Mention @Linear in discussions on Slack, and the Linear agent will create issues informed by your conversation's context."
- Available on all plans
- Triage Rules: configurable to move issues to triage of the same team

### September 18, 2025 — Auto-apply triage suggestions (+ Triage Intelligence rename)
- Banner: "This feature has been renamed to **Triage Intelligence**"
- "take the first pass at triage and automatically apply suggestions to issues"
- Configurable rules: e.g., always auto-apply suggested team/assignee, but only auto-apply specific labels like `bug`
- Auto-applied properties marked in suggestions header; hover reveals reasoning
- Available in Technology Preview on Business and Enterprise plans
- OAuth: short-lived 24-hour access tokens paired with refresh tokens; new OAuth apps issue refresh tokens by default starting Oct 1, 2025; existing apps must migrate by April 1, 2026; added `client_credentials` grant support
- API: new `semanticSearch` query that "can search multiple item types at once"

### September 4, 2025 — Salesforce integration
- Agents: Session created when an issue is delegated to an agent even if no human actor/assignee
- iOS: improved visibility of workspace-level agents in assignee picker
- Mobile: agent status shown in inbox when agent replies in a thread
- PR reviews: improved performance on PRs "with a lot of comments from AI agents"

### August 21, 2025 — Cursor background agents
- Add Cursor as an agent in workspace; delegate issues so Cursor "will use the full issue context to create a plan and start working on an implementation"
- Cursor "will automatically create a branch, draft a PR, and notify you when the work is ready"
- Non-engineers can use it for prototypes, UI fixes, copy updates
- Initiative views: curated, shareable lists of initiatives (Enterprise plans)
- Triage Rules can now add issues to projects

### August 14, 2025 — Product Intelligence (Technology Preview) — ORIGINAL LAUNCH
- Banner: "This feature has been renamed to **Triage Intelligence**"
- "Product Intelligence streamlines your product operations with AI assistance for routine, manual tasks"
- "automating the overhead of triage intake"
- "examines all issues sent to Triage and does the tedious parts of the intake process for you"
- Researches past/existing issues for context; suggests team, projects, assignee; "identifies related issues and likely duplicates"
- Users can accept/dismiss suggestions or hover to see reasoning
- Optional additional guidance can be added at workspace, team, or sub-team levels
- Available in Technology Preview on Business and Enterprise plans
- **Mobile new search:** uses "hybrid semantic search engine"; surfaces recently viewed items; press Enter to search all issues/projects/documents
- Customize Asks email auto-replies
- Attio integration — sync customer details and feedback
- Linear for Agents: "Agent session threads now support resolution and subscriptions, much like regular comment threads"
- Issues: "Going forward, an issue's assignee will always be subscribed to the issue"
- Mobile: added support for issue delegation to agents
- Notifications: subscribers no longer auto-subscribed to comment threads used for agent interaction "to reduce spam"
- MCP server: issue properties (labels, project, status) "can now be modified and queried by name rather than UUID"; added `query` parameter to `list_users`; pagination for `list_issue_labels`; tool annotations exposed
- API/OAuth: `initiative:read` / `initiative:write` and `customer:read` / `customer:write` scopes available with `actor=app`
- Webhooks: `AppUserNotification` returns `OAuthClient` `clientId` in `oauthClientId` field

### July 30, 2025 — Agent Interaction Guidelines and SDK
- **Agent Interaction Guidelines (AIG):** framework distilled from learnings with agent partners; "principles and practices help developers design agents that integrate more naturally into human workflows"; described as a living document
- **Agent Interaction SDK (Developer preview):** structured way to define how agents communicate status/progress; Linear renders UI automatically
- **Agent Delegation:** "When a user delegates an issue to an agent, the user remains the primary assignee, while the agent is added as a contributor"
- **Agent Session:** rich status — actively working, waiting for input, error, or completed
- **Agent Activity:** exposes reasoning steps, tool usage, clarification prompts, final responses
- MCP server: "More cycle details are now returned in `list_cycles`"

### July 24, 2025 — Dashboards
- **Notion AI Connector:** "Search across Linear projects and issues directly from Notion AI"; access to titles, descriptions, assignee, creator, comments
- MCP server: added pagination to `list_issues`; "Replying to comment threads is now supported"; fixed truncated text content

### July 17, 2025 — Email intake for Linear Asks
- MCP: "Included `Issue.delegate` in MCP tools"
- MCP: "Made LLM aware of multiple pages of responses"
- API: added `fromDelegate` and `toDelegate` fields to `IssueHistory`

> **Gap:** Changelog entries prior to July 17, 2025 were not fetched. Worth pulling later if researching pre-Product-Intelligence history.

---

## 3. Blog / Now posts

### Karri Saarinen's strategic essays (Linear Now blog)

| Date | Title | URL | Strategic theme |
|---|---|---|---|
| 2026-05-14 | Code Intelligence for Linear Agent | `/now/code-intelligence-for-linear-agent` | Agent reads codebases as shared context |
| 2026-04-17 | Output isn't design | `/now/output-isn-t-design` | Pushback on "AI = output" framing; protect craft & intent |
| 2026-04-10 | How we use Linear Agent at Linear (Rhea Purohit) | `/now/how-we-use-linear-agent-at-linear` | Internal dogfooding across CX/Product/Eng |
| 2026-03-24 | Issue tracking is dead | `/next` | The big repositioning manifesto |
| 2025-12-19 | Design is more than code | `/now/design-is-more-than-code` | When execution becomes default, "why" devalues |
| 2025-10-22 | Self-driving SaaS | `/now/self-driving-saas` | Three autonomy levels framework |
| 2025-09-03 | How we built Triage Intelligence | `/now/how-we-built-triage-intelligence` | Engineering deep-dive on the ML architecture |
| 2025-08-21 | How Cursor integrated with Linear for Agents (Kevin Hartnett) | `/now/how-cursor-integrated-with-linear-for-agents` | Validation of Agent Interaction SDK |
| 2025-08-01 | Our approach to building the Agent Interaction SDK (Leela Senthil Nathan) | `/now/our-approach-to-building-the-agent-interaction-sdk` | Platform philosophy |
| 2025-07-16 | Inside Mercury's six-month journey building with AI agents (Kevin Hartnett) | `/now/mercury-linear-ai-agents` | Longitudinal customer adoption |
| 2025-04-07 | Design for the AI age | `/now/design-for-the-ai-age` | Early philosophical groundwork |

### Karri Saarinen's X/Twitter signal

- Feb 12, 2026 — preview of Linear Agent launch: "Linear Agent is in Linear next. Think AI PM + AI triage and backlog grooming. Deeper integrations with coding agents, workflows, and tools (MCP, etc.)."
- URL: https://x.com/karrisaarinen/status/2022031620166103237

---

## 4. Developer docs

### Agents (`linear.app/developers/agents`)

**Auth model:**
- OAuth 2.0 with `actor=app` query parameter
- `actor=app` replaces older `actor=application`
- Requires admin permissions (workspace-scoped install)
- Apps using `actor=app` cannot also request `admin` scope

**Optional scopes:**
- `app:assignable` — allow assignment as delegate on issues and project membership
- `app:mentionable` — allow @mentions in issues, documents, editor surfaces
- `customer:read` / `customer:write`
- `initiative:read` / `initiative:write`

**Delegation:**
- Assigned to an agent → agent becomes `delegate`, not `assignee`
- "Humans maintain ownership while agents act on their behalf"

**Identity / Install:**
- Each workspace install produces a unique app ID per workspace
- Retrieve with:
  ```graphql
  query Me { viewer { id } }
  ```
- Linear recommends storing this ID alongside the access token

**Webhooks:**
- Enable in app config under "Agent session events"
- Additional categories: Inbox notifications, Permission changes (sends `PermissionChange` webhook when team access is modified)

**Agent Session lifecycle:**
- Central interaction primitive — tracks lifecycle of a given agent task
- Auto-created on @mention or delegation — no manual state management
- First webhook: `created` `AgentSessionEvent` with `agentSession` object (issue, comment, context)
- On receiving: emit a `thought` activity within **10 seconds** to acknowledge
- Use `promptContext` field to build a formatted string of session context (issue details, comments, guidance)

**Status:** Linear for Agents APIs in **Developer Preview** — APIs may change before GA.

### Developer surface map (`linear.app/developers`)

**Agents cluster:**
- `/developers/agents` — Getting Started
- `/developers/aig` — Agent Interaction Guidelines (Principles and practices for designing agent interactions)
- `/developers/agent-interaction` — Developing the Agent Interaction
- `/developers/agent-best-practices` — Interaction Best Practices
- `/developers/agent-signals` — Signals

**GraphQL API:**
- `/developers/graphql` — Getting started
- `/developers/pagination`
- `/developers/filtering`
- `/developers/rate-limiting`
- `/developers/deprecations`
- `/developers/webhooks`
- `/developers/attachments`
- `/developers/managing-customers`
- External schema reference: https://studio.apollographql.com/public/Linear-API/schema/reference?variant=current

**Authentication:**
- `/developers/oauth-2-0-authentication`
- `/developers/oauth-actor-authorization` — for apps/agents acting on behalf of users
- `/developers/file-storage-authentication`

**TypeScript SDK:**
- `/developers/sdk` — Getting started
- `/developers/sdk-fetching-and-modifying-data`
- `/developers/sdk-errors`
- `/developers/advanced-usage`
- `/developers/sdk-webhooks`
- `/developers/migrating-from-1-x-to-2-x`
- GitHub: https://github.com/linear/linear/tree/master/packages/sdk
- Sample agent: https://github.com/linear/weather-bot (TS SDK + Cloudflare)

**Guides:**
- `/developers/how-to-upload-a-file-to-linear`
- `/developers/create-issues-using-linear-new` — linear.new URL trick
- `/developers/integration-directory`
- CLI importer: https://github.com/linear/linear/tree/master/packages/import

> **Gaps in fetched developer docs:** No standalone MCP documentation page surfaced (URLs `developers.linear.app/docs/mcp` and `linear.app/developers/mcp` both 404 / redirect). The MCP details come from changelog entries instead. The Code Intelligence API doc was not fetched.

---

## 5. "Issue tracking is dead" (Mar 24, 2026)

**URL:** https://linear.app/next
**Author:** Karri Saarinen

### Core thesis
- "Issue tracking is dead."
- Argument: trackers emerged from a handoff model — PMs scoped work, engineers picked it up later, workflows bridged the gap.
- "Complexity started to look like sophistication" and "the process became the work."
- Linear's founding belief: "the best systems remove overhead so teams can focus on building."

### On AI Agents
- Agents are an accelerant of simplification, not just another tool.
- Agents are absorbing procedural work across planning, implementation, and code review, letting people "spend more time on intent, judgment, and taste."
- **Adoption metrics quoted in the essay:**
  - Coding agents installed in "more than 75% of Linear's enterprise workspaces"
  - Agent work volume grew **5×** in three months
  - "Agents authored nearly 25% of new issues"

### Context as the organizing principle
- "The next system is not designed around handoffs. It is designed around context and agents."
- "Agents are not mind readers. They become useful through context" — feedback, ideas, strategy, decisions, and code must live in one shared system.

### Linear's positioning
- "Linear is the shared product system that turns context into execution."
- It "holds feedback, intent, decisions, plans, and code, shapes that context into work, and helps humans and agents carry it all the way to production."

### Human–agent relationship
- Not full autonomy — orchestration.
- A system that should "understand intent, route work to the right actor, escalate when needed, and keep execution moving."
- Humans retain judgment; agents handle mechanics.

### Concrete features launched alongside the manifesto
- **Linear Agent** — native interface to analyze feedback and craft projects, issues, and documents
- **Skills** — codified reusable workflows, triggered via slash commands or automatically
- **Automations** — starting with Triage, firing agent workflows on issue entry

### Coming soon (as of Mar 24, 2026)
- **Code Intelligence** — codebase understanding, Q&A, debugging (shipped May 14, 2026)
- **Code Diffs** — review interface "built for both humans and agents to iterate together"
- **Linear Coding Agent** — writes code and fixes bugs using frontier models plus Linear context

### Closing frame
- "Collapsing the distance between an idea and its implementation."

> **Note:** The manifesto doesn't explicitly use "self-driving software" — that framing is in the earlier "Self-driving SaaS" essay.

---

## 6. "Self-driving SaaS" (Oct 22, 2025)

**URL:** https://linear.app/now/self-driving-saas
**Author:** Karri Saarinen

### Core thesis
- Traditional business software is fundamentally limited — value depends on effort users invest.
- AI chatbots layered onto existing apps = "the old ways of working dressed in a new interface."
- Real breakthrough: software stops waiting for input and proactively advances work itself.

### Three levels of autonomy

| Level | Verbatim framing | Linear equivalent |
|---|---|---|
| **Basic (assistive)** | "The system suggests actions — recommending teams to assign issues to or labels to apply, similar to a lane-departure warning" | Triage Intelligence suggestion view |
| **Moderate** | "auto-apply[s] suggestions selectively," with AI actions clearly identified so they can be reversed | Auto-apply rules (Sep 2025) |
| **Full autonomy** | "You can take your hands off the controls entirely and the system drives the work from start to finish," with humans involved only to evaluate final results | Gong "self-driving issue creation"; Automations end-to-end |

- Critical preserved agency: "you decide which projects to pursue and where to allocate your resources — but the system moves everything forward on its own"
- Not a switch-flip: "capabilities and culture both need to progress"

### Three concrete automation areas named
1. **Customer request extraction** — Pulling requirements automatically from support tickets, customer research, and sales calls
2. **Issue routing** — Newly created issues "automatically assigned to the correct team, project, and person" using completion history, backlog, and roadmap as context
3. **Coding agent dispatch** — "Simple changes are dispatched to a coding agent and completed without additional intervention," while complex work is collated into living project specs

### Quoted product implication
- "We've already started to build and release features to make this a reality. Like with self-driving cars, they can be adopted and operated at different levels of autonomy."

### Building blocks (page footer surfaces)
- Intake, Plan, Build, Agents, Customer Requests

---

## 7. "How we built Triage Intelligence" (Sep 3, 2025)

**URL:** https://linear.app/now/how-we-built-triage-intelligence
**Authors:** Yann-Edern Gillet, Matthijs Wolting

### Architecture overview
- Combination of "search, ranking, and LLM-based reasoning to make suggestions as new issues come in."

### Retrieval layer
- Linear rebuilt search infrastructure earlier in 2025
- Transition: "from a basic keyword-based system to a more general-purpose semantic backend"
- "Already surfacing similar issues using vector search and semantic similarity," then unified retrieval across product
- Semantic search produces candidate issues from backlog → fed into LLM stage

### Model choice & evolution

**First version:**
- "GPT-4o mini and Gemini 2.0 Flash"
- "Tightly scoped prompts and rigid workflows"
- "Could only work with the information we provided up front"

**Current version:**
- "Switched to larger models like **GPT-5 and Gemini 2.5 Pro**, which could handle more complexity in both inputs and reasoning"
- Agentic — agent pulls additional context from Linear's data on demand instead of relying solely on prompt-stuffed context

### Suggestion generation
- Candidate set from search "became the input to our LLMs, which would evaluate each incoming issue and decide whether it was a duplicate, loosely related, or unrelated"
- Beyond duplicates: assignees, labels, projects, related issue links — each with reasoning

### Reasoning transparency UI patterns
- Hover on suggestion → plain-language rationale + alternatives
- "Thinking state" indicator with a timer shows live progress
- Thinking panel shows "the full trace of the model's research: the context it pulled in, the decisions it made, and how additional guidance shaped the outcome"

### Steering model
- **Not** a feedback loop on accept/dismiss
- **Instead:** "Additional Guidance" setting where workspace or team admins write natural-language prompts to steer suggestions
- Article does not describe an automated learning loop

### Latency tradeoff (quoted)
- "If something takes more than a few hundred milliseconds, we try to make it faster"
- Frontier reasoning models are "fast compared to a human, but slower than Linear's usual deterministic systems"
- This drove the progress-indicator UI patterns

### Data used
- Backlog itself is the dataset — "your existing backlog as a data set to understand how similar work has been organized in the past"
- Plus workspace context the agent retrieves during reasoning

### Roadmap (as of Sep 2025)
- Opt-in auto-application of trusted suggestion types (assigning, labeling, routing) — shipped Sep 18, 2025
- Extending LLM use to drafting project and initiative updates — partially shipped via Linear Agent

### Notable omission
- **No quantitative accuracy claims** — no benchmarks, evals, or precision/recall figures

---

## 8. "Our approach to building the Agent Interaction SDK" (Aug 1, 2025)

**URL:** https://linear.app/now/our-approach-to-building-the-agent-interaction-sdk
**Author:** Leela Senthil Nathan

### What the SDK is
- Framework for integrating AI agents as native participants in Linear workspace
- Provides primitives: authenticate, receive work, communicate, surface reasoning
- All while operating within the same product humans use
- Paired with **Agent Interaction Guidelines (AIG)** — design principles codifying Linear's philosophy

### Philosophy: "Flexible guardrails"
- Platform primitives and opt-in constraints that shape behavior without restricting agent capabilities

### Six core design principles (quoted verbatim)

1. "An agent should inhabit the platform natively"
2. "Agents should always disclose that they are agents"
3. "An agent should provide instant feedback"
4. "An agent should be clear and transparent about its internal state"
5. "An agent cannot be held accountable"
6. "Flexible guardrails"

### Why build it (vs. existing standards)
- No explicit comparison to MCP
- Linear reasoning: already positioned as "the orchestration layer where humans and agents interacted"
- Existing foundations: OAuth, scoped permissions, rich API
- Chose to extend native platform rather than retrofit external paradigms — "meet [teams] where they were"

### Surfaces and primitives exposed

**1. Agents as first-class users:**
- OAuth actor mode: `actor=app` creates a dedicated user representing the agent
- Each agent: own identity, token, scoped permissions, team access
- Workspace admins manage them like other users

**2. Opt-in scopes:**
- `app:assignable` — appear in assignment menus
- `app:mentionable` — respond to @-mentions in comments/documents

**3. Agent Session:**
- Abstraction representing an interaction (assignment, mention, trigger)
- When created, Linear sends structured webhook with context
- Agent responds to the session directly; Linear routes the response correctly

**4. Session status types:**
- *waiting for input*, *actively working*, *completed*, *errored*

**5. Agent Activity types** (being added):
- Tool calls
- Thoughts
- Elicitations

**6. Delegation (vs. assignment) — quoted:**
- "Issues can only be assigned to humans, and only delegated to agents"
- Every agent-involved issue retains a human assignee responsible for the outcome alongside the delegated agent
- Linear considered using sub-issues but found them "too independent"

### Evolution note
- First iteration mirrored a user's inbox via webhooks
- Pushed too much complexity onto developers — forcing them to reconstruct context themselves
- Agent Sessions emerged from observing what agents actually needed

### Relationship to MCP
- **Not mentioned in this post.** The post predates Linear's MCP server expansion.

---

## 9. Customer stories

| Date | Customer | URL | Strategic message |
|---|---|---|---|
| 2026-05-13 | Cars24 | `/customers/cars24` | "Cars24's push to being AI-native with Linear" — renewed Jira contract then walked away weeks later to go AI-native on Linear |
| 2026-04-27 | Ramp | `/customers/ramp` | "The coding agent behind 60% of Ramp's merged PRs" — Ramp's internal coding agent ships majority of merged PRs, with Linear "the underlying layer for structured product context" |
| 2026-03-26 | Coinbase | `/customers/coinbase` | "Coinbase's bet on agent-first development" — Base engineering asked to delete IDEs and write zero code for 2 weeks, forcing agent-first workflow |
| 2026-02-04 | Cursor | `/customers/cursor` | "How Cursor builds with Linear" — idea to open branch faster than most teams schedule a meeting |
| 2025-07-16 | Mercury | `/now/mercury-linear-ai-agents` | Six-month longitudinal journey of integrating AI agents at Mercury |

### Internal dogfooding
- 2026-04-10 "How we use Linear Agent at Linear" — workflows where the agent proved useful across CX, Product, and Engineering
- At Linear: "a coding agent takes a crack at reviewing every PR (for the past couple of months, they've been leaning on Codex for this), and then a human engineer makes the final approval. When the pull request is merged, the Github integration marks the related issue in Linear as 'Done'"

---

## 10. Press & community

### Press coverage of Linear Agent launch (Mar 24, 2026)

- **The Register** — "Linear adopts agentic AI as CEO declares issue tracking dead" (Mar 26, 2026) — https://www.theregister.com/2026/03/26/linear_agent/
  - "The Linear cloud issue tracker and project manager has introduced an AI agent and plans to add AI coding assistance"
  - "Linear is developing a proprietary coding agent that wraps existing agents like Devin and Cursor with deeper platform integration"
  - "In the company's Slack channel, customers were positive about the announcement, but asked for model context protocol (MCP) support. An employee responded that 'we're working on MCP support.'" (Resolved Apr 23, 2026 with Linear Agent MCP support)
- **TBPN Digest** — "Linear CEO Karri Saarinen declares 'issue tracking is dead' and reveals Linear's AI-era pivot"
- **DevClass** — "Linear moves sideways to agentic AI as CEO declares issue tracking dead"
- **Department of Product (Substack)** — "Linear says Issue Tracking is Dead" by Rich Holmes
- **Tessl** — "Linear CEO explains why the company is betting on agents"
- **Buttondown** — "The Death of the Ticket: Why Linear is Pivoting from Issue Tracking to 'Agent Management'"
- **Idlen** — "Linear Declares Issue Tracking Dead: AI Agents and Skills"

### Third-party reviews

- **Oflight Inc.** — "Linear AI Features Complete Guide — Agent, Triage Intelligence & Automation for Maximum Efficiency [2026]"
- **AI Tools HQ** — "Linear Agent Review 2026 — Features, Pricing & Alternatives"
  - "Linear Agent is the most practical implementation of AI agents in project management to date. Unlike standalone AI PM tools, it works within the tool teams already use, making adoption seamless."
  - Cites 80% reduction in time spent manually filing issues, 70% cut in triage time, "66% of Forbes-recognized AI companies rely on Linear for their engineering workflows"
- **SaaSCRMReview** — "Linear Review 2026: Pricing, Features, Pros & Cons"
  - Triage Intelligence (Business+) as "AI-powered routing and prioritization of incoming issues"
  - Linear Asks (Business+) as "an AI assistant for answering questions about your backlog and project status"
  - Business plan ~$10/user/month (conflicts with $16/user/month from AI Tools HQ)
- **aiinuse.org** — "Linear – Triage Intelligence for issue routing - AI in Use"
- **RelevanceAI** — "Linear AI Agent Templates"

### Pricing claims observed (need verification in live workspace)

- Business plan: $10–$16/user/month (sources conflict)
- Linear Agent + Skills: all plans including Free
- Triage Intelligence + Automations: Business+ only
- Code Intelligence: Business+ but free during public beta (started May 14, 2026)
- Future usage-based pricing: "High-volume compute capabilities like Automations and Code Intelligence may move to usage-based pricing beyond a certain threshold"

### Community sentiment summary

- Trust in Linear AI is the highest among PM tools per third-party reviews
- Attributed to "no model training on your data" policy and narrow, opinionated feature set
- Triage Intelligence suggestions "spookily accurate" after a few weeks
- Product Intelligence polarizing: "This is going to replace PMs" vs "AI can't know our business context"
- Developer community love unmatched
- Customer Slack-channel request after Mar 2026 launch: MCP support (granted Apr 2026)

---

## 11. Open questions / gaps to close

1. **Exact Business-plan price** — sources conflict ($10 vs $16/user/mo). Check live billing page.
2. **Linear MCP standalone documentation** — both `developers.linear.app/docs/mcp` and `linear.app/developers/mcp` returned 404. Linear may have inlined MCP docs into the agents cluster, or the canonical doc URL is different. Worth checking with Linear MCP connected.
3. **Code Intelligence API surface** — not fetched. Probably under developer docs, but the page wasn't reachable in this session.
4. **Pre-Jul 2025 changelog history** — when did semantic search originally launch? When did the first agent-as-user concept ship? Earlier changelog pages weren't fetched.
5. **Pulse audio implementation** — text + audio digest mentioned, but no detail on voice model used.
6. **Skills marketplace** — Linear has Skills (saved workflows) but no public marketplace yet. Is one planned?
7. **Coding Agent (proprietary) timeline** — "coming soon" per Mar 2026 manifesto. No firm date yet.
8. **Linear Code Reviews public-beta date** — Private beta from Jan 22, 2026. When does it open up?
9. **Quantitative accuracy claims** — Linear publishes none. Would need third-party benchmarks or customer numbers.
10. **Per-tenant model access / AI residency** — Linear hasn't signaled this enterprise governance feature. Atlassian competed on this and walked it back (per Jira research).

---

## 12. Recommended screenshots to capture

If you can capture screenshots from your live Linear workspace (or via MCP/playwright), these are the highest-value visual slots in the doc:

1. **Triage view** with a Suggestions panel showing assignee + team + project + label suggestions and the reasoning hover
2. **Auto-apply rules configuration** — Settings → Product Intelligence → rules-per-property
3. **Linear Agent overlay (⌘J)** — full chat surface from desktop app
4. **Skills library** — Settings → Skills (saved workflow templates)
5. **Agent session sheet** with thoughts, tool calls, elicitations visible
6. **"Open in &lt;agent&gt;" deeplink menu** on an issue (Cursor, Codex, Claude Code, etc.)
7. **Linear MCP tools list** as it appears in Cursor or Claude.ai settings
8. **Pulse digest** — example daily/weekly inbox entry (text + audio control)
9. **AI Filter** in action — natural language → structured filter
10. **Code Intelligence beta toggle / repo connection screen**
11. **Linear Code Reviews** view (if you have private-beta access)
12. **Workflow Builder step invoking Linear Agent** (Slack flow)
13. **Mobile agent session view** showing realtime reasoning
14. **Customer-conversation intake** (Intercom or Zendesk) → issue auto-creation result
15. **Triage Intelligence "thinking" trace panel** — context pulled in + decisions

Drop them as base64-encoded PNGs into the existing `[screenshot slot]` placeholders in `linear_ai_research.html`, or share separately and I'll embed them.

---

*Last updated: 2026-05-15 — companion to `linear_ai_research.html`.*
