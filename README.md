# Sajal Nauman — Portfolio

A single-page portfolio: sage-green theme, a draggable 3D cube in the hero (her photo on one face), two smaller 3D accents (a skills cube and a spinning medal coin), a 4-project slider with real schematics and build photos, a scroll-spy side nav, and an achievements list with medal photos. Pure HTML/CSS/JS — no build step, no dependencies.

## Structure
```
index.html
assets/
  photo.jpg
  medal-1040.jpg, medal-ssc.jpg, medal-hssc.jpg, medal-bronze.jpg
  proj-smps-charger.jpg, proj-5v-supply.jpg, proj-dice-breadboard.jpg
  proj-elevator.jpg, proj-dtmf.jpg, proj-voice.jpg, proj-eq-filter.jpg,
  proj-airport-system.jpg, proj-tictactoe.jpg
vercel.json
.gitignore
```

## Deploy: GitHub → Vercel (recommended, since you'll push to GitHub first)

1. From this folder, make it a repo and commit:
   ```
   git init
   git add -A
   git commit -m "Initial commit"
   git branch -M main
   ```
2. Create a new empty repo on GitHub, then:
   ```
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
3. Go to vercel.com/new, import that GitHub repo, and deploy. No framework preset or build command needed — it's a static site. Every future push to `main` auto-redeploys.

## Alternative: Vercel CLI directly
```
npm i -g vercel
cd sajal-portfolio
vercel
```
Accept the defaults when prompted.

## Editing
Everything lives in `index.html` — content, styles, and the small amount of JS (welcome screen, nav, cube drag, slider, scroll-spy, counters) are all inline. To swap a photo, replace the matching file in `assets/` and keep the same filename.
