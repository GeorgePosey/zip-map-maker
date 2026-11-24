# ZIP Code Map Maker

A single-page tool for making ZIP code choropleth maps of Los Angeles County
and Orange County. Give it a spreadsheet with a ZIP code column and it shades
each ZIP area by a count of rows or by a number in your file.

## What it does

- Reads CSV, TSV and text files, and GeoJSON files (including Census Reporter
  downloads). The file needs a ZIP code column or field.
- Shades each ZIP by how many rows fall in it, or by a number column, summed
  or averaged when a ZIP appears more than once.
- Shows values as the number itself, per 1,000 residents, or per square mile.
- Filters rows before mapping, and lists the records behind any ZIP you select.
- Lets you set the title, subtitle, legend, source note, number format, color
  palette, number of color steps, grouping method, basemap, theme and font.
- Covers LA and Orange County together, or either county alone.
- Exports the finished map as a PNG image or as a standalone HTML file.

## How to use it

Either:

- open the hosted page in a browser, or
- download `index.html` from this repository and open it locally. It is one
  self-contained file with no install and no build step.

Then drop in your file (or click "Try sample data"), pick the ZIP code column,
and adjust the labels, colors and layout in the side panel.

## Privacy

Files you load stay in your browser. Nothing is uploaded. The page only
contacts two outside services: `tiles.openfreemap.org` for the basemaps and
Google Fonts for the typeface.

## Saved maps

"Save map as file" downloads a standalone HTML copy of the tool with your data
and style inside it. Open that file to see the map again, keep editing, and
save again any time. By default a saved map holds per-ZIP totals only; you can
choose to include the row-level records as well.

## License

Released under the MIT License, Copyright (c) 2026 Alex Banh. See
[LICENSE](LICENSE).

Bundled third-party software (Papa Parse, MapLibre GL JS) and the data and
basemap sources keep their own licenses. See
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

Built with AI assistance.
