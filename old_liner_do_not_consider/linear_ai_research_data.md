# Linear AI — Research Data & Sources

> **Purpose**: Supplementary research file containing raw data, sources, timeline, technical details, and competitive notes for future comparison
>
> **Research date**: May 14, 2026
>
> **Researcher notes**: Comprehensive data collected from Linear's official changelog, docs, blog, and customer stories for QPM competitive analysis

---

## Primary Sources

All information sourced from official Linear channels:

### Official Documentation & Websites
- **Linear Changelog:** https://linear.app/changelog
- **Linear Docs - Agent:** https://linear.app/docs/linear-agent  
- **Linear Docs - Triage Intelligence:** https://linear.app/docs/triage-intelligence
- **Linear Docs - Code Intelligence:** https://linear.app/docs/code-intelligence
- **Linear Docs - MCP Servers:** https://linear.app/docs/linear-agent#connect-mcp-servers
- **Linear Blog (Now):** https://linear.app/now (all posts)
- **AI Section:** https://linear.app/now/ai
- **Agents Feature Page:** https://linear.app/agents
- **CEO Letter (March 24, 2026):** https://linear.app/next (Issue tracking is dead)

### Key Blog Posts (Detailed Research)
1. **"How we built Triage Intelligence"** (Sep 3, 2025)
   - Authors: Yann-Edern Gillet, Matthijs Wolting
   - URL: https://linear.app/now/how-we-built-triage-intelligence
   - Content: Architecture (semantic search → agentic reasoning), design patterns, transparency, future roadmap

2. **"Self-driving SaaS: When software runs itself"** (Oct 22, 2025)
   - Author: Karri Saarinen (CEO)
   - URL: https://linear.app/now/self-driving-saas
   - Content: Long-term vision for autonomous agent workflows

3. **"How Cursor integrated with Linear for Agents"** (Aug 21, 2025)
   - Author: Kevin Hartnett
   - URL: https://linear.app/now/how-cursor-integrated-with-linear-for-agents
   - Content: Integration patterns, delegation model, how agents work alongside humans

4. **"How we use Linear Agent at Linear"** (Apr 10, 2026)
   - Author: Rhea Purohit
   - URL: https://linear.app/now/how-we-use-linear-agent-at-linear
   - Content: Internal workflows, real use cases across CX/Product/Eng teams

5. **"Code Intelligence for Linear Agent"** (May 14, 2026)
   - Author: Karri Saarinen
   - URL: https://linear.app/now/code-intelligence-for-linear-agent
   - Content: Latest feature announcement, codebase access, use cases

### Customer Stories
- **Coinbase** - "Agent-first development" (Mar 26, 2026) - Deleted IDEs for 2 weeks
- **Ramp** - Internal coding agent writes 60%+ of PRs (Apr 27, 2026)
- **Cars24** - Migrated from Jira due to Linear's AI-native approach (May 13, 2026)
- **Cursor** - How Cursor builds with Linear (Feb 4, 2026)
- **Mercury** - 6-month journey building with Linear agents (Jul 16, 2025)

---

## Timeline of Linear AI Releases

### Phase 1: Foundation (2025)
- **Sep 2025:** Triage Intelligence launches (beta)
  - Automatic duplicate detection, related issue linking, property suggestions
  - Agentic architecture with semantic search + LLM reasoning
  - Business+ plans only

- **Oct 2025:** Triage Intelligence design patterns documented
  - Thinking state UI, transparency panel, Additional Guidance settings

### Phase 2: Agent Launch (Mar 2026)
- **Mar 24, 2026:** Linear Agent Introduced (public beta)
  - CEO Letter: "Issue tracking is dead"
  - Three main components: Chat, Skills, Automations (Automations on Business+)
  - Chat available everywhere: app, comments, Slack, Teams
  - Skills: save successful workflows for reuse
  - Included on all plans (free during beta)

- **Mar 12, 2026:** UI refresh to support agent-forward workflow

