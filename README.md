# Upcomers email assets

Static assets for Ecomail campaigns, served via jsDelivr:
`https://cdn.jsdelivr.net/gh/MatyasHolata/upcomers-email-assets@main/<path>`

## Newsletter header (dark-mode proof)

Header is a single baked PNG (aurora + logo + meta + H1) so Gmail/iOS dark mode
cannot recolor it. Per issue:

1. Export new header from Figma: **1280 x 376 px PNG** (displays at 640 x 188, retina 2x).
2. Drop it into `nl/` (e.g. `header-002.png`), commit, push.
3. In Ecomail, copy template "Newsletter — MASTER", point the header `<img src>` at the new file.
4. If jsDelivr serves a stale file, purge:
   `https://purge.jsdelivr.net/gh/MatyasHolata/upcomers-email-assets@main/nl/header-002.png`

`nl/px-121212.png` = 1x1 dark pixel locking the footer background against Gmail dark-mode inversion. Do not delete.
