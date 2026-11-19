# Rakshit Tikoo

Chip design engineer building small, single-purpose open-source tools — each one solves one repeated pain and is documented with its own measured limits. All of them are MIT-licensed and free.

## Agent & code safety

- **[skillscan](https://github.com/RakTikoo/skillscan)** — Deterministic, offline scanner for AI-agent skills and MCP servers — check a skill before you install it. Zero dependencies, no LLM, nothing leaves your machine.
- **[stranger-suite](https://github.com/RakTikoo/stranger-suite)** — Fresh-eyes testing for AI agents — tests whether your README actually works for a newcomer, and probes your API the way a stranger would. Bring your own key.
- **[phantomdep-pr-gate](https://github.com/RakTikoo/phantomdep-pr-gate)** — GitHub Action that flags phantom dependencies in pull requests — packages that don't exist, are brand new, or are barely downloaded.
- **[ci-command-truth](https://github.com/RakTikoo/ci-command-truth)** — Checks that the commands in your CI workflows actually exist — catches renamed scripts and phantom targets before CI does.
- **[handoff-reconciler](https://github.com/RakTikoo/handoff-reconciler)** — Verify AI coding-session handoffs against git ground truth — freeze a structured handoff, then get a traffic-light drift report at resume.
- **[living-contract-diff](https://github.com/RakTikoo/living-contract-diff)** — Learn what your API actually returns from recorded traffic, then diff that observed contract against your OpenAPI spec (JSON or YAML) and report the drift.

## Boards & files

- **[kicad-preflight](https://github.com/RakTikoo/kicad-preflight)** — Pre-order checker for KiCad PCB projects — BOM, Gerber package, netlist/ERC-lite and schematic-PCB parity checks that catch what DRC misses before you order.
- **[expiry-radar](https://github.com/RakTikoo/expiry-radar)** — Certificate expiry checker and GitHub Action — watches certificates, JWTs, JWKS and tokens in your repo and opens an issue before they expire.

## Astronomy

- **[epochmatch](https://github.com/RakTikoo/epochmatch)** — Cross-match two star catalogues from different epochs (CSV, VOTable, FITS), propagating positions to a common epoch with proper motions before matching; reports matched, unmatched and ambiguous pairs.
- **[bjd](https://github.com/RakTikoo/bjd)** — Convert a column of observation times in a CSV or FITS table to BJD_TDB (barycentric Julian date). The input format and time scale must be stated — the tool refuses to guess, so times are never silently shifted.
- **[fitslog](https://github.com/RakTikoo/fitslog)** — Turn a folder tree of telescope FITS files into one night-log CSV, with header keywords normalised across instruments and an audit of problem files. Headers only; runs offline.
- **[tonight](https://github.com/RakTikoo/tonight)** — Plan one night of telescope observing: a CSV of targets, a site and a date in — a ranked plan with observable windows, best times and Moon separation out. Runs offline.
- **[fitspeek](https://github.com/RakTikoo/fitspeek)** — Turn a folder of FITS image files into contact-sheet PNGs stamped with header details, plus an index mapping every thumbnail back to its source file.

## Medicine & research data

- **[egfr-batch](https://github.com/RakTikoo/egfr-batch)** — Batch-compute eGFR from a CSV of age, sex and creatinine with the published CKD-EPI 2021 equations (creatinine and creatinine-cystatin C). The creatinine unit must be declared — the tool refuses to guess. Research/educational only; not a medical device.
- **[labunits](https://github.com/RakTikoo/labunits)** — Batch-convert a lab-results CSV between conventional (US) units and SI units for 60 analytes, each factor verified against two authorities; analytes with no single verified factor are refused, with the reason. Research/educational only; not a medical device.
- **[growthz](https://github.com/RakTikoo/growthz)** — Batch-compute CDC growth z-scores and percentiles for a whole CSV of child measurements, using the CDC 2000 LMS method and the CDC's own published tables. Research and educational tool only; not a medical device.
- **[safeharbor-check](https://github.com/RakTikoo/safeharbor-check)** — Check a structured CSV against the HIPAA Safe Harbor identifier classes (45 CFR 164.514(b)(2)) — a checker only, it certifies nothing.
- **[blockrandom](https://github.com/RakTikoo/blockrandom)** — Generate seeded permuted-block randomization lists for small clinical trials — allocation list, sealed enrolment list, per-stratum files, an audit log and a methods paragraph, reproducible byte-for-byte from the seed. Research/educational tool; not a medical device.

## Game art

- **[seamproof](https://github.com/RakTikoo/seamproof)** — Makes a texture or a whole PBR texture set tile seamlessly, with a measured seam score. Applies one shared fix to albedo, normal, roughness and height maps so the set stays in register.
- **[patchproof](https://github.com/RakTikoo/patchproof)** — Finds the 9-slice (nine-patch) borders of game UI panel PNGs and proves each detection by re-rendering. Writes Unity spriteBorder .meta files, Godot StyleBoxTexture .tres files and Android .9.png files for proven panels.
- **[snapgrid](https://github.com/RakTikoo/snapgrid)** — Recovers the pixel grid from damaged pixel art — sprites upscaled with smoothing, AI-generated or JPEG-damaged — and snaps them back to clean pixel art with one shared grid and palette. Abstains when no grid can be proven.

## Format checkers

- **[adifcheck](https://github.com/RakTikoo/adifcheck)** — Check a ham-radio log's contents against the ADIF 3.1.8 spec — the values LoTW/eQSL reject — before you upload.
- **[dwccheck](https://github.com/RakTikoo/dwccheck)** — Check a Darwin Core occurrence file locally, before you upload it to GBIF — GBIF's own flag names, offline, no dependencies.
- **[icslint](https://github.com/RakTikoo/icslint)** — Lint .ics calendar files against RFC 5545 — a local CLI with 67 cited rules. No recurrence expansion, no guessing.

## Install

Every tool installs from GitHub with pip, pipx or uv — each repo's README gives the exact command for that tool. Seventeen of them are also in my own [Homebrew tap](https://github.com/RakTikoo/homebrew-tools) and [Scoop bucket](https://github.com/RakTikoo/scoop-bucket).

## Contributing

Starter tasks are labelled "good first issue" in each repo, and the whole list is collected at [goodfirstissue.org/RakTikoo](https://www.goodfirstissue.org/RakTikoo).
