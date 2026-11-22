# Habit Tracker – website

The small website for **Habit Tracker: Daily Streaks**, the Android app by Horyaal Tech.

- `index.html` – home page
- `privacy.html` – privacy policy (this is the link for Google Play Console)
- `styles.css` – shared styles (light and dark mode)
- `icon.svg`, `icon-180.png` – app icon / favicon
- `CNAME` – the site's own domain (habittracker.horyaaltech.com); keep this file

Plain HTML and CSS: no frameworks, no build step, no JavaScript, no analytics, no cookies, nothing loaded from other
websites.

## Turn on GitHub Pages (once)

1. Open this repository on GitHub → **Settings** → **Pages** (left menu).
2. Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
3. Under **Branch**, choose **main** and the folder **/ (root)**, then **Save**.
4. Wait 1–2 minutes. The page shows "Your site is live at …".

## Own domain: habittracker.horyaaltech.com

The `CNAME` file in this folder tells GitHub Pages to use **habittracker.horyaaltech.com**. The domain also needs one
DNS record where horyaaltech.com is managed:

| Type | Host | Value |
|---|---|---|
| CNAME | `habittracker` | `sicidsanka.github.io` |

Then in **Settings → Pages**, check that **Custom domain** shows `habittracker.horyaaltech.com` (DNS check
successful) and tick **Enforce HTTPS** once GitHub offers it (it can take up to an hour for the certificate).

The addresses are then:

- Home page: https://habittracker.horyaaltech.com/
- Privacy policy: https://habittracker.horyaaltech.com/privacy.html

(The old address https://sicidsanka.github.io/Habit_tracker-site/ redirects there.)

Paste the privacy policy address in Play Console → **App content** → **Privacy policy**.

## After the app is on Google Play

In `index.html`, replace the `href="#"` of the "Get it on Google Play" button (marked `PLAY STORE LINK`) with the
app's Play Store address, commit, and Pages updates by itself.
