# Tutorial
# 🧭 Devansh × Suyog — Mentorship Learning Plan

> *"The goal isn't to learn syntax. The goal is to learn how to learn."*

---

## 📌 What This Repository Is

This is a structured, week-by-week mentorship repository where **Devansh** (mentor) guides **Suyog** (mentee) through the foundational layers of software development — from web basics to systems thinking in C, and then into Python.

Every folder, every assignment, every deadline in this repo exists for one reason: to build Suyog into a developer who can **pick up any tech stack quickly** and use modern AI tools to accelerate development — without being dependent on them.

This is not a course. There are no videos to finish, no certificates to collect. The only proof of learning here is **working code, pushed on time, with honest documentation of the process.**

---

## 🎯 The Final Goal

By the end of this mentorship, Suyog should be able to:

- Look at an unfamiliar technology and build a mental model of it within days, not weeks
- Read documentation and figure things out independently before asking for help
- Debug code by *reasoning* about what the machine is doing, not by randomly changing things
- Build complete, functional projects — not just tutorial clones
- Use AI tools (ChatGPT, Claude, Copilot) as a **force multiplier**, not a crutch
- Contribute meaningfully to real-world codebases with minimal hand-holding

This is the developer Devansh has become through years of curiosity and deliberate experimentation. This plan is designed to compress that journey — not by making it easier, but by making it more intentional.

---

## 👥 People

| Role | Name | Responsibility |
|---|---|---|
| **Mentor** | Devansh | Designs assignments, reviews submissions, evaluates quality, provides feedback |
| **Mentee** | Suyog | Studies concepts, builds assignments, pushes code on time, asks good questions |

---

## 📁 Repository Structure

```
/
├── README.md                  ← You are here. Read this fully before anything else.
├── week-1/
│   ├── ASSIGNMENT.md          ← Read-only. Written by Devansh. Do not edit.
│   └── [Suyog's work files]   ← All submissions go here.
├── week-2/
│   ├── ASSIGNMENT.md
│   └── [Suyog's work files]
├── week-3/
│   ├── ASSIGNMENT.md
│   └── [Suyog's work files]
└── ... and so on
```

Each `week-N/` folder contains:
- **`ASSIGNMENT.md`** — Written and locked by Devansh. Contains the concepts to study, tasks to complete, and resources to refer. Suyog must not edit this file.
- **Suyog's submission files** — Code, notes, projects, or whatever the assignment requires — all go inside the same week folder.

---

## 📅 Assignment Schedule & Rules

### How it works

- Devansh releases the next week's `ASSIGNMENT.md` every **Sunday evening**
- Suyog has until the following **Saturday evening** to complete and push all work
- One full week. No extensions unless discussed in advance with a genuine reason.

### Rules Suyog must follow

1. **Push on time.** The Saturday evening deadline is non-negotiable. An incomplete push is better than no push — commit whatever you have with honest notes about what's missing and why.
2. **Work inside the week folder.** All files related to a week's assignment go inside that week's folder. No exceptions.
3. **Do not edit `ASSIGNMENT.md`.** This file is Devansh's — it's the source of truth for what was assigned. If Suyog has questions or notes about the assignment, they go in a separate `NOTES.md` inside the same folder.
4. **Document your process.** Every submission should include brief notes — what you understood, what confused you, what broke, what you figured out. A working project with no reflection is worth less than a half-broken project with honest documentation.
5. **Disclose AI usage honestly.** See the AI policy section below.

### How Devansh evaluates

Devansh will review the submission after Saturday and push feedback — either as comments in code, a `FEEDBACK.md` inside the week folder, or via direct conversation. Evaluation is based on:

- Does the code actually work?
- Does Suyog understand *why* it works — or just that it does?
- Is the work original, or copy-pasted from a tutorial?
- Are the reflection notes honest and thoughtful?

---

## 🤖 AI Tools Policy

This is important. Read it carefully.

