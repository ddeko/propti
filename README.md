# Propti — Property Sales CRM + Gamification (Indonesia)

A responsive, **frontend-only MVP** for demoing to clients. No backend, no build step.
All data lives in the browser's `localStorage`, so it persists between visits and resets cleanly.

## Run it

- **Easiest:** double-click `index.html` (needs internet — Tailwind & React load from CDN).
- **Or serve the folder** (recommended):
  ```
  npx serve -l 3210 ./agentquest
  ```
  then open http://localhost:3210

## Design & localization
- **Identity:** deep navy (`#1d3856`) + warm amber accent on a warm-paper background, SVG line-icons, minimal gradients — a grounded proptech look.
- **Region:** Indonesia. Currency in **Rupiah** (`Rp`, with `jt` / `M` short forms), Indonesian sample names and Jakarta-area locations.
- **Language switch: EN / ID** in the top bar (and in Profile + the mobile "More" sheet). The whole UI re-renders instantly; the choice is saved. Default is **ID**.

## What's inside

**CRM** — Leads (search, stage filters, add/edit, detail drawer with per-lead history), drag-and-drop **Pipeline** Kanban, property **Listings**, and a day-grouped **Activity** feed.

**Gamification** — XP, levels & 5 tiers (Bronze→Diamond) with level-up celebration; daily/weekly/monthly **Quests** that progress from real CRM actions; **Leaderboard** with podium; auto-unlocking **Achievements/badges**; **Reward Store**, purchasable **Titles**, and a reward-point balance/history.

## Notes for the demo
- Logging activities and moving a lead to *Closed Won* earns XP/points and triggers toasts + confetti.
- **Profile → Reset demo data** restores the seeded sample data anytime.
- Built to swap onto a real API later — all state flows through one store (`actions` in `index.html`), and all copy goes through the `t()` i18n helper.
