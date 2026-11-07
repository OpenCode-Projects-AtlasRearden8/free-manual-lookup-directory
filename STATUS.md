# STATUS.md — Free Manual Lookup Directory

## What was built

A curated, content-only directory for finding free appliance and tool manuals, built for Asdale Dynamics, LLC. No code to run — this is a local-first reference and worksheet kit that works out of any folder, spreadsheet program, or plain text editor.

| File | Purpose | Size |
|---|---|---|
| `README.md` | Overview, 5-step workflow, log column guide, sibling-project separation, safety note | ~120 lines |
| `manufacturers.md` | Direct entry points to manufacturer-hosted PDF manuals for ~25 brands across appliances, HVAC, tools, and small appliances, each with a reliability rating and last-checked date | ~95 lines |
| `archives.md` | Third-party manual libraries (Internet Archive manual collection, ManualsLib, parts-site lookups, etc.) with honest reliability notes; explicit "we deliberately leave out" section for ad-walled and upload-gated sites | ~55 lines |
| `search-patterns.md` | 8 copy-paste search templates (exact-model + filetype, spec-sheet pairing, site-restricted, vintage/Archive patterns) plus an ordered playbook and result-vetting guidance | ~85 lines |
| `model-number-tags.md` | Cheat sheet for where the model tag hides on ~15 appliance/tool types, how to distinguish model vs serial numbers, and 4 common misread traps | ~70 lines |
| `hunting-log.csv` | Plain CSV logging sheet (13 columns) with 2 placeholder example rows so a real hunt can start immediately | 3 rows |
| `LICENSE` | MIT, copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC` | — |
| `STATUS.md` | This file | — |

Distinct from `free-everyday-software-directory` (apps) and `download-organization-kit` (filing), as specified.

## How to run/use it

Nothing to install. Typical flow:

1. Open `model-number-tags.md` to find the model tag on your machine and read it exactly.
2. Open `manufacturers.md` for the brand's own manual portal (best source).
3. If that dead-ends, use `archives.md`, then the numbered search patterns in `search-patterns.md`.
4. Record the outcome in `hunting-log.csv` (opens in any spreadsheet app or text editor).

## Verification results (all run locally on 2026-11)

- **Structure check**: all 6 content files present and referenced correctly — `README.md` link table matches actual filenames (verified via grep; every backticked filename resolves to a real file).
- **CSV integrity check**: `python3 csv.reader` parse of `hunting-log.csv` passes with all rows at exactly 13 columns (found and fixed a column-count bug in an example row during verification).
- **LICENSE check**: grep confirms line 3 is exactly `Copyright (c) 2026 Asdale Dynamics, LLC`; README credits Asdale Dynamics, LLC twice (About + License section).
- **No secrets check**: no API keys, tokens, or personal data in any file; only public manufacturer/archive documentation URLs; log path example is folder-relative with no user-identifying content.
- **Git**: repo initialized in this folder; single commit of all files; no remote configured, nothing pushed or published (per instructions).

## Known gaps

- **Link freshness**: URLs were curated by hand and spot-checked for plausibility at creation (2026-11). Manufacturer sites reorganize support pages occasionally; the per-source "(reliability: X/10, last checked: 2026-11)" notes are meant to be re-dated on a periodic re-verification pass. A future enhancement would be a scripted link checker.
- **No automated tests**: as a pure content artifact, verification is file/structure/parse checks rather than a test suite. If the project grows scripts (e.g., link checker, log validator), those should carry their own tests.
- **Brand coverage is selective**: ~25 major brands are covered; smaller regional, commercial, and non-US brands are not. The search patterns are designed to compensate.
- **Placeholder log rows**: the two rows in `hunting-log.csv` are examples meant to be overwritten, not real hunts.

## Change log

- 2026-11-07 — initial build: all files, LICENSE (MIT / Asdale Dynamics, LLC), README, git init + first commit.
