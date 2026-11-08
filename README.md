# Awesome-AI-Generated-API-Documentation

# Awesome-AI-Generated-API-Documentation

**Top AI Generated API Documentation (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Agentic Doc Authoring, OpenAPI-to-Markdown Generation, llms.txt & Self-Hosted Documentation Pipelines*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI-Generated API Documentation**. These tools enable API teams to turn OpenAPI specs, source code, and prompts into accurate, maintainable documentation—automating the drudgery of writing getting-started guides, endpoint references, and code examples while keeping humans in the review loop.



**Examples** include Mintlify, ReadMe, GitBook, Fern, SwaggerHub, Redocly, Postman, Stoplight, Scalar, and Docusaurus (the category leaders in commercial and open-source space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted doc generation, OpenAPI rendering, and open documentation infrastructure. **Critical note**: The open-source landscape has matured—**Apimatic** generates Markdown API docs directly from Flask/FastAPI source with optional local Ollama or cloud LLM enhancement , **printing-press** turns OpenAPI contracts into fully offline, agent-ready static docs with built-in llms.txt and AGENTS.md , and **Scalar** provides an MIT-licensed OpenAPI reference that many commercial platforms use under the hood. No open-source project matches Mintlify's agentic PR workflow or ReadMe's multi-page audit capabilities, but for core generation and rendering, the building blocks are production-capable.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The API documentation tools and developer portals market is currently valued at approximately **$2.8 billion** and is projected to reach **$7.6 billion** over the next decade (growing at ~11.7% CAGR), spurred by the rapid expansion of API-first architectures and AI-driven developer workflows. The sector is **moderately fragmented** rather than winner-take-all; despite heavyweight incumbents like Postman and SmartBear anchoring enterprise API testing and management, developer preference for modular docs-as-code pipelines, specialized agentic authoring platforms (e.g., Mintlify, ReadMe), and deeply entrenched open-source building blocks (e.g., Scalar, Docusaurus, Backstage) sustains a vibrant, multi-vendor ecosystem.

## SaaS/Hosted Platforms

| Platform | Company Scale (Valuation / Revenue) | Starting Pricing (Paid Tier) | Free Tier Limits | Key Capabilities & Trade-Offs |
| :--- | :--- | :--- | :--- | :--- |
| **Postman** | **$5.6B valuation** (~$300M+ ARR) | **$19/user/month** (Team plan, billed annually) | **Free Forever Plan**: 1 user (solo developer), up to 3 collection runs/month in cloud, limited mock server calls, and 50 Postbot AI credits/month. | Dual documentation paths (native Postman docs via Postbot or full AI docs sites via Fern integration). Broad API testing and management suite. |
| **Mintlify** | **$500M valuation** (~$45M Series B, ARR in multi-millions) | **$450/month** (Pro plan, billed annually) | **Free Forever Starter Plan**: Up to 5 editor seats, 1 custom domain, Git sync, MCP server, and standard API playground. AI agent authoring is plan-gated to Pro/Enterprise. | Full docs-as-code platform with agentic AI writer that opens GitHub PRs or directly commits. Static agent egress requires Enterprise. |
| **SwaggerHub** (SmartBear) | **~$250M+ ARR** (SmartBear parent, PE-backed by Vista & Francisco Partners) | **$29/user/month** (Team plan, billed annually) | **14-day free trial** of Team/Enterprise tier (Open-source Swagger Editor/UI/Codegen tools remain freely self-hosted). Free individual tier capped at 10 APIs and 1 public portal product. | Natural language portal page creation (Portal AI), visual OpenAPI design, and team standardization. AI page generation capped at 10,000 lines of OpenAPI reference. |
| **Stoplight** (SmartBear) | **~$250M+ ARR** (Acquired by SmartBear in 2023) | **$44/month** (Basic plan, billed annually; or $56/month monthly) | **Free Forever Community Plan**: 1 user seat, 1 active project, visual OpenAPI designer, instant mock server, and basic hosted docs. | Design-first API documentation with visual OpenAPI editing, Prism mocking, and Spectral style linting. Less specialized AI authoring depth than newer agent-native platforms. |
| **ReadMe** | **~$36M valuation** (~$10M–$12M ARR) | **$250/month** (Pro plan, billed annually; includes 5 seats) | **Free Forever Starter Plan**: 1 admin seat, 1 project, 1 published API version, and 7-day analytics retention. Ask AI reader assistant requires a $150/mo add-on. | AI Agent in the editor with model picker (Claude Opus, Gemini, GPT), codebase indexing, OpenAPI alignment, and multi-page auditing. |
| **Fern** | **Acquired by Postman** ($13M prior funding raised) | **Custom Enterprise quote** (Intermediate documentation tiers streamlined to Free + Enterprise) | **Free Forever Plan**: Up to 10 team members, 1 documentation site, custom domain, and 250 AI credits/month (Ask Fern costs 2 credits/msg, AI examples cost 1 credit). | Docs-as-code platform with native SDK generation and automated `llms.txt` / Markdown optimization for external AI agents. Slack docs updates consume 50 credits/session. |
| **GitBook** | **Bootstrapped / Lean** (~$3.7M–$4M ARR) | **$65/site/month + $12/user/month** (Essential plan, billed annually) | **Free Forever Plan**: 1 user seat, standard `gitbook.io` subdomain (no custom domain), and 10 GitBook Agent messages/week. | Visual and markdown collaboration with Git sync; GitBook Agent writes docs, translates, flags styleguide issues, and participates as a reviewer in change requests. |
| **Scalar** | **Venture-backed** (General Catalyst, Abstract Ventures; early-stage ARR) | **$125/month** (Pro plan, billed annually; or $150/month monthly) | **Free Forever Plan**: 1 editor seat, up to 3 APIs in registry, SDK support up to 25 endpoints (1 language target), and 50 Agent Scalar AI credits. | Modern, lightweight OpenAPI reference renderer and API client; offers hosted developer portals and SDK generation, plus an MIT open-source version. |
| **Redocly** | **Venture-backed / Private** (Early-stage ARR) | **$249/month** (Pro plan, billed annually; includes 3 projects) | **30-day free trial** of hosted Pro/Scale platform. Permanent free usage available via open-source Redoc CE (renderer) and Redocly CLI (linter/bundler). | API documentation platform featuring in-site AI assistant, full MCP server support (`/mcp`), and automated `llms.txt` export. Advanced platform governance requires Scale/Enterprise. |





## Open-Source GitHub Projects



- **Apimatic**

  **Generate Markdown API docs from source code with optional AI enhancement** (MIT) — **the most practical open-source tool for source-to-Markdown API documentation** found in this research . **Features**: **Scans Flask, FastAPI, and other frameworks** to generate comprehensive Markdown API docs . **AI enhancement is optional**—use local **Ollama** (phi3:mini, llama3:8b) for privacy, or **OpenAI** (gpt-4o-mini), **Google Gemini** (gemini-1.5-flash), or **Groq** (llama3-8b-8192) for speed . **Config commands** store API keys securely in your home directory . **Generation options** include `--src`, `--framework`, `--format markdown`, `--output`, and model selection flags . **Tech stack**: Python (PyPI). **Deploy**: `pip install Apimatic`; `apimatic generate --src . --output API_Docs.md` . **Trade-off**: **Markdown only**—no HTML rendering, no search, no site hosting; you bring the docs platform. **Best for**: developers wanting to generate Markdown API docs from source code with local or cloud LLM enhancement—especially those wanting privacy via Ollama or speed via Groq.



- **printing-press (ppress)**

  **Agentic-first OpenAPI documentation generator** (Go) — **the most complete open-source tool for turning OpenAPI into agent-ready static docs** . **Features**: **Works 100% offline**—open generated docs from disk, zip them, or share as an archive; publish to any static host (GitHub Pages, S3, Netlify, Cloudflare Pages) . **AI and agent output built in**—`AGENTS.md`, `llms.txt`, per-operation and per-model Markdown, plus JSON artifacts . **API catalogs** from directories of OpenAPI specs with multi-version awareness; **integrated diagnostics** via vacuum reports rendered inline; **Mermaid/UML class diagrams** auto-generated for complex schemas . **Tech stack**: Go. **Deploy**: `curl`, npm, Homebrew, Go install, or Docker; `ppress ./openapi.yaml` . **Trade-off**: **Static docs only**—no hosted platform, no built-in search (browser-native only), no AI authoring agent. **Best for**: teams wanting fully offline, agent-ready OpenAPI docs they can host anywhere—especially those who need `llms.txt` and `AGENTS.md` without a SaaS platform.



### Additional Strong Open-Source Options



- **Scalar (open source)** — OpenAPI reference and API client (MIT). Clean rendering, widely adopted. **Note**: **Rendering component, not a generator**—no AI authoring or Markdown generation. **Best for**: embedding an OpenAPI reference in an existing site.

- **Redoc** — OpenAPI reference renderer (MIT). Generates three-panel API docs from OpenAPI specs. **Note**: **Renderer, not an AI generator**—no authoring capabilities. **Best for**: rendering OpenAPI specs as static docs.

- **Docusaurus** — Static site generator for documentation (MIT). **Note**: **Site framework, not an API doc generator**—no OpenAPI parsing or AI authoring; pair with plugins. **Best for**: building a custom docs site where you control every component.



**Frameworks for building custom systems**: Combine **Apimatic** for source-to-Markdown generation with **printing-press** for OpenAPI-to-agent-ready static docs and **Scalar** for rendering—creating a composable open-source AI docs stack. **None of these match Mintlify's PR-based agent or ReadMe's multi-page audit**, but for generation and agent exposure, the options are production-capable.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI documentation platforms handling API specifications and source code must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls and IP protection.

- **The "agentic authoring" vs. "AI-assisted page creation" vs. "source-to-Markdown generation" vs. "OpenAPI-to-static-docs" vs. "rendering" distinction is critical.** **Mintlify, ReadMe, GitBook, and Fern** are **agentic authoring** platforms—their agents research, plan, write, and open PRs with proposed changes . **SwaggerHub** offers **AI-assisted page creation**—natural language prompts generate Portal pages, capped at 10K-line API references . **Apimatic** is **source-to-Markdown generation**—it scans code and generates Markdown with optional LLM enhancement . **printing-press** is **OpenAPI-to-static-docs**—it generates offline docs with agent artifacts . **Scalar and Redoc** are **renderers**—they display OpenAPI specs but do not author or generate content. **Choose based on whether you need an agent, page generation, Markdown generation, static docs, or rendering.**

- **Mintlify's agent is plan-gated to Pro or Enterprise**—it opens PRs for review or commits directly if you trust it . **The trade-off**: static egress for IP allowlists requires Enterprise .

- **ReadMe's Agent is on Pro plans**—Starter gets limited complimentary answers . **The model picker (Claude Opus 5, Gemini 3.8 Flash, GPT5.6 Terra) and codebase indexing are the differentiators**—it can audit across multiple pages in one prompt .

- **GitBook Agent is free while in beta**—10 messages/week on non-Pro plans; translations cost extra . **The change-request workflow and `@gitbook` comment summoning are unique**—it responds to feedback within the change request .

- **Fern's AI credits are metered per feature**—Ask Fern is **2 credits/message**, AI examples **1 credit**, Slack docs update **50 credits/session** . **Every site automatically hosts `llms.txt` and serves Markdown to AI agents**—no configuration needed .

- **SwaggerHub's AI page creation is capped at 10,000 lines of API reference**—larger APIs must be split . **Do not assume it handles large enterprise specs in one pass.**

- **Apimatic is the most practical open-source source-to-Markdown generator**—scans Flask/FastAPI, generates Markdown, and supports local Ollama for privacy or cloud LLMs for speed . **The trade-off**: Markdown only—no rendering or hosting.

- **printing-press is the most complete open-source OpenAPI-to-static-docs tool**—fully offline, agent artifacts (llms.txt, AGENTS.md), Mermaid diagrams, and vacuum diagnostics . **The trade-off**: static only—no hosted platform or search.

- Self-hosted open-source solutions require proper setup (Python for Apimatic, Go for printing-press) and ongoing maintenance. **API documentation tools process proprietary specifications and source code**—ensure your deployment meets your organization's IP protection and security requirements before processing production assets.



---



**Made for API documentation teams, developer experience engineers, and organizations building transparent AI-generated documentation solutions.**

Let's make AI-Generated API Documentation more open, data-driven, and agent-ready.
