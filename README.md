# adurage.github.io

Root site for `https://adurage.github.io/`.

- `index.html` – forwards visitors to Akuru Studio (`/akuru-studio/`).
- `.well-known/assetlinks.json` – proves to Android/Google Play that the Akuru Studio
  Android app (`io.github.adurage.akurustudio`) and this website belong together
  (Trusted Web Activity). Must stay at exactly this path.
- `.nojekyll` – needed so GitHub Pages publishes the `.well-known` folder.

## Updating assetlinks.json

Replace `REPLACE_WITH_SHA256_FROM_GOOGLE_PLAY_APP_SIGNING` with the SHA-256 fingerprint(s) from
Google Play Console ▸ your app ▸ Test and release ▸ App integrity ▸ App signing
(copy the ready-made "Digital Asset Links JSON" there). If you also install a locally built
APK for testing, add that key's SHA-256 too (PWABuilder's `signing-key-info.txt`).

Check: https://developers.google.com/digital-asset-links/tools/generator
