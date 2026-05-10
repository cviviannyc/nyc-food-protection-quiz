# Foodsafe.nyc — NYC Food Protection Course Study Companion

An interactive study tool for the New York City Department of Health & Mental Hygiene (DOHMH) Food Protection Course exam. Two modes — a multiple-choice practice quiz and a flashcard deck — covering all 15 lessons of the official curriculum plus the official 5-day study guide.

**🔗 Live demo:** [cviviannyc.github.io/nyc-food-protection-quiz](https://cviviannyc.github.io/nyc-food-protection-quiz/)

---

## About

I built this while preparing for the NYC Food Protection Certification, which is required for operators of food service establishments — including the micro market and vending operations I run through [Lumi Vending](https://lumivending.com), my Queens-based vending placement company.

The official DOHMH course material is comprehensive but reads like a textbook, with no built-in way to test yourself before sitting the exam. So I built one — and turned a real business need into a portfolio project.

## Features

### Two complementary study modes

- **Practice quiz** — multiple-choice questions with instant feedback, topic filtering, three length options, and an end-of-session review screen showing every question you missed.
- **Flashcards** — click-to-flip cards organized by category. Drill the temperatures, pathogen profiles, and core definitions that show up over and over on the exam. Keyboard shortcuts (← →, space) for fast review.

### Full course coverage

All 15 lessons of the NYC DOHMH Food Protection Course, plus the official 5-day DOH study guide:

| Lesson | Focus |
|--------|-------|
| 1 | NYC Health Code, letter grading, inspections, Administrative Tribunal |
| 2 | Receiving food, temperature danger zone, thermometer calibration |
| 3 | Storage rules — FIFO, refrigeration, freezer, dry storage |
| 4 | Physical, chemical, and biological hazards; the Big 8 allergens |
| 5 | Bacteria — FATTOM, growth phases, destruction methods |
| 6 | Viruses, parasites, yeasts, molds |
| 7 | Foodborne illnesses — Salmonella, E. coli, Botulism, Listeria, Norovirus, etc. |
| 8 | Preparing food — thawing, cooking temps, cooling, reheating |
| 9 | Personal hygiene — handwashing, dress code, sick worker rules |
| 10 | Food establishment design, dishwashing, sanitization |
| 11 | Plumbing — air breaks, AVBs, grease interceptors |
| 12 | Pest control — flies, roaches, rodents, IPM strategy |
| 13 | HACCP — the 7 principles, critical control points |
| 14 | Required DOH postings — choking, hand wash, alcohol/pregnancy |
| 15 | Local laws — Smoke-Free Air Act, tobacco regulations, CPR equipment |
| ★ | Official DOH 5-day Study Guide |

### Numbers

- **~145 quiz questions** with explanations
- **~130 flashcards** across three categories (temperatures & numbers, pathogens, definitions)
- **3-page web app** — landing, quiz, flashcards
- **0 dependencies** — pure HTML, CSS, vanilla JS
- **0 cost** — free forever, no signup

## Tech stack

- **HTML5** — semantic, multi-page structure
- **CSS3** — custom design system with CSS variables, no framework
- **Vanilla JavaScript** — no React, no jQuery, no build step
- **Google Fonts** — Fraunces (serif) + Inter (sans) for editorial typography
- **GitHub Pages** for hosting

The entire app is three small HTML files. Each loads instantly, works offline once cached, and has zero third-party JS dependencies.

## Design

The interface uses an editorial SaaS aesthetic — generous whitespace, large serif headlines, soft warm-cream backgrounds, hairline borders, and minimal flat surfaces. The color palette is built around Lumi Vending's brand:

- **Navy** `#183F72` — primary actions, accents, hero typography
- **Amber** `#D18137` — secondary accents, highlights, the "active" feel
- **Cream** `#FAF8F3` — background; warmer than pure white, less harsh for long study sessions
- **Fraunces** (serif) for headlines, italic emphasis, card content
- **Inter** (sans) for UI, body, labels

## Design decisions

- **No frameworks.** This project didn't need React. Adding a build pipeline for a study app would be over-engineering. Choosing the simplest tool that fits the job is itself a skill.
- **No backend.** Quiz state lives in memory. No database, no auth, no server costs. The trade-off is no leaderboards or saved progress between sessions — acceptable for the use case.
- **Multi-page over SPA.** A landing page sets the tone, then routes to focused tools. Each page is independent — easier to maintain, faster to load, simpler to debug.
- **Editorial typography.** A serif headline font (Fraunces) paired with a clean sans (Inter) creates the calm, trustworthy feel of a publication rather than the busy feel of a typical study app. Helps with long sessions.
- **Sentence case throughout.** No ALL CAPS, no Title Case. Keeps the tone calm — important for a tool used by people preparing for an exam.

## Running locally

```bash
# Clone the repo
git clone https://github.com/cviviannyc/nyc-food-protection-quiz.git
cd nyc-food-protection-quiz

# Open in any browser
open index.html
```

That's it. No `npm install`, no build step, no config.

## File structure

```
nyc-food-protection-quiz/
├── index.html         # Landing page — project intro, feature overview, topic table
├── quiz.html          # Multiple-choice practice quiz
├── flashcards.html    # Click-to-flip flashcard deck
├── README.md          # This file
└── LICENSE            # MIT
```

Each HTML file is fully self-contained — styles and scripts inline. You could host any one of them independently.

## Roadmap

**Future improvements:**

- [ ] Persist quiz history with `localStorage` so users can track progress across sessions
- [ ] Add a "missed questions only" mode that re-quizzes the cards you got wrong
- [ ] Spanish-language version (NYC has a large Spanish-speaking food service workforce)
- [ ] Convert to a Progressive Web App with a service worker for true offline use
- [ ] Optional dark mode
- [ ] Custom question packs (focus on a specific subset based on your weakest areas)

## Disclaimer

This is a study tool I built for personal exam prep and learning. It is **not** an official NYC DOHMH product, and using it does not certify anyone. The official course is at [nyc.gov/health](https://www.nyc.gov/site/doh/business/food-operators/food-protection-course.page).

## License

MIT — feel free to fork it, adapt it, or use it as a template for your own study app.

---

Built by [Vivian](https://github.com/cviviannyc) · 2026
