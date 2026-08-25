# Content to Fill In

Everything in `index.html` that is a placeholder. Nothing here was invented — I left
these blank rather than guessing at your real dates, employers or institutions.

Work through the list, then delete this file before you publish.

---

## 1. Contact links (appears 3 times in the file)

| Placeholder | Replace with |
|---|---|
| `YOUR_EMAIL` | The email address you want recruiters to use |
| `YOUR_LINKEDIN_URL` | `https://linkedin.com/in/your-handle` |
| `YOUR_GITHUB_URL` | `https://github.com/your-username` |

Find them all at once:
```bash
grep -n "YOUR_EMAIL\|YOUR_LINKEDIN_URL\|YOUR_GITHUB_URL" index.html
```

---

## 2. Project links (in the "Signal vs. Noise" card)

Fill these in once the music project is deployed — the steps are in that repo's
`HOW_TO_PUBLISH.md`.

| Placeholder | Replace with |
|---|---|
| `PROJECT_SITE_URL` | `https://YOUR_USERNAME.github.io/music-market-intelligence/` |
| `PROJECT_PAPER_URL` | `https://github.com/YOUR_USERNAME/music-market-intelligence/blob/main/paper/Signal-vs-Noise-Paper.md` |
| `PROJECT_TABLEAU_URL` | Your Tableau Public workbook URL |
| `PROJECT_REPO_URL` | `https://github.com/YOUR_USERNAME/music-market-intelligence` |

---

## 3. Education (Section 04)

Three entries are stubbed. For each, replace:
- `[YEAR – YEAR]` — e.g. `2024 – 2026`
- `[UNIVERSITY NAME]` / `[CONSERVATORY / UNIVERSITY NAME]`
- `[DEGREE]` for the bachelor's entry
- The description line in each

**If you only have two degrees, delete the third `<div class="entry">` block entirely.**

For the Master of Music entry, add your instrument and one or two concrete highlights —
competitions, ensembles, recitals, teaching. Hiring managers outside music will not know
what is impressive, so say it plainly ("principal [instrument], [ensemble name]").

---

## 4. Experience (Section 04)

Two entries are stubbed. For each: job title, organisation, dates, and 2–3 bullets.

**Make every bullet a number.** This is the single highest-return edit on the page.
Compare:

> ~~Coordinated events and managed schedules~~
>
> **Coordinated 40+ recitals and masterclasses per semester across 12 faculty,
> 200 students and 3 venues, cutting scheduling conflicts to zero.**

Pull the numbers from the experience already described in your résumé — student counts,
event counts, budget, audience size, engagement lift, hours saved.

Add more entries by copying a `<div class="entry">…</div>` block.

---

## 5. Résumé PDF

Export your résumé as PDF and save it as:

```
assets/Rebecca-Wu-Resume.pdf
```

The "Résumé" buttons already point there. If you would rather not host a résumé publicly,
delete the two `<a class="btn" href="assets/Rebecca-Wu-Resume.pdf">` links instead.

---

## 6. Remove the yellow note box

Once the Background section is filled in, delete this block from `index.html`:

```html
<div class="note"><b>To complete:</b> …</div>
```

---

## 7. Optional but worth it

- **Add a photo.** A simple headshot in the hero adds a lot of warmth. Save it to
  `assets/` and add an `<img>` in the `.hero` block.
- **Tighten the headline.** The current one ("I turn what audiences actually do into
  decisions the music business can act on") is a positioning statement, not a job title.
  Keep it if it sounds like you; rewrite it if it does not. It should sound like something
  you would actually say out loud in an interview.
- **Reorder the projects.** Whichever project is most relevant to the role you are applying
  for should be first.

---

## Final check before publishing

```bash
grep -n "YOUR_\|PROJECT_\|\[YEAR\|\[UNIVERSITY\|\[JOB TITLE\|\[ORGANISATION\|\[Achievement" index.html
```

If that returns nothing, the page is ready.
