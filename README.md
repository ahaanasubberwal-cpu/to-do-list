# DayPlan — Daily Itinerary Planner

A clean, accessible web app for planning your daily schedule as an interactive to-do list. Built with pure HTML, CSS, and JavaScript — no frameworks or dependencies.

![Screenshot](screenshot.png)

## Live Demo

[https://ahaanasubberwal-cpu.github.io/to-do-list/](https://ahaanasubberwal-cpu.github.io/to-do-list/)

## Features

- **Add tasks** with a title, time, category, location, and notes
- **Four time sections** — Morning (5am–12pm), Afternoon (12pm–5pm), Evening (5pm–9pm), Night (9pm–5am)
- **Auto-section assignment** — setting a time automatically places the task in the right section
- **Drag and drop** to reorder tasks or move them between sections
- **Mark complete** — check off tasks with a satisfying animation
- **Mark as important** — star tasks to highlight them as priority
- **Color-coded categories** — Work, Personal, Food, Travel, Shopping
- **Timeline sidebar** — see your full day ordered chronologically at a glance
- **Progress bar** — tracks how much of the day is done
- **Day summary** — total, completed, and upcoming task counts
- **Duplicate yesterday's plan** — copy the previous day's tasks in one click
- **Collapsible sections** — hide/show time blocks to focus on what matters
- **Local storage persistence** — data survives page refreshes, keyed per day
- **Fully accessible** — WCAG 2.2 AA compliant, keyboard navigable, screen reader friendly
- **Smooth animations** — spring-based transitions, card stagger, and reduced-motion support
- **Mobile responsive** — switches between list and timeline views on small screens

## Usage

No installation or build step needed. Open `index.html` directly in any browser:

```bash
open index.html
```

## Tech Stack

| Layer | Details |
|-------|---------|
| Markup | Semantic HTML5 with ARIA landmarks and roles |
| Styles | Vanilla CSS — custom properties, grid, transitions |
| Logic | Vanilla JavaScript — no frameworks or libraries |
| Storage | `localStorage` keyed by date (`dayplan_YYYY-MM-DD`) |
| Hosting | GitHub Pages |
