# Mindful Tasks & Focus Space

A lightweight, single-file productivity application combining staged task tracking, a Pomodoro timer, ambient audio generators, and CSV data persistence. Built entirely with vanilla HTML5, CSS3, and JavaScript with zero external runtime dependencies.

---

## Features

### 1. Multi-View Architecture
Swipeable, full-screen carousel interface with four operational views:
* **Mindful Space:** Built-in 25-minute Pomodoro timer alongside ambient sound toggles (Storm and Birdsong).
* **Inbox:** Default repository for newly captured tasks.
* **Daily Focus:** Targeted workspace for prioritized daily objectives.
* **Completed Tasks:** Archive tracking harvested tasks with completion dates and data export/import capabilities.

### 2. Gamified Growth Tracking
Tasks follow a 5-stage lifecycle represented by growth indicators:
* `0%`: 🫘 (Seed)
* `25%`: 🌱 (Sprout)
* `50%`: 🌿 (Seedling)
* `75%`: 🪴 (Potted Plant)
* `100%`: 🌳 (Harvested / Completed)

Reaching 100% automatically stamps the completion date, triggers an audio cue, and moves the item to the Archive.

### 3. Ambient Audio & Timers
* Dual audio streams (`storm.mp3`, `birdsong.mp3`) with independent looping toggles.
* Integrated Pomodoro countdown timer with start, pause, resume, and reset functionality.
* Completion alert with dedicated audio ping.

### 4. Data Persistence & Portability
* Real-time sync to browser `localStorage`.
* **CSV Export:** Generates structured `garden_tasks.csv` containing task IDs, descriptions, completion states, and progress markers.
* **CSV Import:** Parses and validates external CSV task backups directly into application state.

---

## File Structure

The project runs out of a single root directory:

```text
.
├── index.html       # Combined application markup, CSS styling, and logic
├── storm.mp3        # Local ambient audio asset: Storm
└── birdsong.mp3     # Local ambient audio asset: Birdsong
