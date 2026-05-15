# Plane AI Research — Summary

> Companion summary for [plane_ai_research.html](plane_ai_research.html) and [plane_ai_research_raw_notes.md](plane_ai_research_raw_notes.md).
>
> **Date:** 2026-05-15

---

## What's in the doc — 17 sections

1. **The OSS thesis** — why Plane is structurally different from every other competitor (open-source + self-hostable + air-gap-ready + BYO model keys)
2. **The three modes** — Ask / Build / Assign (Plane AI's intentionally minimalist surface)
3. **Plane AI formula** — BYO Anthropic/OpenAI keys + workspace context + native MCP + Slack/Teams intake + Agent SDK
4. **Plane AI in depth** — 13 capabilities, all GA today
5. **Agents** — Agent Development Kit, Agent Run lifecycle, Marketplace, open-source MCP server
6. **Slack + Teams AI intake** — @Plane in any channel, "AGI-like" framing, Claude Sonnet 4.0 default
7. **Plane MCP** — 55+ tools, HTTP + PAT + Stdio transports, open-source on GitHub
8. **Self-hosting** — Prime CLI, God Mode, Docker/K8s/air-gapped, full AI parity with cloud
9. **Plane Compose** — Projects-as-Code (YAML in Git) — no competitor has an equivalent
10. **Four products in one workspace** — Projects + Wiki + Plane AI + Desk (coming)
11. **Migration path** — "Get out of Jira/Linear/ClickUp/Monday/Asana"; 2× Fortune 10 customers migrated from Jira
12. **Pricing & BYO-keys** — no AI seat upcharge; self-host customers pay model provider directly
13. **Governance** — air-gapped, "no prompt storage", SOC 2 / ISO 27001 / GDPR / CCPA
14. **Strategic vector** — Vamsi Kurama's "steerable systems" thesis
15. **Release timeline** — 13 milestones, Nov 2025 (Plane AI + Slack launch) → May 2026 (v1.3.1 OSS)
16. **Adoption signals** — Fortune 10, governments, 92 employees, $4M seed (OSS Capital)
17. **Activation & setup** — cloud path (5 steps) + self-hosted path (6 steps)

---

## Two things to flag

- **Screenshots** — same as the prior docs: no Plane MCP / playwright tooling in this session. I marked `[screenshot slot]` placeholders for the 2 most natural visual spots (Plane AI panel in Ask mode, Plane AI in Build mode). 16 recommended screenshots in the raw notes.
- **Plane is the structural outlier of the 7-tool research.** Where ClickUp/monday are aggressive on AI breadth, Notion bets on the workspace-as-memory moat, and Linear/Asana stay narrow, Plane is the *only* competitor where the architectural baseline is open-source + self-hostable + air-gap-ready + BYO model keys. That single choice shapes everything — pricing (no AI seat upcharge), customer mix (Fortune 10 + regulated + government), MCP design (HTTP/PAT/Stdio for self-hosted), migration narrative ("get out of Jira"), and team size (92 employees, smallest by ~10×).

---

## What's structurally unique about Plane vs the other 6 competitors

| Dimension | Plane | All others (Jira, Linear, ClickUp, monday, Notion, Asana) |
|---|---|---|
| Open source | ✅ Yes (github.com/makeplane/plane) | ❌ Closed-source SaaS |
| Self-hostable | ✅ Yes (Docker / K8s / air-gapped) | ❌ Cloud-only |
| BYO model keys | ✅ Yes (Anthropic OR OpenAI direct) | ⚠ No — they aggregate model spend |
| MCP server open source | ✅ Yes (github.com/makeplane/plane-mcp-server) | ❌ MCP servers are proprietary |
| "No prompt storage" guarantee | ✅ Yes (especially air-gapped) | ⚠ Varies; ClickUp/Notion close but on their cloud |
| Projects-as-Code (GitOps) | ✅ Yes (Plane Compose) | ❌ No equivalent |
| AI included on every plan | ✅ Yes ("ships on every plan") | ⚠ Most have AI gated to higher tiers |

---

## The structural takeaway

Plane is targeting the **segment that the other 6 competitors structurally cannot serve** — organisations that won't or can't put their data in a vendor cloud. That's regulated industries (finance, health, pharma), governments (Lithuania, France named publicly), defence-adjacent (Aramco), and Fortune 10 enterprises (2× migrated from Jira). For the QPM positioning question: Plane is the closest analogue to a *competitor your customers can run on-prem with your own AI keys* — none of the others can credibly claim that.

Ready to do **Asana** (last competitor in the 7-tool list) whenever you say. After that we'll have a complete picture of all 7 AI strategies and a natural moment to write the cross-competitor synthesis if you want one.

---

## Sources

- [Plane homepage](https://plane.so/)
- [Plane AI product page](https://plane.so/ai)
- [Plane changelog](https://plane.so/changelog)
- [Plane GitHub repo](https://github.com/makeplane/plane)
- [Plane GitHub releases](https://github.com/makeplane/plane/releases)
- [Plane MCP server (open source)](https://github.com/makeplane/plane-mcp-server)
- [Plane developer docs — MCP server](https://developers.plane.so/dev-tools/mcp-server)
- [Plane developer docs — MCP for Claude Code](https://developers.plane.so/dev-tools/mcp-server-claude-code)
- [TechCrunch — Plane takes on Jira with open source PM (2023)](https://techcrunch.com/2023/11/28/plane-takes-on-jira-with-open-source-project-management-tools-for-software-teams/)
- [Tracxn — Plane company profile](https://tracxn.com/d/companies/plane/__OjXBhlsZqjglanUr7xsV_SOfaNnAto1vJIWKkZCDHus)
- [Clay — Plane funding](https://www.clay.com/dossier/plane-funding)
- [Crunchbase — Vamsi Kurama profile](https://www.crunchbase.com/person/vamsi-kurama)
- [LinkedIn — Vamsi Kurama (Co-founder & CEO)](https://www.linkedin.com/in/vamsi-kurama/)
- [StartupsMeet — $4M seed announcement (April 2024)](https://www.startupsmeet.com/2024/04/tech-startup-plane-secures-4-million-in-seed-funding-to-enhance-project-management/)
- [Codersera — 15 MCP Servers Worth Wiring (2026 ecosystem context)](https://codersera.com/blog/best-mcp-servers-claude-code-cursor-2026/)
