# Crux — Alpha v3

Exam-prep app for university students in Ireland. The student answers a 7-question quiz and gets a day-by-day study plan, then the app guides every session, tracks what they know and brings weak points back until exam day.

> Working name. Alpha build for functional testing only.

## What's in this version

- **Onboarding quiz** — exam date, hours per day, exam type, content covered, target grade, biggest struggle, study time
- **Plan generation** — sessions picked from the quiz answers (triage, Feynman, flashcards, blurting, answer outlines, practice problems, mock exam, quick review)
- **What could come up in the exam** — the student lists the module's topics (or pastes the whole syllabus, one per line) and rates each one: no idea / not sure / got it, plus a star for topics that keep coming up in past papers
- **Sessions tied to topics** — each session targets one topic, in attack order (no idea + starred first)
- **Technique by topic state** — no idea → Feynman first; not sure → flashcards, blurting or questions; got it → only in reviews
- **Self-rating after every technique** — updates the topic's colour; a topic only turns "got it" after a good result on two different days
- **Flashcards, three ways** — ready questions generated from the topic name (no typing), quick cards (write a fact, tap the word to hide) and paste notes (one `question - answer` per line); grade Missed / Not sure / Got it
- **Spaced review** — cards move through 4 boxes; missed and unsure cards come back the same evening or next day; the last day reviews everything not yet solid
- **Deep focus** — Pomodoro presets (25/5 ×4, 50/10 ×2, 90 min flow) available any time, with optional topic
- **Focus guard** — during focus timers the app counts every time the student leaves it; zero exits earns a perfect-focus bonus. Screen stays awake while the timer runs
- **Daily pills** — 3 two-minute quick hits per day using the weakest cards, or a 3-facts recall prompt
- **Rewards** — XP, levels, card combos, day streak, exam readiness %, "topic mastered" moment, reward screen after each session
- **Languages** — English and Brazilian Portuguese; EN/PT toggle at the top, opens in Portuguese when the phone is set to Portuguese
- **Motion** — anime.js v4 (splitText, SVG morph, drawable check); respects the phone's reduce-motion setting

## Known limits (alpha)

- Plan and progress are saved in the browser on this device only (no account, no sync)
- Sign-in is simulated
- No push notifications yet: pills are shown in the app, not sent to the phone
- No real app blocking (like Opal): a web app can't block other apps; that needs the native app (iOS Screen Time API / Android usage access)
- "Fast demo" toggle in session mode speeds the timer up for testing

## How to test

Live: https://studyappav1.vercel.app

Best test: use it for a real exam, follow the plan to exam day, and note where you stopped, what you skipped and what felt confusing.
