# Carroll–Weyl Atlas

A static research website collecting arXiv hep-th papers on Carroll–Weyl gauged null strings.

Published website: https://sarthakduary.github.io/carroll-weyl-atlas/

## Features

- Search titles, authors, arXiv IDs, topics, and editorial summaries.
- Filter by topic and year.
- Sort by original submission date or title.
- Open the arXiv abstract and PDF, copy citations, or download filtered BibTeX.
- Download the complete JSON dataset.

## Publication

This site has no build step or external runtime dependencies. In GitHub Settings → Pages, select **Deploy from a branch**, branch **main**, folder **/ (root)**. The `.nojekyll` file disables Jekyll processing.

For a local preview, serve the folder over HTTP, for example with `python -m http.server 8000`, then open http://localhost:8000. Opening the HTML as a local file may prevent the dataset from loading.

## Updating the collection

Edit `papers.json`. Each record uses `id`, `title`, `authors` (an array), `date` (original submission date, YYYY-MM-DD), `category`, `kind` (`core`), `topics` (an array), and `summary`. Optional source URLs document verification. Set the top-level `updated` date after review.

Keep one entry per arXiv paper, include hep-th papers only, and distinguish each paper's claims from consensus. The featured origins paper is also included in the collection and counted only once. See SOURCES.md for selection and source notes.

## Credits

An independent bibliography, not affiliated with arXiv or INSPIRE. Paper titles, authors, and identifiers link to the original records. Summaries are editorial descriptions. The SVG worldsheet artwork is conceptual, not a physical solution or data plot.
