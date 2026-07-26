# The Lia Chronicle — Corrected Edition

A noir newspaper flip-book for **Lia**: the stone that turned out to be warm.

Open `index.html` in a browser. No build step, no dependencies, one file.

## Drop the photos in

| File | Used on | Size |
| --- | --- | --- |
| `lia.png` | Page 1 — Exhibit A | 488 × 767 |
| `lia2.png` | Page 4 — Exhibit B | 480 × 762 (detail enlargement of Exhibit A) |

Both are in place. Replace either file and the page picks it up — any
portrait aspect works, since the plate letterboxes onto paper tone rather
than cropping a face. If a file goes missing, the drawn placeholders
(`exhibit-a-placeholder.svg`, `exhibit-b-placeholder.svg`) take over.

## Reading it

- Click / tap the left or right half of the paper, swipe, or use `←` `→`
- `Home` / `End` jump to the front and back page, `M` mutes the theme
- Tap the spider. She's carrying the delivery.

## How it stays scaled

Every page is composed in a fixed design-pixel space (`--pw` × `--ph`) and
then uniformly scaled to fit the real viewport, so a phone gets the exact
composition a desktop gets, just smaller — nothing reflows into a mess.
Three modes: `spread` (desktop), `phone` (tall, one page at a time),
`flat` (landscape phones and squat windows). If a page's copy ever
overruns its plate, JS shrinks that composition a notch, so no page can
clip on any device.

Presentation lineage: [aeris-archive](https://github.com/aecha547/aeris-archive)
and the Natasha edition. Original copy and assets here.

## Contents

1. Front page — the wanted notice
2. The Stone Report — cont'd
3. Case file LIA-01 — including the etymological annex
4. The Forensics Desk — Exhibit B and the laboratory finding
5. Corrigendum — the retraction
6. Court report — The People v. Lia
7. Editorial — off the record
8. Back page — clip & keep
