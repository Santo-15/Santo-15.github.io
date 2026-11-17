# Santosh Kukna · Portfolio

A static site: one `index.html` plus an `assets/` folder. No build step and no framework.
Layout and style follow the open-source [Magic UI portfolio](https://github.com/dillionverma/portfolio) by Dillion Verma.

```
index.html                       the whole page (HTML, CSS and JS inline)
assets/Santosh-Kukna-Resume.pdf  résumé linked from the page and the dock
assets/logos/                    TransOrg, CloudDefense and IIT Roorkee logos
assets/rca/rca-agent-demo.mp4    RCA demo video (opens from the project card)
assets/rca/ui-solved.png         RCA screenshot (card image and link-preview image)
```

## Add your photo

Save a square photo as `assets/photo.jpg`. It replaces the "SK" initials automatically.

## Preview locally

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Publish free on GitHub Pages

1. On GitHub, create a new **public** repository named exactly `Santo-15.github.io`.
2. Push this folder to it:

```bash
git init
git add index.html README.md assets
git commit -m "Portfolio"
git branch -M main
git remote add origin https://github.com/Santo-15/Santo-15.github.io.git
git push -u origin main
```

3. In the repository, open **Settings > Pages**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute or two the site is live at **https://santo-15.github.io**.

If you host it somewhere else, update the `og:url` and `og:image` lines in `index.html` so LinkedIn shows the right preview.
