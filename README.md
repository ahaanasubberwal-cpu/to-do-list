# DayPlan — Daily Itinerary Planner

A minimal, dark-themed daily planning app. Organise your day into time blocks, track progress, and stay focused — no accounts, no sync, no distractions.

![Screenshot](screenshot.png)

## Live Demo

[https://ahaanasubberwal-cpu.github.io/to-do-list/](https://ahaanasubberwal-cpu.github.io/to-do-list/)

## Features

- **Four time sections** — Morning (5am–12pm), Afternoon (12pm–5pm), Evening (5pm–9pm), Night (9pm–5am)
- **Smart auto-placement** — setting a time automatically assigns the task to the right section
- **Drag and drop** — reorder tasks or move them between sections
- **Categories** — Work, Personal, Food, Travel, Shopping with colour-coded chips
- **Mark complete** — check off tasks as you go
- **Mark as important** — star any task to highlight it as priority
- **Timeline sidebar** — chronological view of your full day at a glance
- **Progress bar** — shows percentage of tasks completed
- **Day summary** — total, done, and remaining task counts
- **Collapsible sections** — hide/show time blocks to reduce noise
- **Duplicate yesterday** — copy the previous day's tasks in one click
- **Local storage** — data persists per day across refreshes, no server needed
- **Fully accessible** — WCAG 2.2 AA, keyboard navigable, screen reader friendly
- **Smooth animations** — spring-based transitions with reduced-motion support
- **Mobile responsive** — switches between list and timeline views on small screens

## Usage

No installation or build step. Open `index.html` directly in any browser:

```bash
open index.html
```

## Tech Stack

| Layer | Details |
|-------|---------|
| Markup | Semantic HTML5 with ARIA roles and landmarks |
| Styles | Vanilla CSS — custom properties, grid, dark theme |
| Logic | Vanilla JavaScript — no frameworks or dependencies |
| Storage | `localStorage` keyed by date (`dayplan_YYYY-MM-DD`) |
| Hosting | GitHub Pages |
