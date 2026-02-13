# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a learning journal - a developer's diary of going AI-first - hosted as a Jekyll site on GitHub Pages using the minima theme. The audience is Fullscript engineers - assume the reader works at Fullscript. Some entries reference internal tooling.

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

## Internal Tooling Context

The company (Fullscript) has a Homebrew cask (`fullscript/tools/fullscript-claude-code`) that automates Claude Code setup with AWS Bedrock. It handles AWS SSO auth via `rx`, creates per-user inference profiles (Opus 4.6, Sonnet 4.5, Haiku 4.5), and generates env/settings config. Install: `brew install --cask fullscript/tools/fullscript-claude-code`.

## Writing Style

- Use short dashes (-) instead of em dashes. Never use the long dash character.
- Tone is casual, honest, first-person. Not a tutorial - it's a personal journal.
- Keep entries concise and to the point. Trim filler and redundancy - readers should never feel like skipping paragraphs.
