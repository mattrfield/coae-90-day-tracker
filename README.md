# COAE Study Tracker

An interactive, offline-friendly study tracker for the **Hack The Box Certified Offensive AI Expert (HTB COAE)** certification.

It lays out the full curriculum of the [AI Red Teamer Job-Role Path](https://academy.hackthebox.com/path/preview/ai-red-teamer) — all 12 modules / 230 sections — and tracks your progress, notes, and pace as you go. Pick a **30-, 60-, or 90-day timeline** to match the time you have: the curriculum stays the same, just repackaged into a denser or gentler schedule. The whole thing is a single self-contained HTML file: no build step, no dependencies, no internet required.

![The COAE study tracker in its 30-, 60-, and 90-day timeline modes](screenshot.png)

## Features

- **Adjustable 30 / 60 / 90-day timeline** — choose how long you have, and the same full curriculum regroups into denser or lighter days. Day cards, weeks, the progress chart, the pace indicator, and the weekly-hours estimate (≈ 50 / 25 / 10–20 hrs per week) all adjust to match — and your checked-off progress carries over when you switch modes.
- **Day-by-day plan** — the full path from lab setup and AI/ML foundations through prompt injection, data attacks, adversarial evasion, AI privacy, and defense, ending with report-writing practice and a mock engagement.
- **Progress dashboard** — overall completion ring, days completed, best streak, current phase, a weekly progress chart, per-phase breakdown, and an ahead/behind **pace indicator** based on your start date.
- **Notes & journal** — a collapsible notes field on every day to log what you learned, payloads that worked, and things to revisit.
- **Resource library** — 40+ curated links: official HTB modules, frameworks (OWASP LLM Top 10, MITRE ATLAS, Google SAIF, NIST AI RMF), Python/ML foundations, offensive AI tooling (garak, ART, PyRIT), practice playgrounds, and key adversarial-ML papers.
- **Local persistence** — all progress saves automatically to your browser's `localStorage`. Export/Import buttons let you back up or move your progress.

## Getting started

1. Clone the repo:
   ```bash
   git clone https://github.com/mattrfield/coae-study-tracker.git
   ```
2. Open `coae-study-tracker.html` in any modern browser (double-click it, or `File > Open`).
3. Choose your **timeline** (30, 60, or 90 days) and set your **start date** at the top — every day's calendar date and your pace indicator are computed from them.
4. Tick tasks as you complete them. A day turns green when all its tasks are done.

No server, no install. It runs entirely in your browser.

> **Tip:** Progress is stored per-browser. Use the **Export backup** button regularly, and **Import** it if you switch browsers or machines. (Some browsers restrict `localStorage` on `file://` pages — if progress doesn't stick, exporting/importing is your reliable backup.)

## The plan at a glance

| Phase | Days (90-day) | Focus |
|-------|---------------|-------|
| 1 | 1–7 | Foundations & lab setup (Python, ML intuition, security primer) |
| 2 | 8–28 | AI/ML core — *Fundamentals of AI*, *Applications of AI in InfoSec* |
| 3 | 29–49 | LLM attacks — *Red Teaming AI*, *Prompt Injection*, *LLM Output Attacks* |
| 4 | 50–63 | Data & system attacks — *AI Data Attacks*, *Attacking AI: Application & System* |
| 5 | 64–80 | Adversarial evasion — *Foundations*, *First-Order*, *Sparsity Attacks* |
| 6 | 81–90 | *AI Privacy*, *AI Defense*, report practice, mock engagement, exam prep |

The day ranges above describe the default **90-day** layout. The 60-day and 30-day timelines pack the same curriculum — about **217 hours total** — into fewer days, so the weekly load rises: roughly **10–20 hrs/week** at 90 days, **~25 hrs/week** at 60 days, and **~50 hrs/week** at 30 days. All three assume a foundations-level start in both offensive security and AI/ML.

## About the certification

The HTB COAE is earned by completing the AI Red Teamer Job-Role Path and passing a **7-day practical exam** in which you assess an AI-driven infrastructure and submit a commercial-grade technical report. Always confirm current module counts, exam format, and pricing on the [official HTB Academy site](https://academy.hackthebox.com/preview/certifications/htb-certified-offensive-ai-expert).

## Contributing

Issues and pull requests are welcome — improvements to the curriculum, resources, or UI are all fair game. Since the tracker is a single HTML file, edits are straightforward: the curriculum lives in the `CURRICULUM` array and resources in the `RESOURCES` array inside the `<script>` block.

## Disclaimer

This is an independent, community study aid. It is **not affiliated with, endorsed by, or sponsored by Hack The Box**. "Hack The Box" and "HTB" are trademarks of their respective owner.

## License

[MIT](LICENSE) — free to use, modify, and share.
