# Reckless Reports

**by Rodrigo Sarain · Reckless Studios**

A system for converting any input — idea, transcript, brief, requirement, task — into a clean, executable HTML report. Built for creative strategy and software engineering.

→ **Live:** [reckless-reports.vercel.app](https://reckless-reports.vercel.app)  
→ **Framework documentation:** [reckless-reports.vercel.app/reports/analyze-framework](https://reckless-reports.vercel.app/reports/analyze-framework)

---

## What it does

Every report runs the input through 5 analysis lenses:

| Lens | Source | Question |
|------|--------|----------|
| Simple Stick | Ken Segall — *Insanely Simple* | Can this be reduced to one idea? |
| Ways of Seeing | John Berger | What does this actually communicate? |
| Free Play | Stephen Nachmanovitch | Where is the genuine impulse? |
| Jobs To Be Done | Christensen / Ulwick | What job is the audience hiring this to do? |
| Working Backwards | Amazon PR/FAQ | If this works perfectly, what does the press release say? |

Output: themed insights → JTBD statements → Simple Stick filter → PR/FAQ → sprint plan → Notion structure → shareable HTML report.

---

## Three modes

- **Content** — carousels, scripts, video campaigns, launches
- **Software** — requirements, epics, user stories, technical sprints
- **Launch** — new product/service/client that needs a go-to-market strategy

---

## How reports are generated

Reports are created via the `/analyze` Claude Code skill. Drop any input into a Claude Code session and the system runs the full analysis, writes the HTML to this repo, and the result is live on Vercel automatically after `git push`.

---

## Design system

- **Font:** Inter — Bold (700) headings · Semibold (600) body · Medium (500) highlights
- **Colors:** Signal `#D95200` · Void `#1A1A1A` · Paper `#F5F3EE` · Stone `#7A7872`
- **UI:** MacBook-style window chrome + dot-grid whiteboard background
- **Shared styles:** `assets/style.css`

---

## Repo structure

```
reckless-reports/
├── index.html                    ← Reports dashboard
├── assets/
│   ├── style.css                 ← Shared design system
│   └── logo.png                  ← Reckless Studios logo
├── reports/
│   └── [report-slug]/
│       └── index.html            ← Each generated report
└── vercel.json
```

---

*Rodrigo Sarain · Reckless Studios — Córdoba, Argentina*
