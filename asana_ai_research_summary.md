# Asana AI Research — Summary

> Companion summary for [asana_ai_research.html](asana_ai_research.html) and [asana_ai_research_raw_notes.md](asana_ai_research_raw_notes.md).
>
> **Date:** 2026-05-15

---

## What's in the doc — 16 sections

1. **The "Agentic Enterprise" thesis** — Dan Rogers' framing; Asana as "the foundational system of action layer for the Agentic Enterprise"
2. **The three pillars** — AI Studio / AI Teammates / Work Graph
3. **Asana AI formula** — Work Graph + multi-LLM (OpenAI + Anthropic) + Memory Associations + human-in-the-loop
4. **Work Graph®** — the proprietary context model (relational graph of tasks/projects/goals/people)
5. **AI Studio** — no-code AI workflow builder with credit metering (50K Starter / 100K Plus / 5M Pro)
6. **AI Teammates** — 21 prebuilt collaborative agents; GA for sales-led customers Q1 FY27 (≈ May 2026)
7. **The full teammate roster** — 7 Marketing + 6 Ops/PMO + 5 IT + 3 Product/Eng + custom builder
8. **Memory system** — Memory Associations linked to Work Graph objects (text-fact, not vector DB)
9. **Governance** — "context, checkpoints, controls" trust brand; human-in-the-loop by design
10. **Asana Gov** — US public sector tier (Winter 2026 launch); FedRAMP/DoD level not publicly disclosed
11. **Integrations** — Claude (featured), OpenAI, MS Copilot, Slack; AI Connectors for OpenAI/Slack/Notion; **NO public MCP server**
12. **Pricing** — Personal Free / Starter $10.99 / Advanced $24.99 / Enterprise sales-led + Asana Gov; AI Studio credits at three tiers
13. **Strategic vector** — the AI bet IS Asana's growth story; FY27 guidance ($850M-$858M revenue, 15% AI net new ARR) hinges on Teammates GA
14. **Release timeline** — Jun 2024 (initial Teammates announce) → Q1 FY27 GA (≈ May 2026)
15. **Adoption signals + financial context** — 200+ beta customers, 93% full edit access, 2x faster work, $201M Q3 FY26 revenue (+9% YoY), stock down ~50% in 2026
16. **Activation & setup** — 8-step turn-on

---

## Two things to flag

- **Screenshots** — same situation: no Asana MCP / playwright tooling in this session. I marked `[screenshot slot]` placeholders for the 2 most natural visual spots (AI Studio canvas, credit dashboard). 17 recommended screenshots in the raw notes file.
- **The AI Teammates Q1 FY27 GA milestone is the single most important near-term catalyst.** Dan Rogers locked it in on the Q4 FY26 earnings call: sales-led customers GA by end of Q1 FY27 (≈ May 2026), self-serve GA in H2 FY27. The FY27 guidance ($850M–$858M revenue + 15% of net new ARR from AI products) bakes this in. ASAN stock is down ~50% in 2026 and ~92% from all-time highs — the market is pricing the company for AI-disruption risk. The Teammates GA narrative landing at Q1 FY27 earnings (≈ Aug 2026) is the re-rating catalyst.

---

## What's structurally unique about Asana vs the other 6 competitors

| Dimension | Asana | Other 6 |
|---|---|---|
| Brand of AI safety | **"Context, checkpoints, controls"** — explicit trust brand | Various; less crisp |
| Context substrate | **Work Graph** — relational graph of tasks/projects/goals/people | Notion: pages-as-memory; ClickUp: BrainGPT + ActionQuery; monday: mondayDB; Linear: structured tickets |
| Human-in-the-loop posture | **"Claude cannot act autonomously within Asana — every consequential action requires explicit user approval"** | Mixed; ClickUp and monday push more autonomy |
| Enterprise + Gov focus | Strongest — Asana Gov is a named SKU | None has a named gov SKU |
| Stock-market pressure | **Public + down 50% YTD** — AI GA is the catalyst | Linear/ClickUp/Plane/Notion private; monday public but stable; Atlassian public but Rovo isn't the catalyst |
| MCP server | **Conspicuously absent** from /product/ai | Every other competitor in this research has one |

---

## The strategic positioning summary

