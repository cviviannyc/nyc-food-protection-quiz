# NYC Food Protection Course — Practice Quiz

An interactive study tool for the New York City Department of Health & Mental Hygiene (DOHMH) Food Protection Course exam. Built as a single-page web app with no dependencies.

**🔗 Live demo:** [cviviannyc.github.io/nyc-food-protection-quiz](https://cviviannyc.github.io/nyc-food-protection-quiz/)

---

## About

I'm building this while preparing for the NYC Food Protection Certification, which is required for operators of food service establishments — including the micro market and vending operations I run through [Lumi Vending](https://lumivending.com), my Queens-based vending placement company.

The official DOHMH course material is comprehensive but reads like a textbook, with no built-in way to test yourself before sitting the exam. So I'm building one — and turning a real business need into a portfolio project that grows alongside my study progress.

**Current status:** Lessons 1–7 complete with 75 questions. Lessons 8–15 in progress.

## Features

- **Practice questions** spanning the full DOHMH course (lessons 1–7 live now, 8–15 coming as I complete them)
- **Topic filtering** — drill down on a specific lesson (e.g. just bacteria, just storage temperatures) or shuffle from the full bank
- **Three quiz lengths** — quick (10 questions), medium (25), or full set
- **Instant feedback** with the correct answer and a one-line explanation after every question
- **Progress tracking** with running score and a progress bar
- **Answer review screen** at the end, showing every question you got wrong with the correct answer and explanation
- **Mobile-friendly** — works as a Progressive Web App when added to a phone home screen
- **Fully offline-capable** — single HTML file, no backend, no API calls

## Topics covered

### ✅ Live now (Lessons 1–7)

| Lesson | Focus |
|--------|-------|
| 1 | NYC Health Code, letter grading, inspections, Administrative Tribunal |
| 2 | Receiving food, temperature danger zone, thermometer calibration |
| 3 | Storage rules — FIFO, refrigeration, freezer, dry storage |
| 4 | Physical, chemical, and biological hazards; the Big 8 allergens |
| 5 | Bacteria — FATTOM conditions, growth rates, destruction methods |
| 6 | Viruses, parasites, yeasts, molds |
| 7 | Foodborne illnesses — Salmonella, E. coli, Botulism, Listeria, Norovirus, and more |

### 🚧 In progress (Lessons 8–15)

| Lesson | Focus |
|--------|-------|
| 8 | Preparing Food |
| 9 | Personal Hygiene |
| 10 | Food Establishment Design |
| 11 | Plumbing |
| 12 | Pest Control |
| 13 | HACCP: A Food Protection System |
| 14 | Required DOH Postings |
| 15 | Local Laws |

## Tech stack

- **HTML5** — semantic single-file structure
- **CSS3** — custom design system, no framework, mobile-first responsive layout
- **Vanilla JavaScript** — no React, no jQuery, no build step, no dependencies
- **GitHub Pages** for hosting

The entire app is one ~30 KB HTML file. It loads instantly, works offline once cached, and has zero third-party dependencies — which means no security risk, no version drift, and nothing to maintain.

## Design decisions

- **No frameworks.** This project didn't need React. Adding a build pipeline for a study quiz would be over-engineering. Choosing the simplest tool that fits the job is itself a skill.
- **No backend.** Quiz state lives in memory. No database, no auth, no server costs. The trade-off is no leaderboards or saved progress between sessions — acceptable for the use case.
- **Brand-aligned color palette.** Navy `#183F72` and amber `#D18137` — the same colors I use across Lumi Vending's marketing materials, for visual consistency.
- **Sentence-case throughout.** No ALL CAPS, no Title Case — keeps the tone calm and readable, especially helpful for a study tool where users are already nervous about an exam.

## Running locally

```bash
# Clone the repo
git clone https://github.com/cviviannyc/nyc-food-protection-quiz.git
cd nyc-food-protection-quiz

# Open the file directly in any browser
open index.html
```

That's it. No `npm install`, no build step.

## Roadmap

**Next up — content expansion:**
- [ ] Add questions for Lesson 8 (Preparing Food)
- [ ] Add questions for Lesson 9 (Personal Hygiene)
- [ ] Add questions for Lessons 10–12 (Establishment Design, Plumbing, Pest Control)
- [ ] Add questions for Lesson 13 (HACCP)
- [ ] Add questions for Lessons 14–15 (DOH Postings, Local Laws)

**After all 15 lessons are covered:**
- [ ] Persist quiz history with `localStorage` so users can track progress across sessions
- [ ] Add a "missed questions" mode that re-quizzes only the ones you got wrong
- [ ] Add a Spanish-language version (NYC has a large Spanish-speaking food service workforce)
- [ ] Convert to a full Progressive Web App with a service worker for true offline use

## Disclaimer

This is a study tool I'm building for personal exam prep and learning. It is **not** an official NYC DOHMH product, and passing this practice quiz does not certify anyone for anything. The official course is at [nyc.gov/health](https://www.nyc.gov/site/doh/business/food-operators/food-protection-course.page).

## License

MIT — feel free to fork it, adapt it, or use it as a template for your own study app.

---

Built by [Vivian](https://github.com/cviviannyc) · 2026
