# Nawat Wattanawong

**Full-stack developer · Computer Science, Chiang Mai University (year 3)**

I build web apps end to end, put them online, and measure whether they work. Five apps below are live and built solo; Project Z was built in a team of four and signed off by a client. I'm looking for a full-term co-op placement from June to October 2027, and I'm open to relocation.

[![Portfolio](https://img.shields.io/badge/Portfolio-vector033.github.io-ec4899?style=flat-square&logo=githubpages&logoColor=white)](https://vector033.github.io)
[![Email](https://img.shields.io/badge/Email-nawat__wattanawong%40cmu.ac.th-555555?style=flat-square&logo=gmail&logoColor=white)](mailto:nawat_wattanawong@cmu.ac.th)
![Location](https://img.shields.io/badge/Location-Chiang_Mai%2C_Thailand-555555?style=flat-square)

---

## Featured

### MorPlan: timetable planner and rule Q&A for any Thai university

<a href="https://morplan.vercel.app">
  <img src="https://vector033.github.io/img/morplan-planner-1600.webp" alt="MorPlan week grid with 4 courses and 12 credits; 2 clashes are marked in red and an alert names the overlapping courses." width="100%" />
</a>

- Drag courses onto a week grid or place them from the keyboard. Class, midterm, final and duplicate clashes show at once; plans A to E compare side by side and export to .ics or PNG.
- Pick any of the 77 TCAS universities and your major, and it finds your curriculum: what you passed, what is overdue and which electives fit. The browser reads your pasted course table, so MorPlan never asks for your registration password.
- Ask the university's regulations in Thai: every answer cites the document and page. On a 170-question eval, the right page is in the top 5 for 90.3% of answerable questions, and the answer-or-"not found" call is right 78.8% of the time on a held-out split. Hybrid search scored a little higher (91.7% top 5), but its embedding model is too big for a Vercel function, so production runs BM25 at about 1 ms a question.

**Tools:** Next.js 16, TypeScript, Tailwind CSS, dnd-kit, Supabase, Drizzle, Vitest + fast-check, Playwright<br/>
**Links:** [Live app](https://morplan.vercel.app) · [Source](https://github.com/Vector033/MorPlan)

### PingKhana: scholarship, co-op and job deadlines on the web and LINE

<a href="https://pingkhana.vercel.app">
  <img src="https://vector033.github.io/img/pingkhana-home-1280.webp" alt="PingKhana home page: scholarships, co-op, jobs and events that are open now, with a big countdown on the one closing soonest." width="100%" />
</a>

- A FastAPI collector reads CMU faculty sites and education news every hour. It follows robots.txt, retries on 5xx and 429, and merges an announcement posted on several sites into one. It has collected 611 announcements.
- Gemini reads closing dates from text, posters and PDFs, and a rule-based extractor takes over when Gemini fails. On 34 real held-out passages the rules scored 94.1% on a blind run, ahead of Gemini at 91.2%.
- Follow only the sources you care about, no account needed. LINE's free plan allows 300 pushes a month, so the bot sends one digest a day and saves the rest for reminders 3 days and 1 day before a deadline. Anyone can add a source by pasting a link (public hosts only, admin-approved).

**Tools:** Python 3.12, FastAPI, SQLAlchemy 2, PostgreSQL, Next.js 16, LINE LIFF, Gemini, pytest<br/>
**Links:** [Live site](https://pingkhana.vercel.app) · [Source](https://github.com/Vector033/PingKhana)

---

## Selected Projects

| Project | Description | Tools | Demo |
| --- | --- | --- | --- |
| [Project Z](https://github.com/NexusG0/Project-Z) | Multi-tenant AI chat widget for a client, in a team of four. I was the Software Architect: three FastAPI services, Firestore schema, JWT auth and real-time Gemini chat. All 22 user stories delivered with client sign-off. | FastAPI, Vue 3, SSE, Redis, Firestore, Docker | — |
| [ProofMyCV](https://github.com/Vector033/ProofMyCV) (formerly FactFit) | Tailors a résumé to each job posting without inventing facts. A code-based guard blocked 164 of 172 made-up claims on a blind held-out set and kept 24 of 30 honest bullets. Takes a job as a link, a poster photo or text (links get an SSRF check on every redirect) and tracks each application's status. | Next.js 16, Supabase, Drizzle, Gemini, Vitest | [Live](https://proofmycv.vercel.app) |
| [HarnKan](https://github.com/Vector033/HarnKan) | Splits trip costs in real time, makes PromptPay QR codes and reads the payment slip: 92% auto-ticked and 0 wrong on 60 synthetic slips. Works offline and settles in the fewest transfers (exact up to 16 people). | Next.js 16, Supabase Realtime + RLS, PWA | [Live](https://harnkan-ten.vercel.app) |
| [SlipJot](https://github.com/Vector033/SlipJot) | Logs expenses from photos of Thai bank slips. 93% of held-out synthetic slips fully correct, and unsure reads go to a review queue (0% silent errors). Only 13 of 381 slips needed an LLM to pick a category. | Next.js 16, Supabase, tesseract.js, Gemini | [Live](https://slipjot.vercel.app) |

All five solo repositories are public, with their tests and eval sets. The live apps have demo accounts.

---

## Technical Skills

| Area | Technologies |
| --- | --- |
| Frontend | TypeScript, JavaScript, Next.js (App Router, Server Actions), React, Vue 3, Tailwind CSS, PWA |
| Backend | Python, FastAPI, SQLAlchemy, REST APIs, Server-Sent Events, JWT, Redis Pub/Sub |
| Data and cloud | PostgreSQL (RLS), Supabase, Drizzle ORM, Firestore, Docker, GitHub Actions, Vercel, Render |
| AI and search | Gemini structured output, BM25 and hybrid retrieval, Thai OCR (Tesseract) |
| Testing | Vitest, fast-check, Playwright, pytest, mutmut |

---

## Education

- **B.S. in Computer Science**, Chiang Mai University, 2024 to present

## How I Work

- Every app above has an eval with a held-out set and runs its tests in CI.
- I build with AI coding agents; the tests and evals are how their output gets checked.