Asana is the only PM competitor whose **AI bet is the public-market growth catalyst** with a fixed near-term GA date and a baked-in % of net new ARR target. Where Linear is positioning AI as an architectural conviction, ClickUp is converging on a work-OS, monday is rebranding around AI Work Platform, Notion is leaning on pages-as-memory, and Plane is targeting the OSS / air-gap niche, Asana is making a **single concentrated bet that enterprise governance + Work Graph context + AI Teammates GA = the rerating**. If it lands at Q1 FY27 earnings, ASAN re-rates. If it slips, the disruption-risk thesis wins.

---

## All 7 competitors complete

This concludes the 7-tool research run. We now have full docs for:

1. ✅ [JIRA AI](jira_ai_research.html) — Atlassian Intelligence + Rovo + DX (your original)
2. ✅ [Linear AI](linear_ai_research.html) — Triage Intelligence + Linear Agent + Code Intelligence
3. ✅ [ClickUp AI](clickup_ai_research.html) — Brain² + Super Agents + Brain MAX (Qatalog + Codegen acquisitions)
4. ✅ [monday.com AI](monday_ai_research.html) — Sidekick + Vibe + Agents + Agentalent
5. ✅ [Notion AI](notion_ai_research.html) — Notion Agent + Custom Agents + Enterprise Search (with PM+wiki lens)
6. ✅ [Plane AI](plane_ai_research.html) — Plane AI + MCP-native + self-hostable + air-gap
7. ✅ [Asana AI](asana_ai_research.html) — AI Studio + AI Teammates + Work Graph + Asana Gov

The natural next step is a **cross-competitor synthesis** — a single doc that compares all 7 on key dimensions (pricing models, MCP support, agent architecture, governance, model gateways, etc.) and synthesizes the strategic patterns for QPM positioning decisions. Say the word when you want it.

---

## Sources

- [Asana AI overview](https://asana.com/product/ai)
- [Asana AI Teammates](https://asana.com/product/ai/ai-teammates)
- [Asana Work Graph®](https://asana.com/resources/work-graph)
- [How AI Teammates Build Memory](https://asana.com/inside-asana/ai-teammates-turn-work-into-reusable-information)
- [AI Agents Built for Teams: Shared Context and Transparency](https://asana.com/inside-asana/ai-agents-built-for-teams-context-transparency)
- [Asana AI Teammates 2026 overview](https://asana.com/resources/ai-teammates-overview)
- [Asana What's New (Winter 2026 release)](https://asana.com/whats-new)
- [Asana Q4 FY26 earnings press release](https://investors.asana.com/news-releases/news-release-details/asana-announces-fourth-quarter-and-fiscal-year-2026-results)
- [Asana Q3 FY26 earnings press release](https://investors.asana.com/news-releases/news-release-details/asana-announces-third-quarter-fiscal-2026-results)
- [Asana Q4 2026 earnings call transcript (Motley Fool)](https://www.fool.com/earnings/call-transcripts/2026/03/02/asana-asan-q4-2026-earnings-call-transcript/)
- [Seeking Alpha — Asana outlines AI Teammates GA + raised FY26 guidance](https://seekingalpha.com/news/4527894-asana-outlines-ai-teammates-general-availability-and-raises-fy-2026-guidance-amid-9-percent)
- [Computerworld — Asana puts 'AI teammate' agents to work](https://www.computerworld.com/article/4063082/asana-puts-ai-teammate-agents-to-work.html)
- [VentureBeat — Asana launches Claude integration, context-starved framing](https://venturebeat.com/orchestration/asana-launches-claude-integration-says-ai-models-are-context-starved-without)
- [VentureBeat — Asana unveils customizable AI Teammates](https://venturebeat.com/ai/asana-unveils-customizable-and-intelligent-ai-teammates-to-optimize-projects-and-business-workflows)
- [TIKR — Why Asana 50% Crash May Overstate AI Disruption Risk](https://www.tikr.com/blog/heres-why-asana-stocks-50-crash-in-2026-may-overstate-the-ai-disruption-risk)
- [UC Today — Asana Q3 earnings exceed forecasts despite executive resignations](https://www.uctoday.com/unified-communications/asanas-q3-earnings-exceed-forecasts-despite-surprise-executive-resignations/)
- [Asana AI Studio pricing (help center)](https://help.asana.com/s/article/ai-studio-pricing)
- [BusinessWire — Asana Announces New AI Teammates: Collaborative Agents](https://investors.asana.com/news-releases/news-release-details/asana-announces-new-ai-teammates-collaborative-agents-deliver)
- [Asana Catches Security Risks Before Anyone Writes Code with AI Teammates](https://asana.com/resources/asana-catches-security-risks-with-ai-teammates)
