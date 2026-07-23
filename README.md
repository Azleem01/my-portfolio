# Azeez Aleem — Portfolio

A single-page personal portfolio for **Azeez Aleem — Data Scientist & Machine
Learning Engineer**. Static site (HTML + CSS + vanilla JS), no build step, in a
"liquid chrome / glassmorphism" style.

## Structure

```
index.html      All sections (nav, hero, about, projects, skills, contact, footer)
styles.css      Design system (chrome / glass, responsive, reveal animations)
script.js       Mobile nav, scroll-reveal, contact form -> mailto
assets/
  headshot.jpg  Hero portrait
  about.jpg     About-section photo
```

## Run locally

Any static server works. For example:

```bash
python -m http.server 5500
# then open http://localhost:5500
```

Or just open `index.html` in a browser.

## Swap the hero photo

The hero uses `assets/headshot.jpg`. To use a different photo (e.g. a studio
headshot), just replace that file — keep the same name, and ideally a square-ish
crop for the circular frame.

## Add your LinkedIn

In `index.html`, find the Contact section link with
`href="https://www.linkedin.com/in/YOUR-LINKEDIN"` and replace `YOUR-LINKEDIN`
with your profile handle. You can then delete the `— add your URL` note next to it.

## Deploy (so clients can see a live URL)

### Option A — GitHub Pages (free)

1. Create a public repo (e.g. `portfolio`) on GitHub and push this folder.
2. Repo **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`, then **Save**.
4. Your site goes live at `https://<your-username>.github.io/portfolio/`.

### Option B — Netlify (drag & drop, no CLI)

1. Go to <https://app.netlify.com/drop>.
2. Drag this whole folder onto the page. Done — you get an instant live URL.

### Option C — Vercel

1. Push to GitHub, then import the repo at <https://vercel.com/new>.
2. Framework preset: **Other** (it's static). Deploy.

The only external dependency is Google Fonts, which loads fine on all of the
above.