### Phase 3: Agent Expansion (Apr 2026)
- **Apr 2, 2026:** Web forms for Linear Asks
  - Custom web intake forms for internal requests
  - Enterprise-only initially
  - Powered by issue templates

- **Apr 9, 2026:** Multi-level sub-teams
  - Agents can work within nested team structures
  - Up to 5 levels deep

- **Apr 23, 2026:** Linear Agent MCP Support
  - 16+ MCP servers available (Amplitude, Attio, Better Stack, Datadog, GitHub, Glean, Granola, HubSpot, incident.io, Intercom, Jam, Notion, PostHog, Sentry, Slack, Stripe)
  - Custom MCP server support
  - Workspace admin + user-level connection controls

- **Apr 30, 2026:** Releases Feature
  - Track deployments from Linear
  - Auto-update issue status when code deploys
  - Generate release notes with Linear Agent
  - 15 pipelines on Business, unlimited on Enterprise

### Phase 4: Code Awareness (May 2026)
- **May 14, 2026:** Code Intelligence GA (public beta)
  - Controlled GitHub repo access
  - Agents can understand codebase, answer technical questions
  - Business+ plans
  - Respects existing GitHub permissions

---

## Feature Matrix: What Works Where

### Linear Agent (Core Chat)
| Surface | Availability | Use Case |
|---------|--------------|----------|
| Dedicated Chat | All plans | Main conversational interface |
| @Linear in comments | All plans | Inline co-authoring |
| Slack @Linear | All plans | Team collaboration |
| Teams @Linear | All plans | Microsoft Teams integration |
| Mobile sessions | All plans | View agent reasoning on mobile |

### Triage Intelligence
| Capability | Status | Plan | Notes |
|-----------|--------|------|-------|
| Duplicate detection | GA | Business+ | Flags existing duplicate issues |
| Related issue linking | GA | Business+ | Suggests connected work |
| Property suggestions | GA | Business+ | Labels, assignee, project |
| Custom guidance | GA | Business+ | Workspace/team/personal instructions |
| Thinking panel | GA | Business+ | Deep visibility into reasoning |

### Code Intelligence
| Capability | Status | Plan | Notes |
|-----------|--------|------|-------|
| GitHub integration | Beta | Business+ | Read-only codebase access |
| Technical Q&A | Beta | Business+ | Ask about implementation details |
| Repository selection | Beta | Business+ | Admin chooses which repos |
| Permission scoping | Beta | Business+ | Respects GitHub access levels |

### Coding Agent Integrations
| Agent | Status | Feature | Notes |
|-------|--------|---------|-------|
| Cursor | GA | Deep link with context | Opens issue in Cursor with full spec |
| GitHub Copilot | GA | Issue → PR conversion | Native integration |
| Devin | GA | Code + testing | Full issue scope to PR |
| Sentry | GA | Root cause analysis | Powered by Sentry Seer |
| ChatPRD | GA | Requirements + feedback | Write specs, get review |

---

## Skills (Reusable Agent Workflows)

### Out-of-box Suggested Skills
1. My weekly focus areas
2. New project update
3. Project creation from PRD
4. Split into sub-issues
5. Weekly standup summary
6. Bug report template
7. Feature specification
8. Risk assessment
9. Release notes draft
10. Status email draft

### How to Create a Skill
1. Have a successful agent conversation
2. Ask Linear: "Save this as a skill"
3. Linear extracts the workflow
4. Trigger manually with slash command (/) or auto-apply

### Best Practices (Linear's Guidance)
- Start in chat with real problem
- Save once result is good + repeatable
- Keep focused (one job well, not packed)
- Optimize over time (ask agent to remove unnecessary steps)

---

## MCP Integrations (16 Available)

### Supported MCP Servers

#### Analytics & Product Insights
- **Amplitude** - Product analytics, user behavior
- **PostHog** - Feature usage, funnels, insights
- **Better Stack** - Incident tracking

