# Password Strength Checker

A browser-based tool that checks password length, complexity and uniqueness, suggests stronger alternatives, and prevents reuse of old passwords.

**Live demo:** https://YOUR-USERNAME.github.io/password-strength-checker/

## Features
- Length, character-variety and entropy-based strength meter
- Detects common passwords, repeated characters and sequences
- Generates strong random passwords and passphrases (`crypto.getRandomValues`)
- Reuse prevention: saved passwords are stored only as SHA-256 hashes in `localStorage`
- 100% client-side, no data leaves the browser

## Concepts learned
- Entropy: `bits = length × log2(character pool size)`
- Hashing (SHA-256) vs storing plain text
- Cryptographically secure randomness vs `Math.random()`

## Run locally
Pick any one:

1. **Simplest:** double-click `index.html`. (Saving to history needs a secure page, so use option 2 or 3 for that feature.)
2. **Python:** `python -m http.server 8080`, then open http://localhost:8080
3. **Node.js:** `npm start`, then open http://localhost:8080

## Create your own live website (fork and deploy)
1. Click **Fork** at the top of this repo.
2. In your fork go to **Settings → Pages** and set **Source** to **GitHub Actions**.
3. Go to the **Actions** tab, enable workflows if asked, and run **Deploy website to GitHub Pages**.
4. Your site goes live at `https://YOUR-USERNAME.github.io/password-strength-checker/`.

After that, every push to `main` redeploys the site automatically.

## Tech
HTML, CSS, vanilla JavaScript, Web Crypto API
