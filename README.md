# Aidin Nemati

Engineer building and operating production web systems, automation tooling, and quantitative research infrastructure — with verification as the default mode.

## About

I build software end-to-end: React/TypeScript front-ends, Node and Python back-ends, deployment and operations. The through-line in everything public here is proof: test suites that run, gates that block bad releases, and honest documentation of what has been verified, what is historical, and what is still unproven. Systems I run in production include payment failover, transactional inventory, verified backups, and monitoring that pages a human when something breaks.

## Featured Projects

- **[Janebi-Store](https://github.com/MrRooobooot/Janebi-Store)** — production full-stack e-commerce for a Persian/RTL store: React 19 + Express 5 + Drizzle over SQLite, payments with automatic gateway failover, anti-overselling transactions, restore-verified backups; live at [janebiarena.ir](https://janebiarena.ir), CI-gated by a 534-test suite.
- **[quant-research-lab](https://github.com/MrRooobooot/quant-research-lab)** — quantitative research as a falsification lab: fee-wall analysis, walk-forward ML, out-of-sample replays, and a documented correction chain in which the negative result is the deliverable (virtual funds only).
- **[novin-khodro](https://github.com/MrRooobooot/novin-khodro)** — car-dealership web platform built with zero runtime dependencies: ~15k lines of vanilla JS/CSS plus a purpose-built, npm-free 475-check test framework that runs in ~0.5 s.
- **[ikco-profile-harvester](https://github.com/MrRooobooot/ikco-profile-harvester)** — resilient single-file scraper for a public product catalogue behind an F5 WAF: bounded pacing, cooldowns, resume-safe runs, structured JSON output.
- **[shimi-app](https://github.com/MrRooobooot/shimi-app)** — Telegram Mini Apps plus a Cloudflare Worker handling a channel bot's webhook, KV-backed bookings, and ops self-healing for a chemistry-education channel.

## Engineering Themes

- **Verification-first development** — every serious project ships with its own evidence: a local verify gate (`typecheck → tests → build → live probes`) on Janebi-Store, a 475-check dependency-free framework on novin-khodro, assert-based self-checks on the smaller tools (10/10 on both quant-research-lab and the harvester).
- **Failure analysis over failure hiding** — CI red for five consecutive pushes root-caused to an environment mismatch; a leaked credential tracked as a rotation action rather than "fixed" by deletion; a withdrawn +78% backtest figure corrected to +111.21% with both versions documented.
- **Operations as code** — hash-sealed release identity, nginx drift diffs, backup scripts that verify by restoring, health monitors with alerting, log-checked cron jobs.
- **Automation and data pipelines** — WAF-aware crawling with resume semantics; price-sync and ROI reporting pipelines; media and PDF capture with id-normalized naming and resumable downloads.
- **Research discipline** — chronological folds, purged splits, fee-first acceptance criteria, and a rule that a rejected strategy is never re-litigated without new evidence.

## Selected Evidence

- Janebi-Store: **534 tests in 68 files**, CI green; live production verified (HTTP 200, database ok, catalog serving).
- novin-khodro: **475/475 checks, ~0.5 s, exit 0** — on a test framework with no npm dependencies.
- quant-research-lab: **10/10 safety self-checks**, plus a public record of every failed experiment and every correction.
- ikco-profile-harvester: **10/10 self-checks** on the published package.
- All repositories: secret scans (gitleaks full-history where applicable) and sanitization gates run before publication.

## AI-Assisted Engineering

AI agents are part of my engineering toolchain — used for implementation, debugging, test scaffolding, documentation, and repetitive automation — under human-directed architecture and verification. Every claim published in these repositories is checked against real execution (tests, probes, CI, production behavior), not model output. This is deliberately not the same as an AI product: Janebi-Store, novin-khodro, and the shimi pages are conventional systems; quant-research-lab's live paper-trading panel explicitly *removed* LLM automation from its execution path in favor of a deterministic watchdog. AI assistance in development, not AI in the runtime.

## Engineering Philosophy

- Evidence over assumptions.
- Tests over intuition.
- Production behavior over local claims.
- Documented failures over hidden ones.

## Current Focus

- Operating and hardening the live Janebi-Store deployment (payments, backups, monitoring).
- Extending the falsification-driven research methodology in quant-research-lab.
- Building small, verifiable automation tools (harvesters, pipelines, probes).

## Tech Stack

- **Languages:** TypeScript, JavaScript, Python, SQL, Shell
- **Frontend:** React 19, Vite, Tailwind CSS, vanilla JS/CSS (zero-dependency builds)
- **Backend:** Node.js, Express 5, Zod, Drizzle ORM, SQLite (WAL, FTS5), PostgreSQL
- **Research/Data:** Python data pipelines, LightGBM experiments, backtesting harnesses
- **Infra/Ops:** Docker Compose, nginx, Let's Encrypt, Cloudflare Workers, GitHub Pages, GitHub Actions, launchd-supervised services
- **Quality:** Vitest, Supertest, Playwright, gitleaks, custom security gates and live probes, zero-dependency test framework

## Links

- GitHub: [@MrRooobooot](https://github.com/MrRooobooot)
- Live production: [janebiarena.ir](https://janebiarena.ir)
