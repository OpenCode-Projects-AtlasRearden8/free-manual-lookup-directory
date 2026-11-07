# Free Manual Lookup Directory

**A curated directory for finding free appliance and tool manuals — so you only hunt once.**

You just moved into a place with a mystery dishwasher. Or you inherited your grandpa's table saw with no book. Or your fridge started making The Sound and you need the manual *now*.

This directory is your starting map. It tells you:

- Where the manufacturers themselves host the PDFs (the best source, always)
- Which archived manual libraries are worth your time
- Simple search patterns that work when the "official" site fails you
- How to read the model-number tag on almost any appliance
- A logging sheet, so the next time you need that manual, you don't re-hunt — you just open your log

No uploads, no accounts, no personal data. Just plain links with quick, honest notes on how reliable each source is.

## Who this is for

Anyone who owns things with moving parts and would like to keep them moving. Renters, homeowners, DIYers, resellers, and people who'd rather fix it than replace it. Everything here is written like a friend would explain it — plain English, step by step, never condescending.

## What's in this folder

| File | What it does |
|---|---|
| [`manufacturers.md`](manufacturers.md) | Where each major brand houses its own free PDF manuals, with direct entry points |
| [`archives.md`](archives.md) | Third-party manual libraries and archives, rated for reliability |
| [`search-patterns.md`](search-patterns.md) | Spec-sheet search patterns: query templates that find manuals fast |
| [`model-number-tags.md`](model-number-tags.md) | Cheat sheet: where the model tag lives on each appliance, and how to read it |
| [`hunting-log.csv`](hunting-log.csv) | The logging sheet. Log it once, never hunt again |

## How to use it (the short version)

1. **Find the model number first.** Check [`model-number-tags.md`](model-number-tags.md) for where the tag hides on your appliance type.
2. **Try the manufacturer's own site.** Check [`manufacturers.md`](manufacturers.md) for the direct search page. This is the gold standard: newest revision, free, no sketchy ads.
3. **If the manufacturer dead-ends** (discontinued product, absorbed brand, broken search), go to [`archives.md`](archives.md) and try the top-rated archive.
4. **If both fail**, use a search template from [`search-patterns.md`](search-patterns.md) — these find PDFs other people have hosted.
5. **Log it.** Open `hunting-log.csv`, add one row: model number, what you found, where the PDF lives. Done. Hunting once is the whole point.

## The hunting log, column by column

`hunting-log.csv` is a plain spreadsheet you can open in Excel, Google Sheets, LibreOffice, or any text editor. One row per hunt:

| Column | What to put here |
|---|---|
| `item_type` | `appliance`, `tool`, `hvac`, `water heater`, `small appliance`, or whatever else you classify |
| `brand` | Manufacturer name from the tag |
| `model_number` | The **full model number**, exactly as read off the tag |
| `serial_number` | Optional — useful when a manual revision depends on it |
| `document_found` | What you got: owner's manual, install guide, service manual, spec sheet |
| `source_url` | The link that actually worked |
| `source_type` | `manufacturer`, `archive`, `search`, or `parts site` |
| `reliability_note` | One-word verdict: `reliable`, `flaky`, `ad-heavy` |
| `found_via` | How: "manufacturer owner center", "search pattern 2", and so on |
| `date_found` | `YYYY-MM-DD` |
| `vault_location` | Where you keep the PDF locally — a folder path or notebook name. No personal info needed: a folder-relative path like `Appliances/Washer/WFW9620HC` is enough |
| `status` | `found` or `not found` — a `not found` entry saves future-you an hour |
| `notes` | Anything else: wrong revision warnings, suffix gotchas, "site search broken, used pattern 4" |

The two example rows are placeholders — overwrite or delete them.

## Distinct from its siblings

This directory intentionally does **not** cover:

- **Free everyday software** (apps and programs) — that lives in the separate `free-everyday-software-directory` project
- **Download/file organization** (how to file what you download) — that lives in the `download-organization-kit` project

Here we only answer: *where is the free manual for this specific machine?*

## Reliability notes, honestly

Every source in this directory has a quick reliability note with two numbers, like **(reliability: 9/10, last checked: 2026-11)**. As of the last check, all links pointed at real sites and the manufacturer pages listed below were live and searchable. Third-party archives move more often than manufacturer sites, so their ratings are more conservative.

Nothing here is affiliated with any manufacturer. Trademarks belong to their owners; we're just pointing at doorways.

## Safety, in one breath

Manuals tell you how machines work, not whether *you* should work on them. Gas appliances, anything wired in, and anything with a sealed refrigeration loop deserve a professional. Read the manual, know the machine, and when in doubt, call someone licensed. This directory is general information, not repair or safety advice for your specific situation.

## About this project

Built by **Asdale Dynamics, LLC** — Dylan Asdale's shop for beginner-friendly AI education, books, and practical tools that respect your time. Plain English, step by step, never condescending. Learn more at <https://dylanasdale.github.io>.

## License

MIT — see [`LICENSE`](LICENSE). Copyright (c) 2026 Asdale Dynamics, LLC.
