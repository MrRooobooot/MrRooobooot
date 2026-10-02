I build and operate production web systems — React/TypeScript front-ends, Node and Python back-ends, deployment and operations. What I publish is checked against real execution — tests, CI, live deployments — with notes on what is verified, what is historical, and what is still unproven. Preferred defaults when nothing else dictates: TypeScript on Node, SQLite or Postgres, dependency-light tooling — and as few moving parts as possible.

![JanebiArena — live product page (Persian/RTL)](https://raw.githubusercontent.com/MrRooobooot/Janebi-Store/main/docs/screenshots/product-page-light.png)

## Featured Projects

- **[Janebi-Store](https://github.com/MrRooobooot/Janebi-Store)** — production full-stack e-commerce for a Persian/RTL store (React 19 + Express 5 + Drizzle over SQLite), live at [janebiarena.ir](https://janebiarena.ir). Gateway-failover payments, anti-overselling inventory transactions, restore-verified backups; CI-gated by 534 tests in 68 files.
- **[quant-research-lab](https://github.com/MrRooobooot/quant-research-lab)** — falsification-first research: fee-wall analysis, walk-forward ML that failed to beat costs, out-of-sample replays, and a documented correction chain of its own findings. The negative result is the deliverable; paper trading only.
- **[ikco-profile-harvester](https://github.com/MrRooobooot/ikco-profile-harvester)** — single-file Python harvester for a public product catalogue behind an F5 WAF: bounded pacing, cooldowns on blocks, resume-safe runs, structured JSON output.
- **[shimi-app](https://github.com/MrRooobooot/shimi-app)** — Telegram Mini Apps plus a Cloudflare Worker running a channel bot's webhook: quiz and planner pages, PDF study assets, KV-backed class bookings; pages served from GitHub Pages.
- **[novin-khodro](https://github.com/MrRooobooot/novin-khodro)** — car-dealership web platform with zero runtime dependencies: ~15k lines of vanilla JS, CSS, and HTML plus a purpose-built, npm-free test framework (475 checks, ~0.5 s); sanitized snapshot, not publicly served.

## How I Work

- **Verification over claims** — projects ship with their own evidence: a local gate (typecheck, tests, build, live probes), assert-based self-checks, or a purpose-built test framework.
- **Production-minded** — hash-sealed release identity, restore-tested backups, health monitors that alert instead of failing silently.
- **Failures stay documented** — rejected strategies and corrected numbers remain in the record instead of being quietly tuned away.

## AI-Assisted Engineering

AI agents are part of my development toolchain — implementation, debugging, test scaffolding, and documentation — under human-directed architecture and review. Shipped systems are validated by tests and real-world behavior.

## Current Focus

- Operating and hardening the live JanebiArena deployment — payments, backups, monitoring.
- Extending the falsification-driven methodology in quant-research-lab.
- Building small, verifiable automation tools.
