# Diwali Dhamaka 🪔

Celebrate Diwali digitally — no smoke, no noise complaints. Works on desktop (mouse) and phones (touch).
Open `index.html` in a browser (no build step).

- Pick a firecracker from the bottom row (swipe the row on small screens).
- It glides to the bottom centre and your cursor / finger becomes a sparkler.
- Touch the sparkler tip to the fuse: light and sound follow. 🔊 button top-left mutes.
- Top-right shows the live AQI for your location (Open-Meteo; falls back to Delhi).
  Each burst raises the AQI and blurs/hazes the starry sky.

## Add your own firecracker
Open `index.html` and edit the `CRACKERS` list (Section 1). Copy any entry and change:
`id`, `name`, `type` (`fountain`, `rocket`, `bomb`, `spinner`, `string`, `candle` or `custom`),
`pollution`, `opts`, and `art` (SVG lines in a 60×120 box with one `class="fuse-tip"` shape).
For a totally custom effect use `type: 'custom'` with a `run(api)` function — examples are in the comments.

## Hosting (GitHub Pages)
The site is a single static file (`index.html`), so any static host works.
1. Repo → Settings → Pages → *Build and deployment* → Source: **Deploy from a branch**.
2. Choose branch `main`, folder `/ (root)`, Save.
3. The site appears at `https://<username>.github.io/Diwali-Dhamaka/` after a minute.

Later, with your own domain: Settings → Pages → *Custom domain*, add a DNS record at your registrar
(CNAME to `<username>.github.io`, or A records to GitHub's Pages IPs), then tick *Enforce HTTPS*.
