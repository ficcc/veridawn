# Veridawn website

The public site for the Veridawn app, served by GitHub Pages at **https://ficcc.github.io/veridawn/**.

| File | What it is |
|---|---|
| `index.html` | Home: what the app does, the Google Play link, privacy, support, feedback. The app's Settings → Support → Project page opens it. |
| `privacy.html` | The privacy policy. Its URL goes in Play Console → App content → Privacy policy. |
| `terms.html` | Terms of use: predictions are a guide, outdoor safety, tips, third-party data, no warranty. |
| `404.html` | Shown for any missing page. |
| `style.css` | Shared styles: charcoal and gold, light and dark. |
| `icon.png` | The Valley V icon (a copy of `docs/store/icon-512.png` in the app repo). |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

Contact address on every page: **veridawn.app@gmail.com**.

## Publish (once)

1. In this folder:

   ```bash
   git init -b main
   ```

   ```bash
   git add -A && git commit -m "Veridawn website"
   ```

   ```bash
   git remote add origin https://github.com/ficcc/veridawn.git
   ```

   ```bash
   git push -u origin main
   ```

2. On GitHub: **ficcc/veridawn → Settings → Pages → Build and deployment → Deploy from a branch → `main` / `/ (root)` → Save.**
3. After a minute or two, check:
   - https://ficcc.github.io/veridawn/
   - https://ficcc.github.io/veridawn/privacy.html
   - https://ficcc.github.io/veridawn/terms.html
4. In Play Console:
   - **App content → Privacy policy:** `https://ficcc.github.io/veridawn/privacy.html`
   - **Store settings → Store listing contact details:** email `veridawn.app@gmail.com`, website `https://ficcc.github.io/veridawn/`

## Rules for this site

- **No external payment links** (Ko-fi, PayPal, Buy Me a Coffee…) on `index.html`. The app links to it, and Google Play's payments policy bars in-app links that lead to a payment method other than Play billing, indirect ones included. Tips stay in the app, through Google Play.
- Keep `privacy.html` in step with the app's in-app Privacy screen and `docs/privacy-policy.md` in the app repo. When either changes, change the date at the top.
- The source of truth is the `site/` folder in the app repo (`ficcc/goldenhour`). Edit it there, then copy it here and push.
- The terms are a plain-language starting point, not legal advice.
