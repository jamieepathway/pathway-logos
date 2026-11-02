# pathway-logos

Curated company brand logos for the Productive.io migration (company avatars).

Each `logos/<slug>.png` is a 256×256 PNG. These are referenced as company
`avatar_url`s via `raw.githubusercontent.com`, so this repo must stay **public**
(Productive fetches the URL unauthenticated, browser-side).

Sourced from each brand's own site (logo / apple-touch-icon) or Brandfetch,
human-reviewed. Logos are the trademarks of their respective owners; used here
only as account avatars in an internal tool.

## Figma mirror — keep in sync

Every logo here is also on the **Client logos** section of the Clients page in
Pathway Playground, which is where client logos are browsed:
https://www.figma.com/design/JxZ2ppypoR7Xg4sh14MbaQ/Pathway-Playground?node-id=737-2

One tile per `logos/<slug>.png`, named by slug, A–Z, 256×256, image fill set to
Fit. After adding or replacing a logo here, do all of these:

1. **Logo:** save it as `logos/<slug>.png`, 256×256, no transparency (pad onto
   white or the brand colour). Commit and push to `main`.
2. **Productive:** set the company's `avatar_url` to
   `https://raw.githubusercontent.com/jamieepathway/pathway-logos/main/logos/<slug>.png`.
3. **Figma:** in the Client logos section, duplicate any tile in the "Logo grid"
   frame, rename the tile and its rectangle to the slug, update the label, and
   drop the PNG onto the rectangle as an image fill (Fit). Move it into A–Z order.
   For a replaced logo, swap the image fill on the existing tile.

Claude can do all three from this README: "add <brand>'s logo to pathway-logos".
