# Dero Greens Website

Source files for the Dero Greens marketing site — pre-cooked, dried traditional Kenyan leafy vegetables (managu, terere, saga, and more), sold direct-to-consumer (B2C, diaspora shipping via DHL Express) and to distributors/importers (B2B, bulk & private label).

## Pages

- `index.dc.html` — Home
- `shop.dc.html` — Shop (B2C catalogue, cart)
- `distributors.dc.html` — Distributors (B2B, export info, quote request form)
- `recipes-usage.dc.html` — Recipes & Usage
- `about.dc.html` — About & Trust (story, certifications, contact)

## Stack

Built with Claude Design's `.dc.html` format — a lightweight component runtime (`support.js`) plus the "Classical" design system (`_ds/classical-*/styles.css`). `image-slot.js` powers the drag-and-drop photo placeholders.

**Photos:** every image on the site is currently a placeholder (`<image-slot>`). The drag-and-drop uploader only works live inside [claude.ai/design](https://claude.ai/design) — on a static host like GitHub Pages, adding real photos means either:
1. Continuing to edit in claude.ai/design and re-exporting here, or
2. Manually editing the HTML — replace an `<image-slot>`'s `src="..."` attribute with a real image URL, or swap the tag for a plain `<img>`.

## Outstanding content (flagged in the source, not yet final)

- Exact legal footer wording for Kito Kubuni / Dero Greens
- A personal "cooking for the diaspora" note for the homepage
- Usage ideas & photography for the 5 signature blends

## Local preview

These are static HTML files — open any `.dc.html` file directly in a browser, or serve the folder with any static file server, e.g.:

```bash
npx serve .
```
