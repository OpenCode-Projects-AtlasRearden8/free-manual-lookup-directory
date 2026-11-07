# Spec-Sheet Search Patterns — query templates that find manuals

When the manufacturer's search fails or shows you only current SKUs, general web search is your side door. These patterns work in any search engine. Replace `BRAND`, `MODEL`, and `TYPE` with the real values read straight off the tag (see `model-number-tags.md`).

Why these beat typing "manual" into the box alone:

- **Quoted model numbers** force exact matches — this is the single biggest upgrade. Most failed searches happen because the model number got mangled.
- **`filetype:pdf`** goes straight to documents instead of landing pages.
- **`site:`** restricts a search to one domain — perfect when a site's own search engine is broken.

## Core patterns (in order of usefulness)

**1. Exact model, exact file** — start here every time:
```
"MODEL" manual filetype:pdf
```

**2. Manual + spec sheet pair** — manufacturer spec sheets surface manuals as related results:
```
"MODEL" "spec sheet" OR "specifications" filetype:pdf
```

**3. Different revisions** — manuals are revised; asking for the older revision finds documents newer sites no longer link:
```
"MODEL" "rev 1" OR "revision a" manual
```

**4. Site-restricted** — for when the manufacturer's site hides its own PDFs from their search:
```
"MODEL" manual site:whirlpool.com
```
(Repeat for any domain: `site:searspartsdirect.com`, `site:manualslib.com`, etc.)

**5. Parts-diagram side door** — parts databases attach manuals to diagrams. A diagram result can confirm the model number is right even if the manual itself doesn't surface:
```
"MODEL" "parts diagram" OR "parts list"
```

**6. Service & install guides** — the other half of the documentation packet:
```
"MODEL" ("installation guide" OR "service manual") filetype:pdf
```

**7. Archive-restricted vintage pattern** — for pre-internet gear. The Internet Archive scans carry searchable OCR text, so you can find them with ordinary queries:
```
"BRAND" "MODEL" site:archive.org/details/manuals
```

**8. Alternate phrasing** — manuals use different names for the same document; test a few:
```
"MODEL" ("owners manual" OR "user manual" OR "use and care" OR "operator's manual")
```

## Pattern stack (playbook)

Run patterns in this order. Most manuals are found by pattern 1 or 2:

1. `"MODEL" manual filetype:pdf`
2. `"MODEL" "spec sheet" filetype:pdf`
3. `"MODEL" ("owners manual" OR "use and care" OR "operator's manual")`
4. `"MODEL" manual site:manufacturer-domain.com` (from `manufacturers.md`)
5. `"MODEL" "parts diagram"` → follow the parts-site result to their manual attachment
6. `"MODEL" site:archive.org/details/manuals` (vintage or discontinued gear)
7. Search post-verification: read the tag again, in daylight, and check for a suffix you missed (see `model-number-tags.md` — the `-03` factory-suffix mistake is the #1 cause of "manual not found")

## Reading results skeptically

- **Match the suffix exactly.** `WDT750SAKZ0` is not `WDT750SAHZ0`. This kind of silent prefix/suffix swap is the top source of wrong-manual downloads; this character of unsuspicion gets people parts diagrams for the wrong door hinge.
- **Prefer PDFs hosted on manufacturer or archive domains** (`.com` brand sites, `archive.org`) over random file-host mirror pages.
- **Trust workflows, not dates.** A manual from 2014 with the matching model number beats a 2019 PDF for a different model family with the same product name. Manuals attach to *model numbers*, not product-marketing names. People confuse "Galaxy 5000 washer" (marketing name, meaningless) with *actual* model tag text (everything).

## The energy label trick

For appliances and HVAC, the yellow US DOE energy guide labels almost always display the *full model number* in the small footer text. If your physical tag is worn/missing, search:
```
"BRAND TYPE" energy guide label "MODEL"
```
That's often enough to recover the full model number, which you then feed back to patterns 1–4. This trick starts a loop worth knowing; the loop is: **label → model number → manual → log it**.
