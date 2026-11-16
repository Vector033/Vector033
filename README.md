# Nawat Wattanawong

**Full-stack developer · Computer Science, Chiang Mai University (year 3)**

I build web apps end to end, put them online, and measure whether they work. Five apps below are live and built solo; Project Z was built in a team of four and signed off by a client. I'm looking for a full-term co-op placement from June to October 2027, and I'm open to relocation.

[![Portfolio](https://img.shields.io/badge/Portfolio-vector033.github.io-ec4899?style=flat-square&logo=githubpages&logoColor=white)](https://vector033.github.io)
[![Email](https://img.shields.io/badge/Email-nawat__wattanawong%40cmu.ac.th-555555?style=flat-square&logo=gmail&logoColor=white)](mailto:nawat_wattanawong@cmu.ac.th)
![Location](https://img.shields.io/badge/Location-Chiang_Mai%2C_Thailand-555555?style=flat-square)

---

## Featured

### MorPlan: CMU timetable planner and Thai regulation Q&A

<a href="https://morplan.vercel.app">
  <img src="https://vector033.github.io/img/morplan-planner-1600.webp" alt="MorPlan week grid with five courses placed; two classes overlap and are marked in red, and an alert names the clash." width="100%" />
</a>

- Drag courses onto a week grid, or place them from the keyboard. Class, midterm, final and duplicate clashes show at once.
- Compare plans A to E side by side, share a read-only link, and export to .ics or PNG.
- Ask the university's regulations in Thai: every answer cites the document and page. On a 170-question eval, the right page is in the top 5 for 90.3% of answerable questions, and the answer-or-"not found" call is right 78.8% of the time on a held-out split.

**Tools:** Next.js 16, TypeScript, Tailwind CSS, dnd-kit, Supabase, Drizzle, Vitest + fast-check, Playwright<br/>
**Links:** [Live app](https://morplan.vercel.app)

### PingKhana: scholarship, co-op and job deadlines on the web and LINE

<a href="https://pingkhana.vercel.app">
  <img src="https://vector033.github.io/img/pingkhana-home-1280.webp" alt="PingKhana home page: 352 announcements from 13 sites and a list of the ones closing soonest." width="100%" />
</a>

- A FastAPI collector reads 13 sources (CMU faculty sites and education news) every hour, follows robots.txt, and merges an announcement posted on several sites into one. It has gathered 352 announcements.
- Gemini reads closing dates from text, posters and PDFs. The LINE bot reminds you 3 days and 1 day before a deadline, and deadlines export to .ics or Google Calendar.
- It grew from a CMU-only bot after a teacher asked for school news. Anyone can add a source by pasting a link (SSRF-guarded, admin-approved).

**Tools:** Python 3.12, FastAPI, SQLAlchemy 2, PostgreSQL, Next.js 16, LINE LIFF, Gemini, pytest<br/>
**Links:** [Live site](https://pingkhana.vercel.app)

---

## Selected Projects

| Project | Description | Tools | Demo |
| --- | --- | --- | --- |
| [Project Z](https://github.com/NexusG0/Project-Z) | Multi-tenant AI chat widget for a client, in a team of four. I was the Software Architect: three FastAPI services, Firestore schema, JWT auth and real-time Gemini chat. All 22 user stories delivered with client sign-off. | FastAPI, Vue 3, SSE, Redis, Firestore, Docker | — |
| FactFit | Tailors a résumé to a job posting without inventing facts. A code-based guard blocked 164 of 172 made-up claims on a blind held-out set. | Next.js 16, Supabase, Drizzle, Gemini, Vitest | [Live](https://factfit-five.vercel.app) |
| HarnKan | Splits trip costs in real time, makes PromptPay QR codes and reads the payment slip. 0 wrong auto-ticks on 60 synthetic slips. | Next.js 16, Supabase Realtime + RLS, PWA | [Live](https://harnkan-ten.vercel.app) |
| SlipJot | Logs expenses from photos of Thai bank slips. 93% of held-out synthetic slips fully correct, and unsure reads go to a review queue (0% silent errors). | Next.js 16, Supabase, tesseract.js, Gemini | [Live](https://slipjot.vercel.app) |

The source code of my solo projects is private for now; the live apps have demo accounts.

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
