# Digital Diwali

Celebrate Diwali digitally with no smoke, no noise complaints.
Open `index.html` in a browser (no build step).

- Try the **Pyro Stick**: light it, then hold the mouse button (or drag a finger) to write or draw in the air. It burns for 6 seconds.
- Pick a firecracker from the bottom row (swipe the row on small screens).
- It glides to the bottom centre and your cursor / finger becomes a sparkler.
- Touch the sparkler tip to the fuse: light and sound follow. 🔊 button top-left mutes.
- Top-right shows the live AQI for your location (Open-Meteo; falls back to Delhi).
  Each burst raises the AQI and blurs/hazes the starry sky.

**Live:** https://dhruvb-cloud.github.io/Digital-Diwali/

- Below the Noise meter there are share buttons for X, LinkedIn and Instagram.
  (Instagram has no web share link, so phones open the share sheet and computers copy the text and link.)

## SEO files
- `index.html` head: title, description, canonical link, Open Graph / Twitter cards, JSON-LD.
- `og-image.png`: the 1200×630 preview picture shown when the link is shared.
- `robots.txt` and `sitemap.xml`: for search engines. When you move to your own domain, change the
  address in these two files, in `SHARE_URL` (in the script) and in the canonical/Open Graph tags in `index.html`.

## Add your own firecracker
Open `index.html` and edit the `CRACKERS` list (Section 1). Copy any entry and change:
`id`, `name`, `type` (`fountain`, `rocket`, `bomb`, `spinner`, `string`, `candle` or `custom`),
`pollution`, `opts`, and `art` (SVG lines in a 60×120 box with one `class="fuse-tip"` shape).
For a totally custom effect use `type: 'custom'` with a `run(api)` function — examples are in the comments.
