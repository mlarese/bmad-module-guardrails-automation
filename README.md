# Guardrails Automation (`gau`)

A focused BMad module for routing repeatable processes across software, databases, legal, tax, design, architecture, healthcare, web, paid media, social content, creative video, and revenue management.

This is a focused BMad module in the [Guardrails](https://github.com/mlarese/bmad-module-guardrails)
bundle. It keeps the same behavior and shared memory while installing only the figures and
workflows for the automation area.

> **Generated.** This repository is produced by `tools/build_modules.py` in the
> [bmad-module-guardrails](https://github.com/mlarese/bmad-module-guardrails) repository.
> Make changes there and regenerate; local changes here will be overwritten.

## Agents

| Agent | Role | Skill | Focus |
| ----- | ---- | ----- | ----- |
| 🛡️ Vera | Data Protection Officer | `grl-agent-privacy` | Personal data, GDPR, DPIAs, retention, analytics, logs, and data in prompts. |
| 🔐 Kai | Application Security Engineer | `grl-agent-security` | APIs, authentication, authorization, secrets, dependencies, CVEs, and LLM attack surfaces. |
| ⚖️ Aldo | Tech Lawyer | `grl-agent-legal` | Licenses, contracts, DPAs, ownership, AI outputs, and AI Act obligations. |
| 📐 Nils | Regulatory Compliance | `grl-agent-compliance` | NIS2, DORA, EAA/WCAG, eIDAS, CRA, MDR, and sector-specific obligations. |
| 🧾 Marta | Tax and Incentives Specialist | `grl-agent-fiscal` | Taxes, VAT, grants, incentives, tax credits, and reporting. |
| 👁️ Iris | Design Critic | `grl-agent-ui-critic` | UI, landing pages, markup, CSS, typography, palettes, density, and layout. |
| 🧱 Otto | Code Architect | `grl-agent-architecture` | Boundaries, folders, dependencies, interfaces, factories, and architectural layers. |
| 🗄️ Dario | Database Architect & Designer | `grl-agent-database` | Data models, PostgreSQL, Oracle, MongoDB, Redis/Valkey, distributed SQL, NoSQL, search, analytics, time-series, graph, vector, and hybrid search. |
| 🖥️ Bruno | Infrastructure & Ops Engineer | `grl-agent-ops` | Servers, VPS, Docker, CI/CD, deployment, TLS, backups, logs, and incidents. |
| 🩺 Livia | Clinical Informatics | `grl-agent-health` | Clinical data, codes, HL7/FHIR/DICOM, clinical workflows, and patient safety. |
| 🧠 Enzo | AI Engineer | `grl-agent-ai` | LLMs, prompts, RAG, embeddings, tool calling, evaluations, costs, and latency. |
| 🧩 Milo | WordPress Component Architect | `grl-agent-wordpress` | Gutenberg, Elementor, ACF, post types, template parts, and the Media Library. |
| 🔎 Nora | SEO Strategist & Search Systems Auditor | `grl-agent-seo` | Search intent, crawling, indexing, content, structured data, and Search Console. |
| 📣 Dalia | Media Manager & Paid Advertising Strategist | `grl-agent-ads` | Google Ads, paid advertising, audiences, creative, tracking, consent, budgets, and policies. |
| 📱 Sofia | Social Media & Content Strategist | `grl-agent-social` | Organic strategy, content pillars, calendars, posts, captions, community, and metrics. |
| 🎬 Marco | Advertising Creative Director & Short-form Video Producer | `grl-agent-creative` | Advertising concepts, design, scripts, storyboards, shot lists, Reels, TikToks, and Shorts. |
| 📈 Rhea | Revenue Management Strategist | `grl-agent-revenue` | Occupancy, ADR, RevPAR, TRevPAR, NRevPAR, GOPPAR, MUP, MOL, pickup, forecasting, pricing, PMS, and Channel Manager. |

## Skills and workflows

| Skill | Purpose |
| ----- | ------- |
| `gau-profile` | Project profile | Collects the project context shared by every installed figure. |
| `gau-board` | Multidisciplinary review | Convenes the relevant figures on one artifact and returns a review summary or release verdict. |
| `grl-legal-updates` | Live legal updates | Searches primary sources for laws, decrees, rulings, and amendments in a defined period, with coverage and freshness checks. |
| `grl-fiscal-updates` | Live fiscal updates | Searches primary sources for tax rules, circulars, grants, incentives, amendments, and deadlines in a defined period. |
| `grl-mdsw` | Medical-device qualification | Assesses whether a software feature has a medical purpose and identifies the relevant MDR scope and planning impact. |
| `grl-web` | Web experience delivery | Moves landing pages and websites from a conversion brief through visual review, accessibility, SEO, and delivery. |
| `grl-ads` | Paid media operations | Audits, plans, tracks, optimizes, preflights, and applies paid-media change sets behind approval and rollback gates. |
| `grl-social` | Organic social strategy | Builds social strategies, calendars, content, audits, and measurement plans without scheduling or publishing. |
| `grl-social-creative` | Social creative production | Turns a brief into producible concepts, scripts, storyboards, shot lists, specifications, and channel variants. |
| `grl-revenue-audit` | Revenue data and pricing audit | Produces a read-only audit of exports, data quality, KPIs, demand, and the economic floor. |
| `grl-revenue-plan` | Revenue planning | Builds pricing, demand, and profit scenarios while separating the economic floor, market, and forecast. |
| `grl-revenue-preflight` | PMS and Channel Manager preflight | Checks contract, mapping, dry-run, response, reconciliation, idempotency, and rollback before transmission. |
| `grl-automation` | Controlled automation | Routes work from read-only checks through dry-run to observable execution, with explicit approvals and rollback. |

## Installation

```
bmad install gau
```

As a first step, run `gau-profile`. It collects the project profile — sector, data,
market, stack, and criticality — so each figure can calibrate its review. Without a profile,
the default remains `normal` and the figures start without context.

## Shared memory

The profile lives in `{project-root}/_bmad/memory/grl-shared/project-profile.md`, together
with `decisions.md` and `accepted-risks.md`. All Guardrails modules use the same path, so two
installed modules still share one profile.

## Using it with the bundle

This module installs skills with **the same names** as the `grl` bundle — `grl-agent-privacy`
is identical in both. Do not install the full bundle and thematic modules in the same project:
choose the complete bundle, or only the thematic modules you need.

## License

MIT.
