# 📋 Week 1 Assignment — HTML Foundations

> **Assigned by:** Devansh
> **Released:** Sunday Evening (Week 1)
> **Deadline:** Saturday Evening (Week 1) — no extensions
> **Phase:** Phase 1 — Web Fundamentals

---

> ⚠️ **Read this file fully before writing a single line of code.**
> This file is read-only. Do not edit it.
> All your work goes in separate files inside this `week-1/` folder.

---

## 🎯 What This Week Is About

This week is about one thing: **understanding that HTML is structure, not style.**

Every tag you write this week is a decision — not about how something looks, but about what something *is*. A heading isn't big text. It's a heading. A nav isn't a box on the side. It's navigation. A table isn't a layout tool. It's tabular data.

By the end of this week, you should be able to look at any webpage, open the inspector, and make sense of its HTML skeleton. That skill will follow you for the rest of your career.

There is no CSS this week. The page will look ugly. That's not a problem — it's the assignment. Feel that limitation. It's setting something up.

---

## 📚 Concepts to Study

Study these **in order**. Don't skip ahead.

---

### 1. How the Web Works (Conceptual — No Code)

Before you write a single tag, you need a mental model of what HTML actually is and where it lives.

Understand the following at a high level — no deep networking theory, just the picture:
- What happens when you type a URL into a browser and press Enter?
- What is a "request" and what is a "response"?
- What does the browser actually *do* with an HTML file once it receives it?
- What is the DOM (Document Object Model)? You don't need to manipulate it yet — just know it exists and what it represents.