The end goal of this mentorship is to make Suyog someone who uses AI tools the way senior developers do — as a **thinking partner and accelerator**, not as someone who outsources their thinking to a chatbot. That skill requires a foundation that AI cannot build for you.

### Phase 1 & 2 — No AI Tools

During the HTML/CSS/JS phase and the C programming phase: **no AI assistance of any kind.**

This means no ChatGPT, no Claude, no Copilot, no AI-powered autocomplete.

Use Google. Use MDN. Use W3Schools. Use Stack Overflow. Sit with the bug for an hour before asking for help. That discomfort is exactly where learning happens.

*Why?* Because these phases are specifically designed to build your mental model from the ground up. The moment you ask Claude to fix your pointer error, you've short-circuited the process that was supposed to build your reasoning ability. You'll get the right answer and learn nothing.

### Phase 3 onwards — Conditional AI Use

From the Python phase onward, AI tools are permitted — with strict conditions:

- **Attempt first, always.** Try the problem yourself before opening any AI tool. Document where you got stuck.
- **Use AI to understand, not to generate.** Ask Claude to explain a concept. Don't ask it to write your code.
- **Rewrite from scratch.** If AI explained something or showed an example, close the window and rewrite it yourself from memory. If you can't, you didn't learn it.
- **No black-box copying.** Pasting AI output into your submission without understanding it line by line is the same as not doing the assignment.

### The honesty rule — applies to all phases

> If you used AI anywhere in an assignment — for any reason — you must say so at the top of the relevant file. State what you used, what you asked, and what you learned from it.

Hiding AI usage is treated the same as not submitting the assignment. This isn't about catching you — it's about building the habit of intellectual honesty that makes great engineers trustworthy.

---

## 🗺️ The Learning Plan

### Overview

| Phase | Focus | Duration | AI Allowed? |
|---|---|---|---|
| Phase 1 | HTML, CSS, Vanilla JS | 6–8 weeks | ❌ No |
| Phase 2 | C Programming | 8–10 weeks | ❌ No |
| Phase 3 | Python | 4–5 weeks | ✅ Conditional |
| Phase 4 | Onwards (decided together) | Open-ended | ✅ Full use |

Total foundation: approximately **5–6 months**. After that, Suyog should be ready to learn any stack independently with AI as a tool.

---

### Phase 1 — Web Fundamentals (6–8 weeks)

**The rule for this phase:** learn each layer in isolation before combining them.

#### HTML (Weeks 1–2)
- Semantic structure, headings, paragraphs, lists, links, images
- Forms and input elements
- Tables
- **Goal:** Build a static personal page using only HTML. No CSS — intentionally ugly. Raw structure, nothing else.

#### CSS (Weeks 3–4)
- Box model, selectors, specificity
- Flexbox and Grid layouts
- Responsive design and media queries
- Basic typography and color
- **Goal:** Take the ugly HTML page from Phase 1 and make it clean, organized, and responsive on both desktop and mobile.

#### Vanilla JavaScript (Weeks 5–8)
- Variables, data types, functions, loops, conditionals
- DOM manipulation — selecting elements, changing content, handling events
- Fetch API — calling a public API and displaying real data
- localStorage — saving state in the browser
- Browser DevTools — the console is your best friend
- **Goal:** Build a functional interactive project — a to-do app, a weather widget using a public API, or a quiz app. No libraries, no frameworks. Everything from scratch.

**Phase 1 Milestone:** One complete project built from scratch using only HTML, CSS, and Vanilla JS. It must be functional, not just visual.

---

### Phase 2 — C Programming (8–10 weeks)

This is the hardest phase, and also the most important one. Do not rush it.

**Why C?** C forces you to understand what actually happens when code runs — memory, the call stack, how variables are stored, what a pointer actually is. Languages like Python hide all of this from you. If you learn C properly, every other language becomes easier to understand because you'll know what it's doing under the hood.

