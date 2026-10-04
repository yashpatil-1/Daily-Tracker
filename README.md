readme_content = """# ⚡ Life OS (Daily Tracker)

> A lightweight, zero-dependency personal dashboard and daily habit tracker engineered for speed, privacy, and full offline persistence.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Vanilla JS](https://img.shields.io/badge/Vanilla-JS%20%2F%20HTML5%20%2F%20CSS3-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-0-success.svg)](#)

---

## 🧭 Overview

**Life OS** is a self-contained productivity engine designed to eliminate friction in daily habit logging. Built entirely into a single zero-dependency file, it combines daily habit tracking, weighted performance scoring, gym logging with exercise breakdowns, structured task queues, and a local rule-based AI assistant.

All data remains strictly within your browser via `localStorage`, ensuring complete privacy, zero server costs, and instant load times.

---

## ✨ Key Features

### 1. 📊 Holistic Daily Scoring & Streak Engine
- **Weighted Daily Score (0–100):** Aggregates water, sleep consistency, fitness, reading, protein, deep work, and task completion based on customizable user weights.
- **Dynamic Visual Rings:** Real-time SVG circular indicators tracking daily progress against individual thresholds.
- **Streak Tracker:** Automatically calculates current streaks and personal records for days meeting target performance.

### 2. 💧 Quick-Action Habit Logging
- **Water & Nutrition:** Rapid-increment buttons (`+250ml`, `+500ml`, custom amounts) with protein and meal-by-meal checkboxes.
- **Sleep & Circadian Rhythm:** Computes total sleep duration dynamically using bedtime and wake timestamps.
- **Micro-Timer for Deep Work:** One-tap start and stop session tracker with incremental manual adjustments (`+15 min`).

### 3. 🏋️ Integrated Workout Planner & Logger
- **Split Routine Schedules:** Preloaded with weekly splits (*Chest + Triceps*, *Back + Biceps*, *Legs*, *Shoulders + Abs*, *Rest*).
- **Active Workout Mode:** Live logging interface for recording sets, weights (kg), reps, and completion per movement.
- **Volume & Muscle Split History:** Visualizes historical training frequency and workout logs.

### 4. 📈 Interactive Analytics & Heatmap
- **Configurable Ranges:** View progress curves and rolling totals across 7-day, 30-day, 90-day, and all-time windows.
- **Custom SVG Trendlines & Bar Graphs:** Clean data visualizations without external charting libraries.
- **GitHub-Style Contribution Heatmap:** Interactive 5-week grid allowing day-by-day retrospective inspection.

### 5. 🤖 Rule-Based Natural Language AI Center
- **Natural Language Parsing:** Input phrases like *"Drink 3.5 liters of water"* or *"Add bench press every Monday"* to generate interactive proposals.
- **Review Inbox:** Staging queue that lets you approve, edit, or reject AI-generated routine changes before applying them.
- **Quick Queries:** Pre-built prompts for daily executive briefs, habit shortfall analysis, and weekly performance summaries.

### 6. 🎨 Mobile-First & Accessible Architecture
- **Responsive Layout:** Adaptive desktop sidebar navigation shifting seamlessly to an ergonomic mobile bottom bar.
- **Theming:** Full native Dark and Light mode support.
- **Zero Config:** Instant data portability via one-click JSON clipboard export.

---

## 🛠️ Tech Stack

- **Markup & Layout:** Semantic HTML5, safe-area inset adaptation for mobile viewports
- **Styling:** Vanilla CSS3 with CSS custom properties (variables), CSS grid, and responsive flexbox
- **Logic & Charts:** Pure Vanilla JavaScript (ES6+), custom SVG data rendering, client-side state machine
- **Storage:** LocalStorage (`lifeos-v1`)

---

## 🚀 Getting Started

Because Life OS requires zero build steps, bundlers, or package managers, setup takes seconds.

### Method 1: Local Browser Execution

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yashpatil-1/Daily-Tracker.git](https://github.com/yashpatil-1/Daily-Tracker.git)
