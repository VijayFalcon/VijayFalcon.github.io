# vijayfalcon.github.io

Personal portfolio website for Vijay Aravindh Srinivasan — AI/ML Engineer and BTech CSE (AI & ML) student at VIT Chennai.

Live at: **[vijayfalcon.github.io](https://vijayfalcon.github.io)**

---

## What's in it

**Hero** — name, tagline, and quick-links to projects, LinkedIn, and GitHub.

**About** — bio, focus areas, and contact details.

**Skills** — tech stack across six categories (AI/LLM Engineering, Machine Learning, Full-Stack, Data & Infrastructure, Languages, Other) with animated proficiency bars.

**Projects** — MEDIQA-CORE (TumorClassifier) as a hardcoded featured card with architecture breakdown, plus all other public repos pulled live from the GitHub API and sorted by last updated. Adding a new repo and giving it a description is all it takes for it to appear here automatically.

**Experience** — timeline of education, internship, and club roles.

**Contact** — email, LinkedIn, GitHub.

---

## Stack

Pure HTML, CSS, and vanilla JavaScript. No framework, no build step, no dependencies. One file.

- Google Fonts (Syne + DM Mono)
- GitHub REST API (`/users/VijayFalcon/repos`) for live project cards
- GitHub Pages for hosting

---

## Repo structure

```
VijayFalcon.github.io/
├── index.html      # The entire site
├── profile.jpg     # Profile photo used in the About section
└── README.md
```

---

## Updating content

**Bio / skills / experience / contact** -- edit directly in `index.html` and push to `main`.

**Projects** -- update the Description field on any GitHub repo (gear icon next to About on the repo page). The portfolio reads it live on every page load.

**Featured project (MEDIQA-CORE)** -- hardcoded in the `<!-- Featured -->` block inside `index.html` since it has a custom architecture panel. Update it there directly.

**Profile photo** -- replace `profile.jpg` in the repo root with a new image of the same name.

---

## Local development

No install needed. Just run a local server from the repo folder:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`. The GitHub API fetch requires a real HTTP origin -- opening `index.html` directly as a `file://` URL will cause the projects section to fail to load.
