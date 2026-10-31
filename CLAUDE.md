# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

- The whole app is a single static `index.html` (inline CSS and JS). There is no build step, package manager, tests or linter. Open the file in a browser to try changes.
- It is served as a static site at <https://defrag.lol> (see `CNAME`). Keep the OG/Twitter meta tags in `index.html` on absolute `https://defrag.lol/...` URLs, because link scrapers don't resolve relative ones.
- `og-image.png` (1200×630) is the top 2276×1192 region of `screenshot.png`, resized. If the UI changes noticeably, update `screenshot.png` and regenerate `og-image.png` the same way. Crop with PIL: `sips -c` ignores the offset and crops from the center.
