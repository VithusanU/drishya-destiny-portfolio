# Images

Drop the photos in this folder using **exactly** these filenames. The site picks them up
automatically — no code changes needed. Any file that's missing falls back to a dashed
placeholder showing its filename, so the page never looks broken.

**Status:** all installed except `drishya-headshot` — the hero still shows the "D"
placeholder until a portrait is added. Use the best-quality original available (ideally
straight off her phone, not a re-compressed social download); it's the first thing
anyone sees on the page.

| Filename | Where it appears | Best shape | Suggested photo |
|---|---|---|---|
| `drishya-headshot.jpg` | Hero, top of page | **Portrait 3:4** | The strongest headshot — this is the first thing anyone sees |
| `fessenden-trott-buddle.jpg` | Fessenden-Trott award card | **Landscape 3:2** | The Trent feature photo with Dr. Melanie Buddle |
| `soroptimist-award.jpg` | Soroptimist card, left of three | **Portrait 3:4** | Solo shot with the roses in front of the Soroptimist banner |
| `soroptimist-presentation.jpg` | Soroptimist card, middle of three | **Portrait 3:4** | The two-person photo at the presentation |
| `soroptimist-group.jpg` | Soroptimist card, right of three | **Portrait 3:4** | The group of four with the banner |
| `scars-and-curves.jpg` | Scars & Curves feature block | **Square 1:1** | The brand mark — line art woman with flowers and butterfly on blush |

## Notes

- **Format**: `.jpg` or `.png` — the page tries both, so either extension works with the
  names above. Use `.png` for the Scars & Curves logo to keep the line art crisp.
- **The Scars & Curves slot** uses `object-fit: contain` on a blush field (`#F7EBE5`), so
  the logo is never cropped and its background blends into the card. Every other slot
  uses `cover` and crops from the edges.
- **The three Soroptimist photos** sit side by side in one full-width card at portrait
  3:4 — that shape was chosen because all three originals are portrait, and cropping them
  square cut people out of the group shot. On phones the three become a horizontal
  swipe strip rather than shrinking to unreadable thumbnails.
- **Size**: aim for ~1600px on the long edge and under ~500KB each. These load on every
  page view, and GitHub Pages doesn't optimize them for you.
- **Cropping**: images are `object-fit: cover`, so they fill their slot and crop from the
  edges. Keep faces near the centre. The shapes above are what each slot expects — a photo
  cropped to roughly the right ratio will look best.
- **Clicking** any photo opens it full-size in a lightbox. The caption comes from the
  `data-caption` attribute on that `<img>` in `index.html`.

## Permissions

The Trent feature photo (`fessenden-trott-buddle.jpg`) was taken by Trent University for
their news story. Confirm it's okay to reuse on a personal site before publishing —
otherwise swap in one of her own photos from the same event.
