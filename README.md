# ⚡ Life OS (Daily Tracker)

> A modern, zero-dependency personal dashboard and habit tracker engineered for speed, privacy, and full offline persistence.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Vanilla JS](https://img.shields.io/badge/Vanilla-JS%20%2F%20HTML5%20%2F%20CSS3-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-0-success.svg)](#)

---

## 🧭 Overview

**Life OS** is a self-contained productivity engine designed to eliminate friction in daily habit logging. Built entirely into a single zero-dependency file, it combines daily habit tracking, weighted performance scoring, gym logging with exercise breakdowns, structured task queues, and a local rule-based AI assistant.

All data remains strictly within your browser via `localStorage`, ensuring complete privacy, zero latency, and instant load times.

---

## ✨ Key Features

### 1. 📊 Holistic Daily Scoring & Streak Engine
- **Weighted Daily Score (0–100):** Calculates an aggregate daily rating combining wake time, bedtime, water, running, tasks, gym workouts, reading, self-work, and protein intake based on customizable user weights.
- **Dynamic Circular Ring:** Real-time SVG circular visual indicator displaying daily completion score.
- **Streak & Consistency Tracker:** Automatically tracks consecutive active days scoring 50+ points and records all-time best streaks.

### 2. 💧 Quick-Action Habit Logging
- **Water & Protein:** Rapid increment/decrement buttons (`+250ml`, `+500ml`, `+10g`, `+20g`, custom inputs) with complete entry undo and history logs.
- **Sleep & Circadian Rhythm:** Computes total sleep duration dynamically using logged bedtime and wake timestamps.
- **Deep Work Stopwatch:** One-tap start and stop timer session tracking for focused self-work, plus quick `+15 min` increments.
- **Meals Checklist:** Fast tracking for Breakfast, Lunch, Snacks, and Dinner.

### 3. 🏋️ Integrated Workout Planner & Logger
- **Split Routine Schedules:** Preloaded with weekly splits (*Chest + Triceps*, *Back + Biceps*, *Legs*, *Shoulders + Abs*, *Rest*).
- **Active Workout Mode:** Live logging interface for recording sets, weights (kg), reps, and completion per movement.
- **Volume & Muscle Split History:** Visualizes historical training frequency and workout logs.

### 4. 📈 Interactive Analytics & Heatmap
- **Configurable Ranges:** View trends and rolling totals across 7-day, 30-day, 90-day, and all-time windows.
- **Custom SVG Trendlines & Bar Graphs:** Zero-library visual metrics for water, sleep consistency, running mileage, gym frequency, protein intake, and reading volume.
- **GitHub-Style Contribution Heatmap:** Interactive 5-week grid allowing day-by-day retrospective inspection.

### 5. 🤖 Rule-Based Natural Language AI Center
- **Natural Language Parsing:** Input natural commands like *"Drink 3.5 litres of water daily"*, *"Run 5 km three times a week"*, or *"Add bench press every Monday"* to generate interactive proposals.
- **Review Inbox:** Staging queue that lets you approve, edit, or dismiss AI-generated routine changes before applying them.
- **Quick Queries:** Pre-built prompts for daily executive briefs, habit shortfall analysis, and weekly performance summaries.

### 6. 🎨 Mobile-First & Accessible Architecture
- **Responsive Layout:** Adaptive desktop sidebar navigation shifting seamlessly to an ergonomic mobile bottom navigation bar.
- **Theming:** Full native Dark (`#0B0F14`) and Light mode support with CSS variables.
- **Data Portability:** Instant JSON clipboard copy for backups, plus safe reset options and preloaded 30-day demo data.

---

## 🛠️ Built With

- **HTML5:** Semantic document structure with mobile safe-area viewport optimizations (`viewport-fit=cover`).
- **CSS3:** Custom properties (CSS variables), CSS Grid, Flexbox, smooth animations, and clean responsive typography.
- **Vanilla JavaScript (ES6+):** Client-side state machine, SVG visual generators, NLP parser, and event delegation.
- **Storage:** Browser `localStorage` (`lifeos-v1`).

---

## 🚀 Getting Started

Because Life OS is a pure client-side application, there are no bundlers, compilation steps, or npm packages required.

### Local Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yashpatil-1/Daily-Tracker.git
   ```

2. **Navigate into the folder:**
   ```bash
   cd Daily-Tracker
   ```

3. **Open the app:**
   - Double-click `index.html` to run directly in any modern browser (Chrome, Edge, Safari, Firefox), **OR**
   - Serve using VS Code with the **Live Server** extension.

### Deploying to GitHub Pages

1. Go to your repository on GitHub and open **Settings** > **Pages**.
2. Under **Build and deployment** > **Branch**, select `main` and root directory `/(root)`.
3. Click **Save**. Your tracker will be live at:
   ```text
   https://yashpatil-1.github.io/Daily-Tracker/
   ```

---

## 📁 Repository Structure

```text
Daily-Tracker/
├── index.html        # Monolithic single-file app (UI, styles, state logic, SVG charts)
└── README.md         # Project documentation
```

---

## ⚙️ State & Data Architecture

All app data resides in a single reactive JSON structure stored under the key `lifeos-v1`:

```javascript
{
  set: {
    name: "Yash",
    theme: "dark",
    waterGoal: 3000,
    protGoal: 100,
    runGoal: 5,
    readGoal: 5,
    w: { wake: 10, bed: 5, water: 15, run: 10, work: 15, gym: 15, read: 10, self: 10, prot: 10 },
    lab: { read: "Reading", self: "Self work" }
  },
  days: { /* "YYYY-MM-DD": { water, prot, run, read, meals, custom, wake, sb, gym, self } */ },
  tasks: [ /* { id, title, done, pri, due, cat, top } */ ],
  habits: [ /* { id, title } */ ],
  inbox: [ /* AI proposals */ ],
  sched: [ /* 7-day workout split */ ],
  hist: [ /* completed workouts */ ]
}
```

---

## 👤 Author

**Yash Patil**
- GitHub: [@yashpatil-1](https://github.com/yashpatil-1)

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).
