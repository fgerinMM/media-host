# CTA 2026 — Plenary Session Keynote

Banner artwork announcing the GLASSS keynote in the **Plenary Session** at the
**30° Congresso CTA**.

---

## The event (from the official CTA poster)

| | |
|---|---|
| Event | **30° Congresso CTA** |
| Dates | **30 September – 2 October 2026** |
| City | **Roma** |
| Venue | Centro Congressi Fontana di Trevi — Piazza della Pilotta 4 |
| Theme | *Innovazione, sicurezza, futuro sostenibile: tutte le strade portano all'acciaio* |
| Site | <https://www.ctanet.it> |

## Reference links

| # | Purpose | URL |
|---|---------|-----|
| 1 | CTA — main site | <https://www.collegiotecniciacciaio.it/> |
| 2 | CTA — congress / presentation page | <https://www.collegiotecniciacciaio.it/congressi/presentazione/> |

**Link target for the banner:** link #2. Link #1 is the general reference.

### Logo assets on the CTA site

| Asset | URL | Notes |
|---|---|---|
| Horizontal lockup | `…/uploads/2023/04/logosocial.jpg` | 589 × 172 — **the one used** |
| Square / stacked | `…/uploads/2025/02/Quadrato-1.png` | 1500 × 1500, alpha channel present but 100 % opaque |
| Congress poster | `…/uploads/2026/09/1-scaled.jpg` | 1810 × 2560 — source of the event details above |

There is **no SVG logo** on the site. Every variant is a white-background
raster, so the horizontal lockup was keyed to transparency locally (see
*How the logo was prepared*).

---

## Source document

`20260927_Presentazione CTA_MAFFAIS_REV02 (1).pdf` — the presentation deck.
30 pages, 4.7 MB. REV02, filename dated 27 Sept 2026.

| | |
|---|---|
| This talk | **BARQ-008** — Viadotto Pescara 1 (A25) |
| Format | 5 talks in parallel, 4 days |
| Speaker org | Maffeis Engineering SpA — Via Mignano 26, 36020 Solagna (VI) |
| Partner org | SOIL ENGINEERING Srl — Via San Vigilio 1, 20142 Milano |
| Parallel talks | ZAM-011, FV02ST_2, CALCOLATRICE, PAT-004 |

> ⚠️ The deck's cover says *"Rassegna tecnica — 24-27 settembre 2026"*. That is
> **stale** — the official poster gives **30 Sept – 2 Oct 2026**. Trust the
> poster. The deck also names no speaker and no session, so *"Plenary Session
> Keynote"* is not corroborated by the PDF.

---

## Copy on the banner

| Line | Text | Style |
|------|------|-------|
| Title | `PLENARY SESSION KEYNOTE` | 40px, weight 800, `#164675`, tracking 0.08em, uppercase |
| Sub | `CTA 2026` | 34px, weight 500, `#2166ab`, tracking 0.16em, uppercase |
| When | `24–27 settembre 2026` | 30px, weight 500, `#2166ab`, tracking 0.16em, uppercase |

Class names: `.text-title`, `.text-dates`, `.text-when`. Baselines 116 / 168 / 212.

## Files

| File | Size | What |
|------|------|------|
| `banner.svg` | 20.6 KB | **Vector source — edit this one.** |
| `banner.png` | 81.8 KB | 1600 × 300 render, transparent. For email / HTML only. |
| `20260927_…pdf` | 4.7 MB | The source deck. |

Never hand-edit the PNG. Change the SVG, re-render, overwrite the PNG.

## Spec

- Canvas `1600 × 300`, transparent background
- Enclosure frame: 3px `#2166ab` at 35 % opacity, corner radius 18
- Vertical divider at `x = 800` (exact canvas centre)
- CTA logo at 650 × 168, centred in the left compartment
- Both compartments measured: padding 48/48 (logo) and 72/71 (text)

### How the logo was prepared

The CTA lockup is a JPEG on pure white, so it was converted to alpha locally:
alpha derived from distance-from-white (ramp 6→30), colour un-premultiplied,
then trimmed to the ink box (565 × 146). 88.6 % of the resulting ink is fully
opaque — the remainder is normal anti-aliased edge. It is then palette-quantised
to 64 colours and embedded in `banner.svg` as a base64 `<image>`, so the SVG is
self-contained and renders identically anywhere.

This is why `banner.png` is 82 KB rather than the 31 KB it was with the vector
GLASSS mark: a raster logo with soft edges compresses far worse than paths.

---

## Open questions

- **⚠️ The banner's dates contradict the official poster.** The banner carries
  the deck's *24–27 settembre 2026*; the poster says the congress runs
  *30 settembre – 2 ottobre 2026*. One of the two is wrong. This was raised,
  and the deck's dates were chosen deliberately — but it is still unresolved,
  and the banner is public-facing.
- **Speaker name** — still nowhere.
- Only the horizontal `1600 × 300` format exists. A square or portrait cut for
  social/print would be a separate file.
- The CTA logo is a raster at 565 px wide, placed at 650 px — a 1.15× upscale.
  A vector version from CTA would remove that and shrink the PNG.
