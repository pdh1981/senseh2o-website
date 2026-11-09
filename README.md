# SenseH2O website

The public website for SenseH2O, a NERC-funded project to transform real-time water quality monitoring, led by the University of Stirling with the University of Glasgow.

It is a single static page (`index.html`) with no build step, published with GitHub Pages.

## Editing

- **Text:** edit `index.html` directly on GitHub (pencil icon) and commit. The live site updates within a minute or two.
- **Project log:** in the "Progress updates" section, copy one `<article class="update">` block, paste it at the top of the list, and change the date, tag, title and text. The page shows the newest three entries and hides the rest behind a "Show more" button automatically.
- **Images:** add files to `images/` and reference them as `images/your-file.jpg`. Keep photos to about 1400 px wide.
- **Settings:** the dashboard link and the SensorThings API address are at the top of the `<script>` block near the end of `index.html`.
- Text highlighted in yellow on the page (`class="ph"`) is placeholder content still to be filled in.

## Live data

The "Latest data from our sensors" section tries to load observations from the SensorThings API in the visitor's browser. That works only if the FROST-Server allows anonymous read access and CORS for the site's domain. Until then the page shows clearly labelled example data.

## Brand

- Logos: `images/logo-senseh2o-colour.svg` (header) and `images/logo-senseh2o-tagline-colour.svg` (footer), the full-colour "classic" three-node logo.
- Favicons: `favicon.svg`, `favicon.ico`, `apple-touch-icon.png`.
- Colours: greens #006938, #76b72a, #9fcc69; teals #008996, #005e63. Typeface: Inter.

## Custom domain

When `senseh2o.ac.uk` is registered, point DNS at GitHub Pages:

- `www` CNAME to `pdh1981.github.io`
- apex A records: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

Then set the custom domain under Settings > Pages and tick "Enforce HTTPS".
