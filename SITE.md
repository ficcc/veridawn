# Veridawn website notes

The public site for the Veridawn app, served by GitHub Pages at **https://ficcc.github.io/veridawn/** from the root of `main`.

| File | What it is |
|---|---|
| `index.html` | Home: what the app does, the video, the Google Play link, privacy, support, feedback. The app's Settings → Support → Project page opens it. |
| `privacy.html` | The privacy policy. Its URL goes in Play Console → App content → Privacy policy. |
| `terms.html` | Terms of use: predictions are a guide, outdoor safety, tips, third-party data, no warranty. |
| `404.html` | Shown for any missing page. |
| `style.css` | Shared styles: charcoal and gold, light and dark. |
| `icon.png` | The Valley V icon (a copy of `docs/store/icon-512.png` in the app repo). |
| `banner.png` | The README banner (a copy of `docs/store/feature-graphic.png` in the app repo). |
| `video-poster.jpg` | The video's thumbnail, kept here so the page asks YouTube for nothing until play is pressed. |
| `README.md` | What people see on GitHub: the app, not the site. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

Contact address on every page: **veridawn.app@gmail.com**.

## Publish a change

1. Edit the `site/` folder in the app repo (`ficcc/goldenhour`), which is the source of truth.
2. Copy it here, push `main`, and check the live page after a minute or two.
3. If the privacy policy's address ever moves, update Play Console → App content → Privacy policy.

## Rules for this site

- **No external payment links** (Ko-fi, PayPal, Buy Me a Coffee…) on `index.html`. The app links to it, and Google Play's payments policy bars in-app links that lead to a payment method other than Play billing, indirect ones included. Tips stay in the app, through Google Play.
- **No links to the web app** from anything here, for the same reason: the web app has a tip link.
- **The video stays click-to-load**, so a visit to the home page sends nothing to YouTube, as the privacy policy says.
- Keep `privacy.html` in step with the app's in-app Privacy screen and `docs/privacy-policy.md` in the app repo. When either changes, change the date at the top.
- The terms are a plain-language starting point, not legal advice.
