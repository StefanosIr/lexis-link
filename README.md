# Lexis — Download Link & Social Assets

Smart "get the app" link and launch graphics for **Lexis**, a word puzzle game for iOS and Android.

**Live link:** https://stefanosir.github.io/lexis-link/

Visiting the link automatically sends each visitor to the right store:

| Device | Goes to |
| --- | --- |
| iPhone / iPad | App Store |
| Android | Google Play |
| Desktop / other | A page with both store buttons |

## Store links

- **App Store:** https://apps.apple.com/us/app/lexis-word-puzzle-game/id6762004245
- **Google Play:** https://play.google.com/store/apps/details?id=com.stefanosirodotou.lexis

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The smart-redirect landing page (device detection + fallback buttons). |
| `icon.png` | Lexis app icon, shown on the landing page. |
| `lexis_social_1080.png` | 1080×1080 social post with official App Store / Google Play badges. |

## How the redirect works

`index.html` reads the browser's user-agent and calls `location.replace()` to the
matching store. If neither iOS nor Android is detected, the page stays put and shows
both store buttons as a fallback. No tracking, no dependencies, no build step — one
static file.

## Updating

1. Edit `index.html` (or regenerate the social image from the app repo's
   `social/make_social.py`).
2. Commit and push to `main`.
3. GitHub Pages redeploys automatically within a minute.

## Using the link

- **Instagram / TikTok bio** → set the bio link to the live URL.
- **Stories** → add a Link sticker pointing to the live URL.
- **Facebook / X / LinkedIn** → paste the URL in the caption.
- **Post the image** → `lexis_social_1080.png`.

## Trademarks

The **App Store** badge and Apple logo are trademarks of Apple Inc. The **Google Play**
badge and logo are trademarks of Google LLC. They are used here only to link to the
respective app listings, in line with each company's marketing guidelines.

---

See [LICENSE](LICENSE) for copyright terms.
