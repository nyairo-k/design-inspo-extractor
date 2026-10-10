# Design inspo extractor

Runs [dembrandt](https://github.com/dembrandt/dembrandt) on GitHub's servers so nothing is installed locally.

1. Actions tab → "Extract design inspo" → "Run workflow".
2. Enter the site URL, the maximum number of pages to extract (pages are found through the site sitemap and merged into one result), and whether to also capture dark mode.
3. When the run finishes, open it and download the `inspo-<n>` artifact zip.

Inside the zip:
- `report-desktop.html`, `report-mobile.html` (and `report-dark.html` if chosen): open in a browser.
- `DESIGN.md`: tokens + prose, drop next to CLAUDE.md in a project to style against it.
- `output/<site>/<timestamp>.json`: raw data, including the full `motion` object.
