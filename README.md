# Trackd
Your daily focus, beautifully simple.

Trackd is a minimalist, native-web habit tracker that prioritizes beautiful aesthetics, speed, and absolute privacy. 
Built completely with Vanilla HTML, CSS, and JavaScript, it acts as a lightweight companion to keep your daily routines on point, storing everything right in your browser.

## Features

- 📅 **Daily Task View:** Clean, focused list of tasks for the day.
- 🕒 **Task Details & Durations:** Attach duration estimates and rich descriptions.
- 📊 **Activity Heatmap:** A GitHub-style contribution graph directly integrated into your dashboard helping you visualize and maintain a hot streak.
- ♻️ **Repeating Tasks:** Automatically re-generate routines on a Daily or Weekly cadence.
- ⏳ **Time Travel:** Need to fix an accidental checkmark from yesterday? The interactive heatmap and header arrows enable fluid travel backwards (or a day into the future) to manage your history.
- 🛡️ **Absolute Privacy:** 100% Client-side. No databases, no logins, no loading spinners. Your data is purely locally persisted.
- ✨ **Aesthetic First:** Deep Midnight Charcoal glassmorphism UI with smooth, premium micro-animations.

## Getting Started

1. Clone the repository.
2. Open `index.html` in any modern web browser. 
3. Start tracking!

## Architecture Details
Trackd was built to demonstrate how far you can push a unified single-file `index.html` application. State management runs completely off an in-memory `appState` dictionary synced to the browser's native `localStorage`. The DOM is dynamically re-painted via performant Vanilla JS functions bound to interaction listeners.

## License
MIT