**Resource:** [How the Web Works — MDN](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

---

### 2. HTML Document Structure

Every valid HTML file follows a structure. Understand each piece — don't just copy it blindly.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
  </head>
  <body>
    <!-- Content goes here -->
  </body>
</html>
```

For each line above, you should be able to answer: *what does this do, and what happens if I remove it?*

Topics to understand:
- What `<!DOCTYPE html>` tells the browser
- What lives in `<head>` vs `<body>` — and why
- What `charset="UTF-8"` means and why it matters
- What the `viewport` meta tag does (you'll feel this more in Week 3, but understand it now)

**Resource:** [HTML Document Structure — MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)

---

### 3. Semantic HTML — The Most Important Concept This Week

Most beginners treat HTML as a visual tool. `<h1>` makes text big. `<p>` adds spacing. That thinking will slow you down.

HTML tags describe **what content is** — not how it looks. That's CSS's job. HTML's job is meaning.

A `<nav>` tells the browser, search engines, and screen readers: *"this is navigation."* A `<article>` says: *"this is a self-contained piece of content."* A `<div>` says: *"this is... a thing."* — which is why you reach for semantic tags first and `<div>` only when nothing else fits.

**Tags to learn and understand:**

| Tag | What it means |
|---|---|
| `<h1>` – `<h6>` | Headings — hierarchy, not size. One `<h1>` per page. |
| `<p>` | A paragraph of text |
| `<strong>` | Important text (not just bold) |
| `<em>` | Emphasized text (not just italic) |
| `<header>` | Introductory content for a page or section |
| `<nav>` | A block of navigation links |
| `<main>` | The primary content of the page — only one per page |
| `<section>` | A thematic grouping of content |
| `<article>` | Self-contained content (a blog post, a profile card) |
| `<aside>` | Content tangentially related to the main content |
| `<footer>` | Footer for a page or section |
| `<div>` | Generic container — use only when no semantic tag fits |
| `<span>` | Generic inline container — same rule as `<div>` |

**The question to ask before every tag:** *What is this content, not how should it look?*

**Resource:** [Semantics in HTML — MDN](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html)

---

### 4. Text, Lists, and Basic Inline Elements

- `<p>`, `<br>`, `<hr>`
- `<strong>` vs `<b>` — what's the difference, and when does it matter?
- `<em>` vs `<i>` — same question
- Unordered lists: `<ul>` + `<li>`
- Ordered lists: `<ol>` + `<li>`
- Nested lists — a list inside a list
- When do you use `<ol>` vs `<ul>`? Think about this with real examples.

**Resource:** [HTML Text Fundamentals — MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

---

### 5. Links and Navigation

- `<a href="">` — the anchor tag
- Absolute URLs (`https://google.com`) vs relative URLs (`./about.html`)
- `target="_blank"` — opening in a new tab. And why you should always pair it with `rel="noopener noreferrer"` (look this up — it's a security thing)
- Anchor links — linking to a specific section on the same page using `id` attributes

```html
<a href="#contact">Jump to Contact</a>

<!-- Somewhere else on the page -->
<section id="contact">
  ...
</section>
```

**Resource:** [Creating Hyperlinks — MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)

---

### 6. Images

- `<img src="" alt="">` — the two required attributes
- The `alt` attribute is not optional. It describes what the image is for users who can't see it (screen readers, failed loads, search engines). A missing or empty `alt` on an informational image is a mistake.
- Exception: decorative images that add no meaning can have `alt=""` — but you must make that decision consciously, not lazily.
- Relative vs absolute paths for `src`
- `width` and `height` attributes — why setting them matters for page layout stability

**Resource:** [Images in HTML — MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)

---

### 7. Tables

Tables are for tabular data — information that has a natural row-and-column structure. They are **not** for page layout. Ever. (Old websites did this. It was a mistake. Don't repeat it.)

- `<table>`, `<thead>`, `<tbody>`, `<tfoot>`
- `<tr>` — table row
- `<th>` — table header cell (semantic — means "this is a header")
- `<td>` — table data cell
- The `scope` attribute on `<th>` — `scope="col"` or `scope="row"` for accessibility

```html
<table>
  <thead>
    <tr>
      <th scope="col">Name</th>
      <th scope="col">Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Suyog</td>
      <td>18</td>
    </tr>
  </tbody>
</table>
```

**Resource:** [HTML Tables — MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

---

### 8. Forms — Basics Only

Forms don't need to actually submit anywhere this week. Understand the structure and the why.

- `<form>` — the container. `action` (where it submits) and `method` (`GET` vs `POST`) attributes — understand what they mean conceptually
- `<label>` and `<input>` — always pair them. Always. Use the `for` attribute on `<label>` matching the `id` on `<input>`. This is accessibility, not decoration.
- Input types: `text`, `email`, `password`, `number`, `checkbox`, `radio`, `submit`
- `<textarea>` — for multi-line text
- `<select>` and `<option>` — dropdowns
- `<button>` vs `<input type="submit">` — know the difference

```html
<!-- Correct — label is associated with input -->
<label for="email">Email address</label>
<input type="email" id="email" name="email">

<!-- Wrong — label is just text floating near an input -->
<label>Email address</label>
<input type="email">
```

**Resource:** [Web Forms — MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)

---

## 🛠️ Tasks

---

### Task 1 — Set Up Your Environment

Before writing any HTML, set up properly:

1. Install [VS Code](https://code.visualstudio.com/) if you haven't already
2. Install the **Live Server** extension in VS Code (by Ritwick Dey) — this lets you see your HTML update in the browser in real time as you save
3. Create a file called `index.html` inside the `week-1/` folder
4. Write the base HTML document structure from memory (not copy-paste) and open it with Live Server
5. Confirm it opens in your browser — even if it's blank

**Deliverable:** `index.html` exists in `week-1/` and has a valid base structure.

---

### Task 2 — Build Your Personal Profile Page

Build a single-page personal profile in `index.html` using only HTML. No CSS. No JS. No frameworks.

Your page must include all of the following:

#### 2a. Navigation
- A `<nav>` at the top with anchor links that jump to each section of the page
- At minimum: About, Skills, Schedule, Contact

#### 2b. About Section
- Your name in an `<h1>` (only one `<h1>` on the page)
- A short bio in one or two `<p>` tags — who you are, what you're learning, why
- At least one image (can be a placeholder from [https://placekitten.com](https://placekitten.com) or any image you choose) with a meaningful `alt` attribute

#### 2c. Skills or Interests Section
- An unordered list of at least 5 things you know or are learning
- A nested list inside at least one item — for example, "Programming" with sub-items for each language

#### 2d. Weekly Schedule Table
- A table showing your weekly schedule (or any structured data you prefer — book list, comparison table, etc.)
- Must include `<thead>`, `<tbody>`, `<th>` with `scope` attributes, and `<td>`
- At least 4 columns and 5 rows of real data

#### 2e. Contact Section
- A form with the following fields:
  - Name (text input)
  - Email (email input)
  - Message (textarea)
  - A subject dropdown (select) with at least 3 options
  - A submit button
- Every input must have a properly associated `<label>`
- The form does not need to submit anywhere — no `action` required

#### 2f. Footer
- A `<footer>` with your name and a note like "Learning HTML — Week 1"
- At least one external link (to MDN, GitHub, or anywhere relevant) that opens in a new tab with `rel="noopener noreferrer"`

**Deliverable:** A complete `index.html` that passes the following self-check:

- [ ] One `<h1>` on the entire page
- [ ] Navigation anchor links actually jump to the right sections
- [ ] No tag is used purely for visual effect — every tag has a semantic reason
- [ ] Every image has a meaningful `alt` attribute
- [ ] Every form input has an associated `<label>` using `for` and `id`
- [ ] Table uses `<thead>`, `<tbody>`, and `scope` on `<th>` elements
- [ ] Page structure uses semantic tags — `<header>`, `<main>`, `<section>`, `<footer>`, `<nav>`

---

### Task 3 — The Inspector Challenge (Thinking Task)

Open **3 websites** you actually use — could be YouTube, Instagram, Zomato, GitHub, anything.

On each one:
1. Right-click anywhere → **Inspect** (or press `F12`)
2. Go to the **Elements** tab
3. Spend 10 minutes reading the HTML structure

Then write a short note in your `NOTES.md` — **at least 10 lines total** — covering:
- What semantic tags did you spot? (`<nav>`, `<article>`, `<main>`, etc.)
- Did you see any tags you don't recognise? List them.
- Did any site use a `<div>` for something that probably deserved a semantic tag?
- What surprised you?
- What did you not understand?

There are no wrong answers here. The goal is observation and honest reflection.

**Deliverable:** `NOTES.md` in `week-1/` with your inspector observations.

---

### Task 4 — Break It on Purpose

Pick any 5 things from the list below. For each one: make the change, observe what happens in the browser, then revert it. Document all 5 observations in your `NOTES.md` under a section called `## Break Log`.

- Remove `<!DOCTYPE html>` — does anything change visibly?
- Remove the `<head>` block entirely
- Put content directly in `<html>` without `<body>`
- Nest a `<p>` inside another `<p>`
- Use `<h3>` before you've used `<h2>`
- Remove the `alt` attribute from an image
- Give two elements the same `id`
- Remove the `for` attribute from a `<label>`
- Put a `<div>` inside a `<span>`
- Use a `<table>` with `<td>` but no `<tr>`

For each: write one sentence on what you did, and one sentence on what happened (or didn't happen) and what you think that tells you.

**Deliverable:** A `## Break Log` section in your `NOTES.md` with 5 entries.

---

## 📂 What to Submit

Your `week-1/` folder should contain the following before the deadline:

```
week-1/
├── ASSIGNMENT.md        ← This file. Not touched.
├── index.html           ← Your personal profile page
└── NOTES.md             ← Inspector observations + Break Log
```

No other files are required. If you used any images locally, put them in a `week-1/images/` subfolder and reference them with relative paths.

---

## 🚫 Rules for This Week

- **No CSS.** Not a single `style` attribute, not a `<style>` tag, not a `.css` file. If you add CSS, the assignment is incomplete.
- **No JavaScript.**
- **No AI tools.** No ChatGPT, no Claude, no Copilot. Use MDN, W3Schools, and your own experimentation.
- **No copy-pasting code** from tutorials. Type everything yourself. Muscle memory matters more than you think right now.

---

## 📬 Submission

Push everything to GitHub before **Saturday evening**. If you're not done, push what you have with a note at the top of `NOTES.md` explaining what's missing and why.

An honest incomplete is better than a silent miss.

---

## 💬 A Note from Devansh

The page you build this week will look terrible. That's the point.

Don't spend time trying to make it look better — you don't have the tools for that yet, and reaching for tricks to style things in HTML alone is exactly the wrong instinct to build. Sit with the ugly page. Notice what's missing. That frustration is doing something.

When you open the inspector on YouTube or GitHub and see thousands of lines of HTML — don't be intimidated. Every one of those tags is just a decision someone made about what a piece of content *is*. By Saturday, you'll be making those same decisions.

Write the code. Break the code. Read the docs. Push by Saturday.

---

*This file is read-only. Do not edit it. All work goes in separate files.*
*Assignment designed by Devansh for Suyog — Week 1 of the mentorship plan.*