# MAD × LUMEN — From Vision to Market

Interactive version of the MAD × LUMEN brand development & execution deck
(*MAD_LUMEN_Creative_Universe_v2*), built as a single self-contained page.

**Client:** MAD — founder-led women's ready-to-wear brand (Madawi), Saudi Arabia / GCC
**Partners:** LUMEN (strategy, product, sourcing, production) · White Rabbit Hole (creative, digital, identity, AI workflows)

## Structure

Ten chapters, matching the original deck one-to-one:

| # | Chapter | Source slides |
|---|---------|---------------|
| 00 | Cover | 01 |
| 01 | The vision | 02 |
| 02 | References | 03 |
| 03 | Creative universe | 04–09 |
| 04 | First collection | 10 |
| 05 | Capabilities | 11 |
| 06 | The team | 12 |
| 07 | The journey | 13–18 |
| 08 | One MAD piece | 19 |
| 09 | Ready for launch | 20 |

## Interaction

- Sticky chapter index with scroll-spy, `←` / `→` keyboard navigation, scroll progress bar
- Creative territories filterable by theme (Flower / Soft architecture / Abaya editions / Afterglow)
- Full-screen lightbox with keyboard navigation, scoped to the active filter
- Reference cards expand on click
- Journey timeline: phase switch + 8 selectable steps, each opening its own detail panel
- Print stylesheet: every section expands and paginates

## Access gate

Disabled by default. To switch it on, in `index.html`:

```js
const REQUIRE_CODE = true;
```

To change the code, generate a new hash and paste it into `CODE_HASH`:

```bash
printf '%s' 'YOURCODE' | shasum -a 256
```

The current hash corresponds to `MAD2026`. This is a light client-side gate — it keeps
the page out of casual reach, it is not a security boundary.

## Assets

`assets/img/` — 11 garment visuals + hero, extracted from the source PDF and converted to
WebP (12 MB → 1.1 MB). All garment visuals are **AI-generated creative explorations**, not
photographs of finished product; the page states this in the closing disclaimer.

## Local preview

```bash
python3 -m http.server 4173
```

No build step, no dependencies, no external requests.
