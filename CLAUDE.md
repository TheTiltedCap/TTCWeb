# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

TTCWeb is the static marketing site for **The Tilted Cap** (thetiltedcap.com), hosted via **GitHub Pages** with a custom domain. It is a single-page static site — no build step, no framework, no bundler.

## Architecture

- `index.html` — the entire site: markup, inline CSS, and content. There is no JavaScript.
- `assets/` — images (logos, app store badges, screenshots) and video placeholders.

## Development

Open `index.html` in a browser. No build or serve command is needed. For live-reload during development, any static file server works (e.g., `python3 -m http.server` or the VS Code Live Server extension).

## Deployment

Pushing to `master` deploys automatically via GitHub Pages. There is no CI pipeline or build process.

## Style Notes

- Dark theme (`#0a0a0a` background) with Inter font from Google Fonts.
- All CSS is inlined in `<style>` within `index.html` — there are no external stylesheets.
- The `.gitignore` references Jekyll artifacts (`.sass-cache`, `_site`, `Gemfile.lock`) from a prior setup, but the site no longer uses Jekyll.
