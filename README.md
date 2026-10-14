# Zeus Tenerife — Portfolio

Personal portfolio site: Virtual Assistant · Customer & Technical Support.
Live at **https://zakura1x.github.io/**

Plain HTML/CSS/JS, no build step. GitHub Pages serves the `main` branch as-is.

```
index.html    all content (edit text here)
styles.css    colors (top of file, :root), layout, responsive rules
script.js     mobile menu, active nav link, scroll reveal
favicon.svg   "ZT" icon
```

## Common edits

- **Profile photo:** add `assets/profile.jpg` (square, ~600×600), then in `index.html` replace
  `<div class="avatar avatar-monogram">ZT</div>` with
  `<img class="avatar" src="assets/profile.jpg" alt="Zeus Tenerife">`.
- **Download CV button:** add a public CV (no phone number) as `assets/Zeus-Tenerife-CV.pdf` and add
  `<a class="btn btn-ghost" href="assets/Zeus-Tenerife-CV.pdf" download>Download My CV</a>` inside `.hero-cta`.
- **Add a project:** copy one `<article class="card project">…</article>` block in the Portfolio section and edit it.
  Label classes: `label-pro`, `label-personal`, `label-academic`. Mock header variants: `mock-chat`, `mock-table`,
  `mock-compare`, `mock-docs`, `mock-phone`, `mock-quiz`. To use a real (sanitized) screenshot, replace the
  `<div class="mock …">` with `<img src="assets/your-image.webp" alt="…" style="height:170px;object-fit:cover">`.
- **Experience / skills / services:** edit the matching section in `index.html`; every entry is a plain list item.
- **Colors:** change the variables in `:root` in `styles.css`.

## Preview locally

```bash
python -m http.server 5500
```

Then open http://localhost:5500.

## Deploy an update

```bash
git add -A
git commit -m "Update portfolio"
git push
```

GitHub Pages republishes automatically within a minute or two (check the repo's **Actions** tab for the
"pages build and deployment" run).

Never commit CVs with phone numbers, credentials, or screenshots from employer/client systems.
