# Code Life v2 — Current implementation status

Updated: 2026-10-02

## Step 1: Entry screen
- Implemented `index.html` with Bri's **exact approved second screenshot** (the official blue </> app icon, Code Life white/cyan wordmark, original Pixel Pup, neon skyline and Get Started art).
- The screenshot itself is the displayed artwork; it is **not** replaced with a CSS recreation. A real accessible HTML button is positioned over Get Started.
- Tapping Get Started shows Bri's **exact approved third screenshot** (coding level selection) as an image only. The choices on that next screen have **not** yet been coded; do not claim onboarding is complete.
- `manifest.webmanifest` references the official icon **cropped from the approved screenshot**.
- The entry artwork, level reference and icon files exist in Bri's generated `Code-Life-v2-Entry-ASSETS-ONLY.zip` package but still **need to be uploaded by Bri to the repository**. Expected paths:
  - `assets/entry-approved.webp`
  - `assets/level-approved.webp`
  - `icons/icon-192.png`
  - `icons/icon-512.png`
- Do not use other generated mascot art, logo variants or stock scenery as a fallback. If these binary assets are missing from GitHub, report that they need uploading rather than visually substituting something.
- The local rendering and Get Started route were tested in a phone-sized simulated browser, without JS errors. Once the assets are uploaded, verify GitHub Pages separately.

## Next
1. Wait for Bri to upload the assets/images and verify her GitHub Pages URL.
2. Implement **Choose Your Coding Level** interactions from the third approved screenshot, keeping that screenshot's design; keep all other approved screenshots locked per `DESIGN-LOCK.md`.
3. Preserve the previously approved scrolling Code City behavior; build that later as a separate phase.

## Asset upload verified (2026-10-02)
Bri uploaded all four files to the repository ROOT rather than the requested folders. Correct uploaded paths: `entry-approved.webp`, `level-approved.webp`, `icon-192.png`, `icon-512.png`. `index.html` and `manifest.webmanifest` have been updated to use these exact root paths, so no additional file upload is necessary. GitHub Pages publication has not yet been confirmed on a browser; user should visit site or turn on Pages via Settings > Pages > Deploy from a branch, `main`, `/(root)`.

## Step 2: Choose Your Coding Level implemented (2026-10-02)
- The APPROVED `level-approved.webp` screenshot is displayed directly; no graphic replacements.
- Three real invisible accessibility-labeled buttons placed precisely over Beginner, Intermediate and Advanced screenshot cards. Beginner initially selected; users may change selection, with a cyan focus/selection ring.
- Continue saves the chosen level to `localStorage` (`code-life-v2:onboarding:level`) and confirms the save on the same screen. Saved choice is restored upon reopening; tapping the top-left area returns to the original entry screen.
- The next learner identity screen is not yet built. **Continue does not navigate to it yet**, so do not claim full onboarding is finished.
- Verified all artwork file paths are present in the GitHub repository. Local JavaScript logic tests for exclusive choice, persistence, back and image selection passed; browser-based mobile validation was blocked by test environment policy, so user must check the live app.
