# Model-Number Tag Cheat Sheet — where the tag lives, and how to read it

Everything in this directory starts with one string of characters: **the full model number**, read *exactly* as printed. Get it right and every search on every site works twice as fast. Get it wrong and you'll spend twenty minutes chasing ghosts.

## The golden rule

> **The model number is what's on the tag, not what's on the box, not the marketing name, and not the serial number.**

Two examples worth memorizing:

- The marketing name says **"Whirlpool 5.0 cu. ft. Smart Front Load Washer"** — useless for lookup.
- The tag says **`WFW9620HC` (model) / `HC9182345` (serial)** — the model is what you search.

Also: *read every character*. A trailing digit like `...Z0` or a leading prefix can be the difference between two product variants. If a search with the model number fails, check for:

- A **suffix digit** you mistyped (`...Z0` vs `...Z1`)
- **Similar characters**: `0` (zero) vs `O` (letter), `1` vs `I` vs `l`, `5` vs `S`, `8` vs `B`
- A **serial-looking string you used by mistake** — serial numbers come *after* the model number on the tag and are usually longer

## Where the tag lives, by appliance

| Appliance | Common tag spots |
|---|---|
| Refrigerator | behind the fresh-food door, upper wall; or near the crisper drawers on the side wall; some side-by-side models: inside face of the freezer door frame |
| Dishwasher | left or right side of the inner door edge — you have to open the door; sometimes under the door on the tub frame |
| Washer (top-load) | under the lid, near the top back rim; or back of the control panel area |
| Washer (front-load) | inside the door opening, on the door jamb or drum frame |
| Dryer | inside or just below the door opening on the frame; sometimes back panel |
| Oven / range | on the drawer or frame edge in front, or near the burner controls; also behind an oven door jamb edge |
| Microwave (built-in) | inside the door jamb frame; countertop units: bottom of the cabinet or back panel |
| Air conditioner (window) | side or back of the case; built-in units: front frame behind the filter |
| Furnace / air handler | inside the blower door front panel, right on the blower housing or cabinet |
| Water heater | the rating plate on the outside or, for some gas units, behind the access door near the burner |
| Vacuum | lower back of the body or on the bottom plate |
| Power tool (cordless/drill) | on the motor housing back or battery-side plate; sometimes on the bottom of the handle |
| Table saw / stationary tools | somewhere on the frame rib or side housing |
| Mower | under the throttle handle or beneath the seat |
| Chainsaw | under the bar and chain guard cover or on the top housing |

If a spot above doesn't pan out, check the *opposite* side of the appliance from the control panel — manufactures love that.

## How to decode a typical tag

A tag usually packs several strings. Here's a real-looking layout for reference:

```
MODEL: WFW9620HC          ← your search string
SERIAL: HC9182345         ← useful for service, useless for manual lookup
TYPE: BF49-35L            ← often ignored type code, don't confuse with model
```

Order of operations:

1. The **model** is the entry labeled `MODEL`, `MOD`, or `MODEL NO.`.
2. **Serial** (`SERIAL`, `SER`, `S/N`) tells you the manufacture date — occasionally you need this to pick a manual revision. It is *never* the search key.
3. Extra codes (`TYPE`, `CODE`, `ENR`, `STYLE`) — ignore for manual searches, but note them in your log if you had to pick between revisions.

Armed with the model number, go to `manufacturers.md` and work down the chain, then `search-patterns.md` when needed. Then log the outcome in `hunting-log.csv`.