#### Code & DevOps
- **GitHub** - Repository data, PRs, commits
- **Sentry** - Error tracking, performance
- **Datadog** - Monitoring, logs, traces

#### Communication & Feedback
- **Slack** - Channel content, threads, messages
- **Intercom** - Customer support tickets, conversations
- **Granola** - Meeting notes, transcripts

#### Data & Intelligence
- **Glean** - Enterprise search, knowledge base
- **Notion** - Documents, databases, wikis

#### CRM & Sales
- **Attio** - CRM data, customer records
- **HubSpot** - Contacts, deals, pipelines
- **Stripe** - Payment events, subscriptions

#### Other
- **incident.io** - Incident management
- **Jam** - Screenshot/video feedback
- **Custom URLs** - Any HTTPS MCP server

### Permission Model
- **Workspace level:** Admin approves which servers are available
- **User level:** Individual connects their own account (OAuth if needed)
- **Agent access:** Only use servers user has connected

### Real-world Use Case Examples

1. **"Pull meeting takeaways from Granola and create issues"**
   - Granola → fetch recent meeting notes
   - Linear Agent → create issues from key decisions
   - Auto-assign based on owners mentioned

2. **"Look up enterprise context to inform spec"**
   - Glean → search for existing customer data
   - HubSpot → check if customer mentioned
   - Notion → find related docs/precedents
   - Linear Agent → write more informed spec

3. **"Validate feature request with data"**
   - PostHog → check current usage
   - Amplitude → analyze user segment
   - Intercom → see what customers asked
   - Decision: prioritize or defer

4. **"Root cause analysis from error"**
   - Sentry → get crash context
   - GitHub → find recent commits to code path
   - Datadog → check perf around error time
   - Recommend fix vector

---

## Automations: Trigger Agent on Triage

### What They Do
- Run agent workflows automatically when issues enter triage
- No human prompt needed
- Define open-ended instructions (not rigid rules)

### Available On
- Business plan and above
- Public beta (April 2026)

### Example Automations
1. **SSO issue routing:** "If issue mentions SSO or auth, attach troubleshooting guide + assign to Security team"
2. **Customer impact:** "If marked as customer issue, add summary of customer impact from our CRM"
3. **Duplicate detection:** "If likely duplicate of existing issue, link and notify PM"
4. **Priority calculation:** "If multiple reports of same issue, increase priority and notify team"

### Configuration
- Team Settings → Triage → Agent behavior
- Can scope to specific issue types or apply workspace-wide
- Each automation has its own instruction set

---

## Guidance: Shape Agent Behavior

### Three Scopes

1. **Workspace Guidance**
   - Applies to everyone
   - Admin controls edit permissions
   - Examples: tone, naming conventions, required fields

2. **Team Guidance**
   - Team-specific instructions
   - Can reference in workspace guidance
   - Override workspace rules for specific team

3. **Personal Guidance**
   - Individual preferences (Settings → Agent personalization)
   - Overrides workspace guidance for that user

### Example Guidance Statements
- "Keep all summaries under 100 words and action-oriented"
- "Use this style guide for writing: [link]"
- "Always mention customer impact when discussing features"
- "For bugs, include: reproduction steps, expected behavior, actual behavior"
- "Use these labels: p0-blocker, p1-urgent, p2-soon, p3-later"

---

## Pricing & Plan Comparison

### Plan Tiers
1. **Starter** - Basic issue tracking
2. **Pro** - Teams, cycles, automations
3. **Business** - AI features, custom fields, SSO
4. **Enterprise** - Advanced permissions, web forms, unlimited releases

### AI Feature Availability

