# Intimacy Mastery Guide — Image Repository

**Last updated:** April 2026 (PDF v3 build)
**Total images:** 58 unique (img-000 through img-061, with 4 smask transparency layers excluded)
**Source PDF:** Intimacy Mastery Guide — Complete Edition v3 (56 pages)

## Two ways to find an image

This repo uses a dual-naming convention so that every image can be referenced in two ways:

### 1. Short canonical filenames (top of folder)

`img-000.jpg`, `img-001.jpg`, …, `img-061.jpg`

These are the **stable URLs** referenced by the Notion hub, all Phase Pages, the Visual Atlas, and Content Library rows. Format:

```
https://raw.githubusercontent.com/poarchteam-rgb/guide-images/main/intimacy-images/img-XXX.jpg
```

**Never rename these.** Doing so breaks every existing Notion embed.

### 2. Descriptive aliases (`descriptive_aliases/` subfolder)

The same 58 images, copied with descriptive names like:

- `img-027_cat-coital-alignment-technique.jpg`
- `img-054_eight-two-thrust-ratio-infographic.jpg`
- `img-060_face-sitting-north-facing-sexinfo101.jpg`

Use these when browsing GitHub directly to find an image by topic without consulting the manifest. The leading `img-XXX_` prefix preserves the link to the canonical short filename.

**Don't reference the descriptive aliases from Notion** — Notion uses the short names. The aliases are for human navigation only.

## Manifest

For a complete table mapping every short filename to its descriptive role, source attribution, and where it's used in the Notion hub, see `MANIFEST.csv` in this directory.

## Skipped numbers

`img-004`, `img-008`, `img-010`, `img-014` exist in the original PDF extraction as smask transparency-mask layers (auxiliary data, not actual images). They are intentionally skipped in this repo.

## Source attribution

Images come from a mix of educator/research illustrations and licensed-asset libraries used under educational fair use:

- **Cleveland Clinic** — anatomical diagrams (img-001)
- **Healthwise** — pelvic anatomy (img-056)
- **Kenneth Play / Beyond Satisfied** — research-informed illustrations (img-057, 058, 059)
- **OMGYes Essentials** — technique demonstrations
- **Caitlin V Neal** — manual technique guides
- **SexPositions Club**, **SexInfo101** — position references
- **Independent illustrators** — various

## Updating the repo

If a future PDF revision adds new images:

1. Extract new images via `pdfimages -all`
2. Compare with this manifest to identify net-new vs replacement vs renumbered
3. Append new images at the next free slot (e.g., `img-062`, `img-063`, …) to avoid breaking existing Notion embeds
4. Add their entries to `MANIFEST.csv` and create descriptive aliases in `descriptive_aliases/`
5. Update the Notion Visual Atlas to embed the new images
