# Design System: Trackd
**Project ID:** 10402838907271955027

## 1. Visual Theme & Atmosphere

Trackd is **Dark, Focused, and Motivating** — a midnight productivity canvas that keeps the user laser-locked on their daily habits. The aesthetic is built on deep, near-black surfaces layered with subtle violet luminance, creating a sense of calm depth without distraction. Glassmorphism card surfaces add a whisper of dimension, making content feel elevated above the background without breaking the minimalist discipline of the design.

## 2. Color Palette & Roles

| Descriptive Name | Hex | Functional Role |
|---|---|---|
| Midnight Charcoal | `#0f0f13` | Page background — the deepest layer |
| Obsidian Surface | `#1a1a24` | Card/container surface — primary layer |
| Graphite Border | `#2a2a38` | Dividers, card outlines, subtle separators |
| Electric Violet | `#7c3aed` | Primary accent — FAB, checked checkboxes, focus rings, active states |
| Violet Glow | `rgba(124,58,237,0.35)` | Ambient shadow glow on violet elements |
| Soft Lavender | `#a78bfa` | Secondary accent — labels, "Today" pill text, count highlights |
| Off-White Frost | `#f4f4f5` | Primary text — high-contrast headings and task labels |
| Muted Pewter | `#a1a1aa` | Secondary text — date sub-labels, placeholder copy |
| Zinc Shadow | `#52525b` | Completed task text — muted strikethrough state |
| Crimson Whisper | `#f43f5e` | Danger / delete — surfaces on hover of destroy actions |

## 3. Typography Rules

- **Font Family:** Inter (Google Fonts) — a geometric sans-serif that is clean without feeling cold
- **App Name / Hero Headings:** Bold weight (700), tight letter-spacing (`-0.04em`), off-white `#f4f4f5`
- **Date Headline:** Semi-bold (600-700), large, muted pewter `#a1a1aa` for the month/day sub-label, off-white for the weekday
- **Task Labels:** Medium weight (500), 15–16px, off-white in default state; transitions to Zinc `#52525b` with line-through on completion
- **Helper / Footer Text:** Regular (400), 12–13px, Zinc `#52525b` — deliberately quiet to avoid competing with task content
- **Labels & Badges:** All-caps, tight letter-spacing (`0.08em`), small (11–12px), Soft Lavender on a translucent violet pill

## 4. Component Stylings

- **FAB (Floating Action Button):** Full circle, 56–58px, solid Electric Violet `#7c3aed` fill, dramatic violet glow drop-shadow. Rotates icon from `+` → `✕` on activation. Scale bounces on hover (+8%) and tap (-5%) for haptic feel.
- **Checkboxes:** 22px rounded square (6px radius), default empty with Graphite Border; on check, fills Electric Violet with white checkmark and a violet ambient glow — the signature interactive moment of the app.
- **Task Cards / Containers:** Background Obsidian Surface `#1a1a24`, 1px Graphite Border, 12–16px generously rounded corners, whisper-soft diffused shadow (`0 4px 24px rgba(0,0,0,0.4)`). Hover state lightens to `#20202e`.
- **Date Banner:** Same card surface, bottom border divider, with the `Today` pill: Soft Lavender text on a translucent violet background with a 1px violet border — pill-shaped (`border-radius: 100px`).
- **Add Task Input:** Rounded (8–10px), dark semi-transparent background (`rgba(255,255,255,0.05)`), Graphite Border strokes at rest; Electric Violet border + glow ring on focus. Placeholder in Zinc `#52525b`.
- **Confirm Button:** Viola-filled rounded square (12px), white checkmark icon, violet ambient shadow. Matches FAB energy at smaller scale.
- **Delete Button (✕):** Ghost/transparent at rest; only revealed on row hover. On hover: icon turns Crimson Whisper `#f43f5e`, background becomes a soft red tint (`rgba(244,63,94,0.12)`). Keeps the UI uncluttered.

## 5. Layout Principles

- **Mobile-first, centered desktop:** Max content width of 540px, horizontally centered. Generous horizontal padding (16–20px inside cards, 16px outside).
- **Generous vertical breathing room:** Header gets 48px top padding; section headers and rows have 13–20px vertical padding — whitespace is treated as a premium design element.
- **Sticky FAB:** Fixed bottom-right with 32px insets on desktop, 24px on mobile — always in reach without obscuring content.
- **Single-column list:** No grid complexity — habit tracking is sequential, and the UI reflects that with a clean vertical rhythm.
- **Subtle radial ambient glow:** A violet radial gradient bleeds from the top-center and bottom-right of the `<body>` to suggest depth and give the background a living, atmospheric quality.
