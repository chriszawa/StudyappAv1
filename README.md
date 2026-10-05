# Crux — Alpha v1

Exam-prep app for university students in Ireland. The student answers a 7-question quiz and gets a day-by-day study plan, then the app guides each session with a timer and clear steps.

> Working name. Alpha build for functional testing only.

## What's in this version

- **Onboarding quiz** — exam date, hours per day, exam type, content covered, target grade, biggest struggle, study time
- **Plan generation** — sessions picked from the quiz answers (triage, Feynman, active recall, blurting, answer outlines, practice problems, mock exam, quick review)
- **Plan reveal** — day-by-day plan with the reason behind each choice
- **Today screen** — countdown to the exam, sessions of the day, progress
- **Session mode** — timer, step-by-step instructions, "Not sure" button that sends items to the end-of-day quick review
- **Check-in** — Easy / OK / Hard after each session; "Hard" adds a review to the next day; essay sessions include a self-check

- **Motion** — quiz text and transitions with anime.js v4 (splitText, SVG morph, drawable check); respects the phone's reduce-motion setting

## Known limits (alpha)

- Plan and progress are saved in the browser on this device only (no account, no sync)
- Sign-in is simulated
- Flashcards can't be created inside the app yet
- "Fast demo" toggle in session mode speeds the timer up for testing

## How to test

Open `index.html` on a phone, or enable GitHub Pages (Settings → Pages → deploy from `main`, root folder) and open the generated link.

Best test: use it for a real exam, follow the plan to exam day, and note where you stopped, what you skipped and what felt confusing.
