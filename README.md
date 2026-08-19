# Humpty Dumpty Kidz School — Site Concept

A single-page static site redesign concept for Humpty Dumpty Kidz School (Durgapur, WB), inspired by the editorial layout of EtonHouse's pre-school pages, rebuilt around the school's own brick-wall namesake and logo.

## Structure

```
.
├── index.html        # the entire site (self-contained HTML/CSS/JS)
├── assets/
│   ├── logo.png       # school logo (header + footer)
│   └── president.jpg  # founder & chairman photo (President's message section)
├── render.yaml        # Render Blueprint for one-click static deploy
└── .gitignore
```

No build step, no dependencies — it's plain HTML/CSS/JS.

## Run locally

Open `index.html` directly in a browser, or serve it:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Deploy to Render

**Option A — Blueprint (uses `render.yaml`):**
1. Push this repo to GitHub.
2. In the Render dashboard, click **New +** → **Blueprint**, and select this repo.
3. Render reads `render.yaml` and provisions a Static Site automatically. Click **Apply**.

**Option B — Manual static site:**
1. In the Render dashboard, click **New +** → **Static Site**, and select this repo.
2. Build Command: leave blank
3. Publish Directory: `.`
4. Click **Create Static Site**.

Every push to the connected branch redeploys automatically.

## Content notes

- Contact/address details are pulled from the real school listing.
- Branch cards beyond the Benachity flagship, and the teacher-student ratios in the FAQ, are placeholders — swap in real figures before treating this as production copy.
