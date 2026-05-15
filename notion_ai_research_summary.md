# Notion AI Research — Summary

> Companion summary for [notion_ai_research.html](notion_ai_research.html) and [notion_ai_research_raw_notes.md](notion_ai_research_raw_notes.md).
>
> **Lens:** Notion as a Jira + Confluence equivalent — i.e. one tool covering task tracking AND wiki/documentation.
> **Date:** 2026-05-15

---

## What's in the doc — 18 sections

1. **PM+wiki verdict** — can Notion replace Jira + Confluence? (decision matrix by team size and type)
2. **Three pillars** — Notion Agent / Custom Agents / Enterprise Search + MCP/Dev Platform horizontal layer
3. **Notion 3.0** — the GPT-5 architectural rebuild (Sep 18, 2025) — 20-min autonomous runs across hundreds of pages
4. **Notion AI formula** — central reasoning model + modular sub-agents + pages-as-memory + multi-model gateway
5. **Notion Agent (personal)** — the in-product assistant, ⌘+I anywhere, Plan Mode, multi-model picker
6. **Custom Agents** — proactive/triggered/autonomous, 1M+ created in 2 months of beta, $10/1000 credits from May 4, 2026
7. **AI Meeting Notes** — Granola-style native transcription (Zoom/Meet/Teams/Slack Huddles/FaceTime/YouTube)
8. **Enterprise Search Beta** — Slack/Drive/GitHub/Jira/Linear/Teams/SharePoint/OneDrive connectors + "Verify any page" → AI citation
9. **Developer Platform 3.5** (May 13, 2026) — External Agents API, Database Sync, Custom Agent Tools, Webhook triggers, Notion Workers, Notion CLI, Agent SDK
10. **Notion MCP** — `https://mcp.notion.com/mcp`, OAuth, full permission inheritance, 91% more token-efficient (Apr 2026)
11. **Notion as PM tool** — Jira lens — what works (DBs/autofill/agents) and what doesn't (sprint velocity, deep Git, JSM)
12. **Notion as wiki** — Confluence lens — what wins (block editor, Verify any page, AI citations) and what doesn't (Jira sync, indefinite version history)
13. **Pricing** — Free / Plus $10 / Business $20 / Enterprise + Notion Credits add-on
14. **Governance** — Custom Agent admin controls, MCP Governance (Enterprise), "no training" stance
15. **Strategic vector** — the all-in-one AI workspace, pages-as-memory moat, 3/6/12-month outlook
16. **Release timeline** — 13 dated milestones, May 2025 (AI Meeting Notes) → May 2026 (Dev Platform 3.5)
17. **Adoption signals & sentiment** — 1M+ Custom Agents, OpenAI's GPT-5 customer story, bullish on docs, weak on PM-only
18. **Activation & setup** — 8-step turn-on tailored for the Jira+Confluence replacement use case

---

## Headline verdict on the lens you asked about

### Can Notion replace Jira + Confluence?

- **Startup / SMB < 50 people:** Yes. Notion 3.0 Agents work cross-database + cross-page; consolidation is a clear win.
- **SMB 50–150, mostly non-engineering:** Yes. Marketing/product/design/HR thrive in Notion.
- **Eng-heavy 50–200 people:** Hybrid. Notion for docs + Enterprise Search to read Jira/Linear; tracker stays where it is.
- **Eng-heavy 200+ people:** No. Atlassian's Jira-Confluence linkage + Rovo unified context is hard to dislodge.
- **Regulated industry:** No (or Notion Enterprise with discipline). Atlassian's compliance posture + Confluence indefinite history wins.

### The single most important differentiator for the PM+wiki use case

**"Verify any page" + AI citations.** When Notion AI cites a page, verified pages outrank unverified ones and get a badge. Confluence has nothing like it. For teams using Notion as both the wiki AND the task-tracking source of truth, this is the feature that prevents "stale-doc-vs-live-ticket" drift — which is exactly the problem Atlassian solves with native Jira ↔ Confluence sync but Notion solves differently.

---

## Two things to flag

- **Screenshots** — same situation: no Notion MCP / playwright tooling in this session. I marked `[screenshot slot]` placeholders for the 2 most natural visual spots (Notion Agent chat panel with model picker, model picker itself). 17 recommended screenshots in the raw notes file.
- **The acquisition story is different here.** Unlike ClickUp (Qatalog + Codegen) or monday (Agentalent), Notion built everything in-house — including the GPT-5 architectural rebuild featured in OpenAI's own customer story. The strategic moat Notion is building is structural: <strong>pages and databases ARE the agent memory</strong>, which means Notion's agents have a substrate competitors had to invent separately.

Ready to move to the next competitor — **Asana** (AI Teammates, AI Studio, Smart Workflows, Work Graph, Asana Gov) or **Plane** (smaller scope, Slack AI intake, MCP, open-source angle) — whenever you say.

---

## Sources

- [Notion AI overview](https://www.notion.com/product/ai)
- [Notion AI Meeting Notes](https://www.notion.com/product/ai-meeting-notes)
- [Notion Releases](https://www.notion.com/releases)
- [Introducing Notion 3.0 (Akshay Kothari, Sep 18, 2025)](https://www.notion.com/blog/introducing-notion-3-0)
- [OpenAI Customer Story — Notion's GPT-5 rebuild](https://openai.com/index/notion/)
- [Notion MCP Help Center](https://www.notion.com/help/notion-mcp)
- [Notion MCP Developer Docs](https://developers.notion.com/docs/mcp)
- [Notion MCP Get Started](https://developers.notion.com/guides/mcp/get-started-with-mcp)
- [GitHub — Official Notion MCP Server (makenotion)](https://github.com/makenotion/notion-mcp-server)
- [GitHub — Claude Code Notion Plugin](https://github.com/makenotion/claude-code-notion-plugin)
- [TechCrunch — Notion launches its first AI agents](https://techcrunch.com/2025/09/18/notion-launches-agents-for-data-analysis-and-task-automation/)
- [TechCrunch — Notion takes on AI notetakers like Granola](https://techcrunch.com/2025/05/13/notion-takes-on-ai-notetakers-like-granola-with-its-own-transcription-feature/)
- [Notion Custom Agent Pricing](https://www.notion.com/help/custom-agent-pricing)
- [Atlassian — Confluence vs Notion](https://www.atlassian.com/software/confluence/comparison/confluence-vs-notion)
- [Nuclino — Notion vs Jira (2026)](https://www.nuclino.com/solutions/notion-vs-jira)
- [Nuclino — Confluence vs Notion (2026)](https://www.nuclino.com/solutions/confluence-vs-notion)
- [Trackr — Notion vs Confluence in 2026](https://www.trytrackr.com/blog/notion-vs-confluence-2026)
- [Docsie — Confluence vs Notion: A Doc Builder's Honest Take](https://www.docsie.io/blog/articles/confluence-vs-notion-enterprise-comparison-2026/)
- [TheDigitalProjectManager — Jira vs Notion](https://thedigitalprojectmanager.com/tools/jira-vs-notion/)
- [Strac — Notion MCP Server: Secure Setup](https://www.strac.io/blog/notion-mcp-server)
- [tl;dv — Notion AI Meeting Notes Review](https://tldv.io/blog/notion-ai-meeting-notes-review/)
- [eesel AI — Notion AI Review 2026](https://www.eesel.ai/blog/notion-ai-review)
- [Connex Digital — Notion Custom Agent Credits](https://connex.digital/blog/notion-custom-agent-credits-how-to-cut-costs-before-the-paid-era-begins/)
- [felloai — Notion AI Pricing 2026](https://felloai.com/notion-ai-pricing/)
