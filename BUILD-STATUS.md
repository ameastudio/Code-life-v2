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

## Step 3: learner identity selector coded (2026-10-02)
- Uses Bri's exact approved screenshot supplied as image #4 in her 2026-10-02 reference collection. The original image was converted to **pixel-identical lossless WebP** named `identity-approved.webp` at the original 941×1672 resolution.
- Real, separately tappable areas are aligned with the four image cards: Student, Self-taught learner, Career switcher, and Professional. Selection gets a cyan highlight and persists on device under `code-life-v2:onboarding:identity` after Continue.
- Screen 2's Continue now saves coding level and navigates to Screen 3 (`#/identity`); Screen 3's top-left back hotspot returns to Screen 2. Entry screen and second-n lettering repair remain unchanged.
- **BINARY ARTWORK UPLOAD IS STILL REQUIRED**: Bri must unzip `Code-Life-v2-Screen3-UPLOAD-THIS.zip` and upload its single `identity-approved.webp` file into the repository ROOT. Code was committed separately using the GitHub connector. Until this file is present, Screen 3 cannot display.
- Screen 3's Continue confirms and saves the selection but intentionally does not navigate further: Screen 4's exact approved pet chooser and controls will be coded separately.

## Step 4: Choose Your Code Pet — CODE COMPLETE, ART UPLOAD PENDING (2026-10-02)
- Screen uses Bri's **exact reference image #5**, converted from original 941×1672 PNG into pixel-identical lossless WebP (`pet-chooser-approved.webp`, pixel equality tested).
- All SIX named approved pets have accessible clickable card hotspots at their original visual locations. Selected pet stored on device under `code-life-v2:onboarding:pet`. Existing Pixel Pup artwork is the default selection; other choices get a dynamic cyan selection indicator. The original static Pixel Pup check badge gets covered only when a different pet is selected to avoid conflicting checked state.
- Screen 3's Continue now persists learner identity and navigates to `#/pet-choice`. Screen 4's back button returns to Screen 3. Screen 4 Start Journey saves the chosen Code Pet and confirms with a temporary message.
- **Required before viewing**: Bri must unzip `Code-Life-v2-Screen4-UPLOAD-THIS.zip`, upload only `pet-chooser-approved.webp` to the repository ROOT and commit. GitHub connector wrote the text code but did not upload the binary image.
- **Code City is NOT implemented yet**; Screen 4 does not open an unapproved placeholder.
- Existing corrected 'Beginner' lettering overlay remains present and is displayed only on the coding level screen.
- Checked GitHub source: one JavaScript block parsed without syntax errors, exactly six pet hotspots, correct navigation and localStorage wiring. User testing on deployed app remains necessary.

## Code City first functional build — single-upload package ready
A tested local Code City build has been prepared as ONE flat 11-file bundle: `Code-Life-v2-ONE-UPLOAD-Code-City.zip`. It contains `code-city.css`, `code-city.js`, `curriculum.js`, `city-road.webp`, `pet-chooser-neutral.webp`, and SIX `pet-map-*.png` exact-approved-character assets. All files belong in the repo ROOT; no subfolders.

GitHub `index.html` is ALREADY connected to load `code-city.css`, `curriculum.js` and `code-city.js` and route Beginner onboarding into Code City. It retains existing 4 approved onboarding screenshots, back buttons, official no-Saturn Code Life wordmark on map, and corrected Beginner lettering. The approved Pixel Pup neutral card art is switched dynamically on selection of other pets.

**The 11 asset/source files in the ZIP have NOT yet been uploaded to GitHub.** Before user uploads the ZIP contents, no claim that Code City is deployed. The original entry/onboarding experience continues to work; clicking Start Journey shows a pending-upload notice if `window.CodeCity` isn't available. Do not attempt additional manual GitHub file-by-file uploads: Bri wants ONE upload.

**Verified locally in a simulated 390px mobile browser:** 27 actual HTML/CSS/JS checkpoint levels (8 lessons + Boss Build per town), 5 district roadside signs, 3 bigger Boss pads, single chosen current pet, upward resume scroll, locked hints, navigation icons; first HTML lesson code validation + end quiz + XP/coins + next checkpoint unlock; no uncaught JS errors. The neutral pet artwork changes only the top-left Pixel Pup tile in the original approved chooser, and a full-body Pixel Pup marker is extracted from the approved six-pet screenshot. ZIP integrity/flat filename paths verified. No new pictures were generated.

**Not finished:** unique high-detail architecture for each future district (currently modest recolored static accents on same blue road reference), Python Lab/Data Vault lesson content (their scenery is visible, but no invented pads/lesson counts), fully pixel-matched lesson screen styling, full rigged pet movement/evolution skins, Intermediate/Advanced placement assessment (onboarding properly gates advanced learners to prevent skipping that decision), the other approved nav screens and monetization. Saved data is local to device. Phone-specific visual check remains pending Bri's return.
