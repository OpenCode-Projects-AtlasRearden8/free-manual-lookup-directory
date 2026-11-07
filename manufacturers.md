# Manufacturer Manual Pages — go straight to the source

The manufacturer's own site is always your first stop. Why:

- It hosts the **current revision** of the manual (archives may hold an older print)
- PDFs are usually free, no account, no waiting
- Installation guides, energy spec sheets, and parts lists often live on the same page

Each entry has a quick reliability note: **(reliability: X/10, last checked: 2026-11)**. Reliability means: is the search easy to use, do searches on dead/old models still work, and does the site actually give you a PDF without dark patterns.

## General workflow at any manufacturer site

1. Find their **owner support** / **manuals & documents** / **product support** section.
2. Enter the **model number exactly** (see `model-number-tags.md` — dashes and suffixes matter).
3. Download the **owner's manual / use & care guide**. Grab the **install guide** too if you're mounting anything.
4. Log the link in `hunting-log.csv`.

## Kitchen & laundry (large appliances)

| Brand | Where the manuals live | Notes |
|---|---|---|
| **Whirlpool** | whirlpool.com → Support → Manuals & Literature: <https://www.whirlpool.com/owner-center.html> | Search by model number or product category. Very forgiving search; handles old models well. Main-brand pages also cover Amana, Maytag, KitchenAid, JennAir models. *(9/10, 2026-11)* |
| **Maytag** | maytag.com → Support: <https://www.maytag.com/support.html> | Shares Whirlpool's document system; usually faster to use the Whirlpool owner center for a Maytag model number. *(9/10, 2026-11)* |
| **GE Appliances** | geappliances.com appliance support: <https://products.geappliances.com/appliance/gea-support-search-content?Content_ID=SR-28> | Searchable by model number; also hosts install guides, spec sheets, and energy labels for each model. *(9/10, 2026-11)* |
| **Samsung** | samsung.com support, enter model: <https://www.samsung.com/us/support/downloads/> | Model page hosts manuals, spec sheets, and firmware where relevant. Search needs the exact model code — read it off the tag, don't eyeball it. *(8/10, 2026-11)* |
| **LG** | LG USA product manuals: <https://www.lg.com/us/support/product-help/manufacture-date-lookup/manuals> | Model search returns manuals and support docs. Occasionally splits documents across several downloads. *(8/10, 2026-11)* |
| **KitchenAid** | kitchenaid.com owner center: <https://www.kitchenaid.com/owner-center.html> | Same platform as Whirlpool; covers stand mixers and small kitchen appliances too. *(9/10, 2026-11)* |
| **Bosch** (home appliances) | bosch-home.com service page: <https://www.bosch-home.com/us/service> | Global sites vary; the US service page asks for model number and gives manuals plus repair service docs. *(7/10, 2026-11)* |
| **Electrolux / Frigidaire** | Frigidaire manuals search: <https://www.frigidaire.com/Owner-Center/Product-Support-Manuals/> | Electrolux-owned brand; Frigidaire's portal covers most shared models. *(8/10, 2026-11)* |

## HVAC & hot water

| Brand | Where the manuals live | Notes |
|---|---|---|
| **Carrier** | Carrier residential support: <https://www.carrier.com/residential/en/us/> | Spec sheets, installation, and service documents live on each product/model page; the site search accepts model numbers. Dense but comprehensive. *(7/10, 2026-11)* |
| **Trane** | Trane residential resource search: <https://www.trane.com/residential/en/north-amerika/resource-library/> | Hosts spec sheets, installation guides, and owner documents by product type and model. *(7/10, 2026-11)* |
| **Rheem** | Rheem resources: <https://www.rheem.com/resources/> | Water heaters and HVAC; manuals and install instructions available by model. *(7/10, 2026-11)* |
| **Bradford White** | Bradford White document search: <https://www.bradfordwhite.com/document-search> | Water heaters only. Very good, plain document search — spec sheets and manuals side by side. *(8/10, 2026-11)* |

## Tools (outdoor, workshop, jobsite)

| Brand | Where the manuals live | Notes |
|---|---|---|
| **DeWalt** | DeWalt service & support, search model: <https://www.dewalt.com/service-and-support> | Manuals + exploded parts diagrams. Handles older tools surprisingly well. *(8/10, 2026-11)* |
| **Milwaukee Tool** | Milwaukee service & product manuals: <https://www.milwaukeetool.com/en-us/service-and-support/service-and-repair#product-manuals> | Search by model number or catalog. *(8/10, 2026-11)* |
| **Ryobi** | Ryobi document search: <https://ryobi-support.com/lookup-data/> | Coverage for older models is spotty but the archive of new ones is deep. *(7/10, 2026-11)* |
| **Craftsman** | Craftsman manuals: <https://www.craftsman.com/support/manuals-parts-lists> | Model number search; many older Craftsman tools route into Schematics archives if the page comes up empty. *(6/10, 2026-11)* |
| **STIHL** | STIHL manual library: <https://www.stihlusa.com/manuals/> | Chainsaw and outdoor power manuals, free PDFs, browsable by product. One of the cleanest manufacturer manual libraries out there. *(9/10, 2026-11)* |
| **Toro** | Toro operator manuals: <https://www.toro.com/en/customer-support/interactive-manual> | Enter model/serial; picks the right operator's manual revision. *(8/10, 2026-11)* |
| **Husqvarna** | Husqvarna support & manuals: <https://www.husqvarna.com/us/support/manuals-downloads/> | Model number → manual, parts list, and sometimes repair docs. *(7/10, 2026-11)* |

## Small kitchen & personal appliances

| Brand | Where the manuals live | Notes |
|---|---|---|
| **Cuisinart** | Cuisinart manuals: <https://www.cuisinart.com/support/manuals-literature/> | Browse by category or search; covers older SKUs decently. *(7/10, 2026-11)* |
| **Ninja / Shark** | Shark Ninja customer service: <https://www.sharkninja.com/customer-service/> | Model/serial required; manuals + parts diagrams. Newer products only, mostly. *(7/10, 2026-11)* |
| **Instant Brands** | Instant Pot manuals: <https://instantpot.com/instant-pot-recipes-and-manuals/> | Manuals for the whole Instant Pot line, always free. *(8/10, 2026-11)* |
| **Philips** | Philips support by product: <https://www.usa.philips.com/support> | Search model → manuals + FAQ. Versions vary by region. *(7/10, 2026-11)* |

## If the manufacturer dead-ends

Happens with: discontinued products, brands that got absorbed in appliance-industry mergers, or sites that only list current SKUs. In that order:

1. Try a lookup of the *parent* brand's site (Whirlpool covers Amana/Maytag/KitchenAid; Electrolux covers Frigidaire).
2. Go to `archives.md` for third-party libraries.
3. Use a spec-sheet search pattern from `search-patterns.md`.

And then log the miss in `hunting-log.csv` with `status = not found` — a negative result is still a result. Future-you deserves to know.