| Feature | Starter | Pro | Business | Enterprise |
|---------|---------|-----|----------|------------|
| **Agent Chat** | ✓ | ✓ | ✓ | ✓ |
| **Skills** | ✓ | ✓ | ✓ | ✓ |
| **Agent in Comments** | ✓ | ✓ | ✓ | ✓ |
| **Agent in Slack** | ✓ | ✓ | ✓ | ✓ |
| **Triage Intelligence** | — | — | ✓ | ✓ |
| **Code Intelligence** | — | — | ✓ Beta | ✓ Beta |
| **Agent Automations** | — | — | ✓ | ✓ |
| **MCP Servers** | — | — | ✓ | ✓ |
| **Web Forms (Asks)** | — | — | — | ✓ |
| **Releases** | — | — | ✓ (15) | ✓ (unlimited) |

### Pricing Commitment
- **During beta:** All features free
- **GA pricing:** Base chat remains in seat price
- **High-compute features:** Usage-based pricing possible (per-token after threshold) for Automations + Code Intelligence
- **Notice period:** 30-day advance notice before pricing changes

---

## Triage Intelligence: Technical Deep Dive

### Evolution: Why Agentic Architecture?

#### Problem with Small Models
- GPT-4o mini, Gemini 2.0 Flash could classify straightforward issues
- Failed on context-sensitive decisions (e.g., "Is this really a duplicate?")
- If context was missing, they had no way to retrieve it
- Result: Missed edge cases, false positives/negatives

#### Solution: Frontier Models + Agentic Reasoning
- Upgraded to: GPT-5, Gemini 2.5 Pro
- These models can:
  1. Analyze initial issue
  2. Decide if they need more context
  3. Dynamically query workspace data
  4. Make final decision with full picture
  5. Explain reasoning

### Architecture Flow
```
1. New issue arrives in triage
   ↓
2. Semantic search finds candidate similar issues (vector similarity)
   ↓
3. LLM analyzes: duplicate? related? new?
   ↓
4. If uncertain → agent pulls additional context from Linear
   ↓
5. LLM re-analyzes with context
   ↓
6. Outputs: suggestions (links, labels, assignee) + explanation
   ↓
7. UI shows reasoning, alternative suggestions, thinking state
```

### Design Decisions: Making Reasoning Transparent

**Challenge:** Frontier models are slower than Linear's usual deterministic systems
**Solution:** Design UI to make slowness acceptable

1. **Visible reasoning**
   - Hover over suggestion → see full explanation
   - Show alternative suggestions when available

2. **Progress indication**
   - "Thinking state" display + timer
   - Goal: System feels active, not idle

3. **Deep dive panel**
   - Full trace of model's reasoning
   - What context it pulled in
   - How guidance shaped the decision

4. **Additional Guidance**
   - Fine-tune at workspace/team level
   - Natural language instructions
   - Steer suggestions toward priorities

### Performance & Trust Principles
From Linear's Agent Interaction Guidelines:
1. **Build trust** - Show reasoning so users can validate
2. **Keep transparency** - Make decision-making visible
3. **Natural integration** - Feel like part of Linear, not an add-on

---

## Code Intelligence: Capabilities & Setup

### What Agent Can Do with Code Access
- **Answer "how?"** - How does this feature work?
- **Identify authors** - Who owns this system?
- **Track changes** - What changed recently in this module?
- **Find related code** - Where else is this pattern used?
- **Debug faster** - What could cause this error?
- **Review design** - Is this architecture sound?

### Setup Process

#### Step 1: GitHub Integration (Admin)
```
Settings → Integrations → GitHub
- Authorize Linear to read repos
- Select which repos to index
```

#### Step 2: Enable Code Intelligence (Admin)
```
Settings → AI → Code Intelligence
- Toggle "Enable Code Intelligence"
```

#### Step 3: Configure Access (Admin)
```
Choose repository access model:
- Option A: All workspace members can query
- Option B: Only users with GitHub access can query
```

### Permission Model
- Respects existing GitHub access controls
- If user doesn't have GitHub access, agent won't give code answers
- Admin can restrict which repos are queryable
- Codebase is read-only (no commit permissions)

