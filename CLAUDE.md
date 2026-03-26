# easygains-website

Marketing site for the EasyGains iOS app. Deployed to GitHub Pages at **easygains.app** via Namecheap DNS.

## Repo & Deployment
- GitHub Pages repo — push to `main` to deploy
- Custom domain: `easygains.app` (CNAME file present, Namecheap DNS pointed to GitHub)
- HTTPS cert: provisioned via GitHub Pages (may take up to 24h after DNS changes)
- No build step — pure HTML/CSS/JS, single `index.html` + `styles.css`

## Design
- Dark theme matching the app: background `#1C1C1E`, cards `#2C2C2E`
- Font: Space Grotesk (Google Fonts)
- Accent colors: amber `#FF9500`, purple `#AF52DE`, green `#34C759`
- Logo: inline SVG dumbbell in nav (white on dark)
- App Store button: `href="#"` — **update this to the real App Store URL once the app is live**

## Structure (index.html)
1. **Nav** — logo + "Download" button linking to `#download`
2. **Hero** — tagline "Eat your protein. Move your body. Don't overthink the rest." + CTA
3. **Screenshots** — 3 phone mockups (home, voice, weekly), clickable to feature. Uses `setFeatured()` JS function. Featured phone scales up with spring animation.
4. **Features** — 3 cards: Voice-first, Weekly view, Workouts
5. **Pricing** — Free ($0) vs Pro ($6.99/mo), Pro card has amber border
6. **Download** — CTA section with App Store button
7. **Support** — 4 FAQ items + contact email `everyone@whimsyxm.com`
8. **Footer** — © 2026 EasyGains, links to XtraMedium

## Assets
- `assets/screenshots/home.png` — home screen (macro rings)
- `assets/screenshots/voice.png` — voice input screen
- `assets/screenshots/weekly.png` — weekly analytics view
- `assets/icon.png` — app icon (white dumbbell on black)
- `assets/favicon.png` — favicon

## Key Details
- Pricing: **$6.99/mo** (no annual plan shown on site yet)
- Support email: `everyone@whimsyxm.com`
- Company footer: XtraMedium (links to extramediumal.github.io)
- App description: voice-first macro tracker, protein is the hero metric

## TODO Before App Store Launch
- Replace `href="#"` on all App Store buttons with the real App Store URL
- Consider adding privacy policy page (Apple requires one for apps with subscriptions)
