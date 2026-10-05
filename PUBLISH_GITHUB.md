# Publish this site on GitHub Pages

Recommended repository name:

`jeansebastienvayre-prog.github.io`

This makes the personal academic website available at:

`https://jeansebastienvayre-prog.github.io/`

MOVICI can remain at:

`https://jeansebastienvayre-prog.github.io/movici/`

## 1. Create the GitHub repository

On GitHub, create a new **public** repository named exactly:

`jeansebastienvayre-prog.github.io`

For the simplest first push, do not add a README, .gitignore, or license on GitHub at creation time, because those files already exist locally or can be added later.

## 2. Open the RStudio project

Open:

`JeanSebastienVayre_Website.Rproj`

Then open the **Terminal** tab in RStudio (not the R Console).

## 3. Initialise Git and upload the source

Run these commands one by one:

```bash
git init
git branch -M main
git add .
git commit -m "Initial personal academic website"
git remote add origin https://github.com/jeansebastienvayre-prog/jeansebastienvayre-prog.github.io.git
git push -u origin main
```

GitHub may ask you to authenticate in the browser.

## 4. Publish the Quarto site

Still in the RStudio Terminal, run:

```bash
quarto publish gh-pages
```

Confirm the requested publication when Quarto asks.

This creates/pushes a `gh-pages` branch containing the rendered website.

## 5. Important for this root user site

Because this repository is the special user-site repository `jeansebastienvayre-prog.github.io`, check:

**GitHub repository → Settings → Pages → Build and deployment**

Choose:

- Source: **Deploy from a branch**
- Branch: **gh-pages**
- Folder: **/(root)**

Save.

The website should then be served at:

`https://jeansebastienvayre-prog.github.io/`

## Updating the site later

After editing the `.qmd` files in RStudio:

```bash
git add .
git commit -m "Update website"
git push
quarto publish gh-pages
```