### Supported Languages
- Python, JavaScript/TypeScript, Go, Java, C/C++, C#, Rust, PHP, Ruby, Kotlin, and more
- Uses AST (Abstract Syntax Tree) parsing for semantic understanding

---

## External Coding Agents: Integration Points

### Deep-link Mechanism
**Problem:** Developers copy issue → paste into IDE → lose context → rewrite → implement (inefficient)

**Solution:** One-click deep link with full context
```
Press: ⌘ Option . (Mac) or Ctrl Alt . (Windows/Linux)
→ Choose coding tool
→ Tool opens with:
  - Issue ID + title
  - Description + all comments
  - Linked references
  - Images + attachments
  - Custom prompt template
```

### Supported Coding Tools (15+)
| Tool | Type | Status |
|------|------|--------|
| Claude Code | LLM IDE | GA |
| Cursor | AI IDE | GA |
| GitHub Copilot | IDE Plugin | GA |
| OpenAI Codex | API | GA |
| Devin | Autonomous agent | GA |
| Warp | CLI + AI | GA |
| v0 | UI builder | GA |
| Replit | Web IDE | GA |
| Lovable | Web builder | GA |
| Zed | Code editor | GA |
| Conductor | Agent | GA |
| Amp | IDE | GA |
| Codex CLI | CLI | GA |
| Factory | Agent | GA |
| Windsurf | IDE | GA |
| Netlify Agent Runners | CI/CD | GA |

### Customizable Prompt Template
Each workspace can customize how context is passed:
```
Example template variable:
{{issue.identifier}} - dynamic issue ID
{{context}} - full issue context
```

Teams can add custom instructions:
```
"Before implementing:
1. Ask me if anything is unclear
2. Give me a detailed plan first
3. After coding, outline required tests
4. If unrelated issues found, comment instead of fixing"
```

### Mobile Agent Sessions
- View agent's chain of thought on mobile
- See real-time reasoning as agent works
- Send follow-up messages to steer work
- Review completed sessions asynchronously

---

## Releases Feature: Deployment Tracking

### What It Does
- Track software releases directly in Linear
- Link issues to releases
- Auto-update issue status when code deploys
- Generate release notes with Linear Agent

### Key Capabilities
1. **Deployment tracking**
   - Define release pipelines (iOS, Android, web, etc.)
   - Auto-sync with CI/CD (when code deploys)
   - Issue status auto-updates when live

2. **Release notes**
   - Auto-generate from included issues
   - Custom formatting with Linear Agent
   - Range support (e.g., "release notes from 0.1.5 to 0.2.0")

3. **Pipeline management**
   - Business: up to 15 pipelines
   - Enterprise: unlimited pipelines
   - Continuous deployment or scheduled release support

### Example Workflow
```
1. Engineer merges PR (closes issue)
2. CI/CD deploys to production
3. Webhook triggers Linear Releases update
4. Issue status auto-updates to "Deployed"
5. Release notes generated: "In version 0.2.1: [features]"
6. Stakeholders know what's live vs. merged
```

---

## Linear Asks: Feedback Intake

### Three Input Channels

#### 1. Slack Integration
- Mention @Linear in any channel
- "file a bug" or "create a feature request"
- Auto-creates issue in team's triage queue
- Requester stays informed via threads

#### 2. Email Capture
- Forward emails to Linear inbox
- Auto-converts to issue
- Sync thread so submitter stays in loop

#### 3. Web Forms (Enterprise)
- Custom forms per team
- Template-based (bug report, feature request, etc.)
- Anyone in company can submit (no Linear account needed)
- Submitter follows up via synced email thread

### Triage Intelligence Integration
- Incoming Asks enter triage automatically
- Triage Intelligence automatically:
  - Detects duplicates
  - Suggests routing team
  - Applies labels + properties
  - Links related work
- No manual intake work needed

---

## Customer Evidence of Agent Adoption

