# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a public learning journal - a developer's diary of going AI-first - hosted as a Jekyll site on GitHub Pages using the minima theme. The site lives at https://danialbetres.github.io/learning-ai-in-public.

## Site Structure

- `entries/` - Blog entries as markdown files, numbered sequentially: `entry-000.md`, `entry-001.md`, etc.
- `index.md` - GitHub Pages home page (Jekyll layout: default)
- `README.md` - GitHub repo landing page
- `_config.yml` - Jekyll configuration

## Adding a New Entry

1. Create `entries/entry-NNN.md` with Jekyll frontmatter (`layout: default`, `title`, `date`)
2. Follow the existing entry format: H1 title, **Date** and **TL;DR** lines, `---` separator, then content sections
3. End each entry with the standard footer: `[Back to Index](../)`
4. Add the entry to the table in **both** `index.md` (link without `.md` extension) and `README.md` (link with `.md` extension)

## Writing Style

- Use short dashes (-) instead of em dashes. Never use the long dash character.
- Tone is casual, honest, first-person. Not a tutorial - it's a personal journal.
- Keep entries concise and to the point. Trim filler and redundancy - readers should never feel like skipping paragraphs.
