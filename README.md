# Rebecca Wu — Personal Portfolio

A single-page portfolio site. One self-contained HTML file, no build step, no framework,
no dependencies, and **free to host permanently**.

---

## Before you publish

Work through **[CONTENT-TO-FILL.md](CONTENT-TO-FILL.md)** — it lists every placeholder in
the page, in order. Nothing about your education, employers or dates was invented, so those
sections are stubbed and waiting for you.

---

## Preview it locally

Just open the file:
```bash
open index.html
```
Or serve it, which better matches how it will behave live:
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## Publish it free (GitHub Pages) — about 10 minutes

1. Create a repository at https://github.com/new
   - **Name it `Reby0318.github.io`** — using your exact GitHub username. That special
     name gives you the clean URL `https://Reby0318.github.io` with no folder suffix,
     which looks far better on a résumé.
   - Set it to **Public**, and do not add a README.
2. Push this folder:
   ```bash
   cd ~/Projects/rebecca-wu-portfolio
   git remote add origin https://github.com/Reby0318/Reby0318.github.io.git
   git branch -M main
   git push -u origin main
   ```
3. Go to **Settings → Pages**, set **Source** to `Deploy from a branch`,
   **Branch** to `main` and folder to `/ (root)`, then **Save**.
4. Wait 1–2 minutes. Your site is live at **`https://Reby0318.github.io`**.

To update it later: edit `index.html`, then
```bash
git add -A && git commit -m "Update portfolio" && git push
```
The live site updates within a minute.

---

## Why GitHub Pages rather than Google Sites or Lovable

| | GitHub Pages | Google Sites | Lovable / Framer / Wix |
|---|---|---|---|
| Cost | Free forever | Free | Free tier, but paid to remove branding or use a custom domain |
| URL | `yourname.github.io` | `sites.google.com/view/…` | `yourproject.lovable.app` |
| Looks bespoke | Yes — full control of the design | No — obviously a template | Depends |
| Vendor lock-in | None, it is just a file | Moderate | High |
| Signals technical skill | **Yes** | No | Slightly |

For business-intelligence and analyst roles, hosting your own site on GitHub is a small,
free, credible signal in itself. It is the same place your project code lives.

**Alternative if you prefer drag-and-drop:** drop this folder onto
https://app.netlify.com/drop — it publishes instantly, free, no account needed. You can
add a custom domain later on either platform.

---

## Adding a new project later

Copy one `<article class="card">…</article>` block in the "Selected work" section and edit it.

The badge controls the label:
- `<span class="badge live">Published</span>` — a finished project
- `<span class="badge plan">In progress</span>` or `Planned`

The `.metrics` block is optional but high impact — use it only when you have real numbers.
**Put your strongest project first**, and reorder for the role you are applying to.

---

## Design notes

- Adapts automatically to light and dark mode
- Responsive down to phone width
- No external requests at all: no fonts, no CDN, no analytics, no tracking — so it loads
  instantly and works offline
- Serif display type is a deliberate nod to the classical background; the sans-serif body
  keeps it readable and current

---

## Custom domain (optional, ~$12/year)

If you buy a domain such as `rebeccawu.com`:
1. Add a file named `CNAME` to this folder containing just `rebeccawu.com`
2. At your registrar, point an `A` record at GitHub's IPs (listed in
   [GitHub's docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))
3. In **Settings → Pages**, enter the domain and tick **Enforce HTTPS**

This is the only part of the setup that costs anything, and it is entirely optional.
