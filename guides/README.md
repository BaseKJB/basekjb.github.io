# ConveyLoop SEO pages

This folder is managed by [ConveyLoop](https://conveyloop.com). It holds the
SEO pages ConveyLoop publishes for this site, and ConveyLoop rewrites its
files whenever it publishes.

**Do not edit files here by hand** — a change made here is lost the next time
ConveyLoop writes that file. Change the page in ConveyLoop instead. To change
how the pages look, see the notes at the top of their stylesheet
(`content/conveyloop.css`, where there is one).

## What is here

- `content/` — the pages, one file per page, and the stylesheet they link to;
  when the pages are served under a path such as `/guides`, also `_index`,
  the section's own page at that path, listing them all
- `sitemap.xml` — the URLs of these pages, for search engines
- `conveyloop-manifest.json` — ConveyLoop's record of the files it wrote here;
  it removes pages you unpublish, and never deletes a file it did not write
- `README.md` — this file

## Getting the pages into search results

Search engines only read `sitemap.xml` if they know it exists. Add a line to
your site's `robots.txt` with its full URL, for example:

    Sitemap: https://www.example.com/path/to/this/folder/sitemap.xml
