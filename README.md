# ☾ Dream Journal

> "A little place for the dreams you don't want to forget."

A single-page, dark-themed **Dream Journal** landing page and interactive prototype — a digital diary for capturing, organizing, and reflecting on your dreams. Built entirely as one self-contained `index.html` file: no build step, no backend, no dependencies beyond two Google Fonts.

## ✨ What it does

- **Live clock & greeting** — a real-time clock reads your browser's timezone (`Intl.DateTimeFormat`) and greets you differently depending on the hour ("Good morning ✦", "Late night thoughts ✦", etc.), updating every second.
- **Dream preview card** — a sample diary entry ("Midnight Hallway") styled like a page torn from a digital diary, with hover motion and a click-to-expand modal.
- **Six feature highlights** — Capture Dreams, Dream Archive, Mood & Tags, Dream Calendar, Dream Insights, Timezone Aware.
- **How it works** — a simple three-step story: Remember → Record → Reflect.
- **Timezone conversion tool** — pick from Bangkok, Tokyo, Singapore, London, Paris, New York, Los Angeles, or Sydney, and watch a recorded dream's time convert live, correctly handling DST via the IANA timezone database (no hard-coded offsets). A "Use my timezone" shortcut detects your browser's zone automatically.
- **Dream archive preview** — sample dream cards you can click to open a full detail modal (title, date/time, timezone, mood, tags).
- **"Start Journaling" flow** — a real, working form (title, date, time, timezone, mood) with inline validation and a success confirmation, saving entries to the browser's `localStorage` under the key `dreamJournalEntries`. Refresh the page and your dreams are still there.
- **Fully responsive & accessible** — mobile hamburger menu, keyboard-navigable modals (closable with `Esc`), visible focus states, semantic HTML, and full support for `prefers-reduced-motion`.

## 🎨 Design language

**Midnight Dream** — a deep navy-to-purple palette (`#0B0D24 → #24184A → #6D4AFF`), soft glassmorphism on cards and navigation, gradient buttons, and gentle glow accents. Typography pairs **DM Serif Display** (headlines, dream titles) with **Plus Jakarta Sans** (body, UI). No characters, people, or animals anywhere — only moons, stars, abstract gradients, and dream-diary motifs.

## 🚀 How to use it

Just open `index.html` in any modern browser — that's it. No installation, no server, no build tools required.

```
open index.html
```

## 🧱 Tech stack

- HTML5, CSS3, vanilla JavaScript (no frameworks)
- Inline SVG icons
- `Intl.DateTimeFormat` for all time, date, and timezone logic
- `localStorage` for demo persistence of journal entries

## ⚠️ Scope notes

This is a **front-end prototype / design concept**, not a production app:

- No real backend, database, authentication, or API — all data lives in the browser's `localStorage`.
- "Sign in" and a few footer links are placeholders for a future real product.
- Intended as a portfolio-quality UI/UX demo that could be extended into a real product later.
