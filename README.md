# Rakshit Tikoo

Chip design engineer building small, single-purpose open-source tools — each one solves one repeated pain, spreads bottom-up, and stays honest about what it can't do.

## Tools

- **[SkillScan](https://github.com/RakTikoo/skillscan)** — deterministic, offline scanner for AI-agent skills and MCP servers. Check a skill before you install it: zero dependencies, no LLM, nothing leaves your machine. Measured on 9,740 labelled skills: 82.4% of malicious skills flagged, 0 false blocks on benign ones.
- **[KiCad Preflight](https://github.com/RakTikoo/kicad-preflight)** — pre-order checks for KiCad PCB projects: BOM, Gerber package, netlist/ERC-lite and schematic↔PCB parity — the order-readiness checks DRC doesn't do.
- **[Expiry Radar](https://github.com/RakTikoo/expiry-radar)** — GitHub Action that watches certificates, JWTs, JWKS and tokens in your repo and opens an issue before they expire.
- **[CI Command Truth](https://github.com/RakTikoo/ci-command-truth)** — verifies the commands in your CI workflows actually exist, before CI finds out they don't.
- **[PhantomDep PR Gate](https://github.com/RakTikoo/phantomdep-pr-gate)** — GitHub Action that flags phantom dependencies in pull requests: packages that don't exist, are brand new, or are barely downloaded.
- **[Stranger Suite](https://github.com/RakTikoo/stranger-suite)** — fresh-eyes API testing for AI agents: bring-your-own-key suites that probe an API the way a stranger would.
- **[Handoff Reconciler](https://github.com/RakTikoo/handoff-reconciler)** — freezes a coding session's claims into a machine-checkable handoff, then verifies every claim against git ground truth when work resumes: MATCH, DRIFT, or BROKEN, claim by claim.
- **[Living Contract Diff](https://github.com/RakTikoo/living-contract-diff)** — learns what your API actually returns from recorded traffic (statistics only, never payload values) and diffs that observed contract against your OpenAPI spec, JSON or YAML, to report drift.

Every tool here is zero-dependency, deterministic, and documented with its own measured limits.
