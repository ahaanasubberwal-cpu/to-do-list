# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Running the app

No build step. Open `index.html` directly in a browser:

```bash
open index.html
```

## Architecture

The entire app lives in a single file: `index.html`. It contains inline `<style>` and `<script>` — no external dependencies, no bundler, no framework.

**State** is a plain array (`tasks[]`) held in memory and persisted to `localStorage` keyed by date (`dayplan_YYYY-MM-DD`). Every mutation calls `save()` then `render()` for a full re-render.

**Sections** — Morning / Afternoon / Evening / Night — are defined in the `SECS` constant. When a task has a time value, `secFromTime()` auto-assigns it to the matching section.

**Drag and drop** uses the HTML5 Drag and Drop API. `dstart/dend/dover/dropTask/dropZone` handlers are re-attached after every `renderSections()` call because the DOM is fully rebuilt on each render.

**"Yesterday" duplication** reads `localStorage` for the previous day's key and clones those tasks with fresh IDs and `completed: false`.

## Deployment

Hosted via GitHub Pages. Pushing to `main` on `github.com/ahaanasubberwal-cpu/to-do-list` updates the live site at `https://ahaanasubberwal-cpu.github.io/to-do-list/`.