### Coinbase (March 2026)
- **Experiment:** "Delete your IDEs" for 2 weeks
- **Outcome:** All software development happened via agents in Linear
- **Implication:** Agents can handle real production work

### Ramp (April 2026)
- **Scale:** Internal coding agent writes 60%+ of merged PRs
- **System:** Linear provides structured context + agent executes
- **Insight:** Coding agent + Linear context = high quality output at scale

### Cars24 (May 2026)
- **Decision:** Switched from Jira to Linear
- **Reason:** Linear's AI-native approach vs. Jira's bolt-on features
- **Note:** Treated existing Jira license as sunk cost

### Cursor (Feb 2026)
- **Integration:** Deep partnership with Linear
- **Model:** Issues in Linear → agents assigned in Cursor → work back to Linear
- **Result:** "Ideas don't wait" — instant branching when feature mentioned

### Mercury (July 2025)
- **Duration:** 6-month journey building with Linear + agents
- **Documentation:** Blog post showing workflows, learnings
- **Implication:** Enterprise adopters are investing time in agent workflows

---

## Competitive Positioning Notes

### vs. Jira + Rovo
| Dimension | Linear | Jira/Rovo |
|-----------|--------|-----------|
| **Agent UI** | First-class (everything is agentic) | Sidebar add-on |
| **Codebase integration** | Code Intelligence (native) | Limited |
| **Speed philosophy** | First principle | Process-heavy |
| **MCP support** | 16+ ecosystems | Enterprise integrations only |
| **Pricing** | Simpler (all features on Business+) | Tiered (premium features higher) |
| **Vision** | Self-driving SaaS | AI-augmented workflow |

### vs. Asana
| Dimension | Linear | Asana |
|-----------|--------|-------|
| **Agent availability** | All plans | Premium+/Advanced tier |
| **Skills/Automations** | Built-in, extensive | Limited, requires setup |
| **Code integration** | Code Intelligence | No |
| **MCP** | Yes, 16+ servers | No |
| **Philosophy** | Compress process | Enhance process |

### vs. ClickUp
| Dimension | Linear | ClickUp |
|-----------|--------|---------|
| **Agent integration** | Native, core product | Bolt-on AI modules |
| **Triage automation** | Triage Intelligence | Basic AI routing |
| **Coding agent partnership** | Deep (Cursor, etc.) | Limited |
| **Speed** | Minimal, fast UI | More feature-heavy |
| **Code awareness** | Code Intelligence | No |

### vs. Monday.com
| Dimension | Linear | Monday.com |
|-----------|--------|------------|
| **AI philosophy** | Replace overhead | Enhance UI |
| **Agent model** | Autonomous + collaborative | Assistant-only |
| **Automations** | Agent-driven | Rule-driven |
| **Coding** | First-class support | No |
| **Simplicity** | Core principle | Full-featured |

---

## Long-term Vision: "Self-driving SaaS"

### CEO's Thesis (Karri Saarinen, Oct 2025)
> "Real progress comes when AI stops requiring constant input and instead proactively moves work forward."

### Progression Roadmap
1. **Today (May 2026):** Agents answer questions, execute on command
2. **Next (2026-2027):** Agents work autonomously within defined boundaries
3. **Future:** Agents proactively identify + move work forward without explicit trigger

### Evidence Already Happening
- Ramp: 60%+ of PRs written by agent (no human per-PR prompt)
- Coinbase: 2-week "delete IDEs" experiment shows agents can drive full development
- Triage Intelligence: Auto-routes, classifies, deduplicates without human review

### Roadmap Announcements
- **Code Diffs:** Modern review UI for human + agent collaboration
- **Linear Coding Agent:** Native code-writing agent in Linear
- **Deep context understanding:** Full system awareness (architecture, customer feedback, strategy, code)

---

## Key Metrics & Adoption Signals