#### Weeks 1–2 — Syntax and Control Flow
- Data types, variables, operators
- Conditionals, loops, functions
- Basic I/O with `printf` and `scanf`
- **Goal:** Solve structured problems — number patterns, basic calculations, simple menu programs

#### Weeks 3–4 — Arrays, Strings, and Pointers
- Arrays and how they sit in memory
- Strings as character arrays
- Pointers — declaration, dereferencing, pointer arithmetic
- **Do not move on until pointers make sense.** Draw them on paper. Trace the memory manually.

#### Weeks 5–6 — Structs and Memory Management
- Defining and using structs
- Dynamic memory allocation — `malloc`, `calloc`, `free`
- File I/O — reading and writing files
- Understanding memory leaks

#### Weeks 7–10 — Project
- Build one non-trivial project using everything covered: a student record system, a text-based game, a file-based database, or similar
- First build it. Then debug it properly. Then refactor it to be clean.
- The goal isn't a perfect first version. The goal is understanding *why* your first version was messy.

**Phase 2 Milestone:** One functional, non-trivial C project that uses structs, pointers, and file I/O. Code must be your own. No AI.

---

### Phase 3 — Python (4–5 weeks)

After C, Python should feel like cheating. That's the point.

#### Week 1 — Syntax
- Python syntax, data types, control flow, functions
- Translate patterns you already know from C into Python
- Understand what Python is abstracting away under the hood (you'll know now)

#### Week 2 — OOP, Files, Standard Library
- Classes and objects
- File handling
- Useful standard library modules — `os`, `json`, `datetime`, `random`

#### Weeks 3–4 — Data and Libraries
- `numpy` basics — arrays, operations
- `pandas` basics — dataframes, filtering, grouping
- `matplotlib` — basic plots and charts

#### Week 5 — Project
- Build something using real data: clean a public dataset, analyze it, and visualize findings
- Or: build a simple ML model using `scikit-learn` on a public dataset
- AI tools are allowed here under the conditions described in the AI policy above

**Phase 3 Milestone:** One data or ML project using real data, with documented analysis and honest notes on what AI was used for (if anything).

---

### Phase 4 — Beyond (decided together)

After Phase 3, Devansh and Suyog will sit together and decide the next direction based on where Suyog's interest and strengths have developed. Possible paths include:

- Full-stack web development (Node.js, React, databases)
- Mobile app development
- Machine learning and AI engineering
- Cloud infrastructure and deployment
- Systems programming

By Phase 4, AI tools are fully enabled. The foundation has been built. The goal now is to learn how to use AI to move fast without losing the ability to think.

---

## 📐 How to Think About Learning (A Note from Devansh)

I didn't get here by finishing courses. I got here by being genuinely curious and experimenting constantly — breaking things, fixing them, wondering *what happens if I change this?*

Every week in this plan, before you consider the assignment complete, ask yourself:

- Do I understand *why* this works, or just *that* it works?
- What happens if I break this in a specific way?
- Could I explain this to someone else from scratch?
- What question did this week raise that I don't have an answer to yet?

If you can't answer the first question honestly with "I understand why" — you're not done yet.

The assignments are the minimum. Curiosity is the actual curriculum.

---

## ✅ Quick Reference — Suyog's Checklist Each Week

- [ ] Read `ASSIGNMENT.md` fully on Sunday evening before starting
- [ ] Study the concepts using the listed resources
- [ ] Build the required tasks inside the week folder
- [ ] Write a `NOTES.md` documenting what you understood, what was hard, and what broke
- [ ] If AI was used (Phase 3+), document it honestly at the top of the relevant file
- [ ] Push all work to GitHub before Saturday evening
- [ ] Do not edit `ASSIGNMENT.md`

---

*This README is a living document. Devansh may update the structure, rules, or learning plan as the mentorship progresses. Always read the latest version before starting a new week.*

---

**Repository maintained by:** Devansh (mentor) · **Active mentee:** Suyog