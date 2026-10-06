# AI60 Growth Engine

A student-to-student referral and growth system built for the NxtWave Growth Intern Challenge.

**Live prototype → [subhashchandra1224.github.io/ai60-growth-engine](https://subhashchandra1224.github.io/ai60-growth-engine/)**

---

## What this is

A working prototype that demonstrates how to get 500 final-year engineering students to register for a free 60-minute AI workshop — with a ₹2,000 budget and 7 days.

Rather than building a static landing page, I built the full growth system: registration, referral loop, contextual sharing, leaderboard, analytics dashboard, and an interactive growth simulator.

---

## The problem it solves

₹2,000 cannot buy 500 registrations through paid ads alone.

The only path to 500 is a distribution loop — where each registration creates the next one. This prototype operationalises that loop end-to-end.

---

## What's inside

| Feature | What it does |
|---|---|
| **Registration form** | Captures student details, generates a unique referral code (`AI60-NAME-XXXX`) |
| **Referral dashboard** | Tracks referral progress, shows reward milestones (3 referrals → AI Project Starter Kit, 5 → AI Interview Guide) |
| **Smart Share Assistant** | Generates contextual WhatsApp messages — 4 audiences × 3 tones = 12 templates. Instant, no API needed |
| **Leaderboard** | Shows top referrers to create social proof and healthy competition |
| **Analytics dashboard** | Campaign funnel, channel breakdown, cost per registration, direct vs referral split |
| **Growth Simulator** | Interactive sliders — change seeders, share rate, referrals per sharer — and see the projected total update live |
| **7-Day Strategy** | Campaign timeline from validate → scale → referral push → urgency |

---

## The growth model

```
Campus Seeders (20) × Registrations/Seeder (12)  =  240 direct
240 × Share Rate (40%) × Referrals/Sharer (1.5)  =  144 referral
Tech Clubs & Communities                          =   76
Paid Instagram experiment                         =   40
                                           Total  =  500
```

**92% of projected registrations come from organic/community distribution.**

We're not trying to buy 500 registrations with ₹2,000. We're using ₹2,000 to activate a distribution loop.

---

## One decision I'm proud of

The Smart Share Assistant generates messages using deterministic templates, not a live LLM API.

AI suggested connecting Gemini for dynamic generation. I rejected it — an API call adds latency, requires exposing a key in a frontend file, and creates a failure point during a live demo, without improving the growth outcome. Templates work instantly, every time. The architecture allows an LLM to replace them later.

---

## Tech stack

- Pure HTML, CSS, vanilla JavaScript — no frameworks
- localStorage for session persistence
- Zero external APIs or backend dependencies
- Deployable as a single file on GitHub Pages

---

## Budget philosophy

| Allocation | Amount | Reasoning |
|---|---|---|
| Instagram A/B creative test | ₹500 | Validate message hook before scaling |
| Scale winning creative | ₹500 | Only after signal confirmed |
| Referral / ambassador incentives | ₹700 | Reserved, not pre-spent |
| Reserve | ₹300 | Best-performing experiment |
| **Total** | **₹2,000** | |

Spreading ₹2,000 across 4 channels produces no usable signal on any of them. Focus produces data. Data produces decisions.

---

## How to run locally

Download `index.html` and open it in any browser. No server, no install, no dependencies.

---

*Built for the NxtWave Growth Intern Challenge by Subhash Chandra.*