### Linear Workspace Adoption
- **Coding agents installed:** 75%+ of Linear enterprise workspaces
- **Agent-generated work:** Nearly 25% of new issues in those workspaces
- **Growth rate:** 5x increase in work volume completed by agents (last 3 months)

### Product Momentum
- **Public beta launch:** March 24, 2026 (Linear Agent)
- **Beta status:** Still free (as of May 2026) — GA pricing TBA
- **Enterprise adoption:** Coinbase, Ramp, Cars24, Cursor, Mercury (public customers)

### Team Size & Investment
- ~500 people at Linear (as of public info)
- Multiple dedicated teams: Agents, Triage, Code Intelligence, Integrations
- Continuous release cadence (weekly changelog updates)

---

## Open Questions & Future Watch Items

### Unknowns
1. **GA pricing:** When will Linear charge for Automations + Code Intelligence? Usage-based or seat-based?
2. **Code Diffs:** Timeline and differentiation from existing PR review tools?
3. **Linear Coding Agent:** How does it differ from delegating to Cursor/Codex directly?
4. **Cross-workspace context:** Will agents ever work across multiple Linear workspaces?
5. **Enterprise scalability:** How do large orgs (100+ teams) manage shared agent governance?

### Potential Improvements to Monitor
1. **Agent reasoning visibility:** Currently requires clicking deep panel. Could be more accessible.
2. **Skills discovery:** How do teams share best practices? Is there a community skills marketplace?
3. **Failed agent actions:** What happens when agent makes mistake? Audit trail + rollback?
4. **Multi-step workflows:** Can agent tasks chain (issue → triage → auto-assign → notify → close) automatically?
5. **Workspace-to-workspace sync:** Can agent pull context from external Linear workspaces?

---

## Key Takeaways for QPM

### What Linear Did Well
1. **Agent-first UX:** Not a sidebar chat. Agents permeate the entire product.
2. **Transparency by design:** Reasoning panels, guidance controls, thinking state displays.
3. **Ecosystem approach:** MCP integrations let users bring their own context.
4. **Developer empathy:** Deep partnerships with coding tools (Cursor, Codex) instead of building solo.
5. **Simplification thesis:** Remove process overhead instead of adding features.

### Strategic Positioning
- Linear is betting on **context → execution** model
- Traditional issue tracking is seen as overhead (handoff-based, process-heavy)
- Agents work best when they have full workspace context + permission to act
- Speed (even with LLM reasoning) is non-negotiable

### Implementation Insights
- Agentic approach (let model pull context vs. rigid prompts) much better for quality
- Frontier models (GPT-5, Gemini 2.5 Pro) worth the compute cost for nuanced reasoning
- Trust requires transparency (thinking panels, reasoning explanations)
- Permissions matter (agents respect user access controls)

---

## Recommended Further Research

### Topics for Next Phase
1. **Jira AI Deep Comparison:** How does Rovo's agent model compare to Linear's?
2. **Asana's Agent Strategy:** What are Asana's plans for AI agents?
3. **ClickUp's AI Roadmap:** How is ClickUp positioning AI?
4. **Notion's Custom Agents:** How do they integrate with Linear (mentioned in changelog)?
5. **MCP Ecosystem:** What other tools are building MCP servers?

### Interviews to Consider
- Linear team (Kevin Hartnett - head of product marketing?)
- Linear customers (Ramp, Cars24, Cursor)
- External developers building custom Linear agents
- MCP server builders

---

## Document Version History

| Date | Changes | Author |
|------|---------|--------|
| May 14, 2026 | Initial research compilation | QPM AI Research |
| — | Linear Agent + Triage + Code Intelligence documented | — |
| — | MCP ecosystem cataloged | — |
| — | Competitive positioning added | — |
| — | Customer stories + metrics included | — |

---

**Last updated:** May 14, 2026  
**Status:** Complete for Linear competitor analysis  
**Next step:** Schedule comparison session across all competitors (Linear, JIRA, Asana, ClickUp, Notion)
