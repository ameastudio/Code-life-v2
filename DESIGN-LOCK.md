# Code Life v2 — Approved Brand and Entry Screen

Status: **APPROVED AND LOCKED** by Bri on 2026-10-02. No redesign without explicit approval.

## Official logo and app icon
Use the **second reference image from Bri's 2026-10-02 screenshot collection** (the portrait entry/splash screen) as the EXACT visual reference:
- **Icon:** glossy, slightly 3D electric-blue rounded square with a bright cyan rim and centered white `</>` code symbol. This is the official app icon, not a pixel cross, orbit emblem, star, or cat icon.
- **Wordmark:** `Code Life`, with "Code" white and "Life" bright cyan-blue, matching that same image.
- This logo/wordmark is our official brand system for Code-Life-v2. Do not substitute other generated logo designs.

## Approved entry / splash screen — EXACT reference
Use that **second portrait screenshot** as the visual specification:
- Electric/deep blue futuristic skyline with elevated circular platforms, clouds and luminous sci-fi details.
- Large official blue-square `</>` icon near the upper center, then Code Life wordmark.
- Tagline: **"Where codes come to life."**
- Original **Pixel Pup** (blue/white fluffy puppy, huge cyan-blue eyes, distinctive blue checkerboard floppy ears and fluffy tail, `</>` tag/collar), full body including ears, all paws and tail, large and centered in foreground.
- Small line **"Learn. Build. Grow."** over bottom button.
- Glowing cyan/blue pill **"Get Started"** button near bottom.
- Preserve layout, colors, exact character styling, composition and proportions when converting this image to the implemented app. Do not substitute another dog, theme or logo.
- Keep UI button as a REAL clickable interface element matching the artwork; do not make an image's baked button the only control. Onboarding must function.

## Engineering / approval rule
Screens should match Bri's approved screenshots as closely as technically feasible across mobile devices. Any responsive deviations or needed asset splitting should be called out before changing visual decisions. Implement one approved screen at a time, then let Bri verify before continuing.

## Other reference images
Bri supplied additional approved references on 2026-10-02 for Code City (floating road and stone checkpoints), onboarding choices, six original pets, courses, Playground, My Pet, lessons, reviews and celebrations. Verify each separately screen-by-screen before treating it as locked. Do not assume similarly-themed later generated images supersede these references.

## ALL USER-SUPPLIED SCREENSHOTS LOCKED (2026-10-02)
Bri explicitly approved **EVERY screenshot she uploaded together in the 2026-10-02 chat** and requests **everything EXACTLY as pictured, with no changes**. These uploaded images—not any later generated replacements, placeholder stock imagery, or vague verbal summaries—are the visual source of truth. They include:
1. Code City floating-blue-road screenshot, header, numbered illuminated checkpoints, district landmark, current pet, bottom navigation.
2. Entry/splash screenshot: official blue-square </> logo and app icon, Code Life wordmark, exact original Pixel Pup, city background and Get Started button (already individually locked above).
3. Coding-level selection screenshot (Beginner / Intermediate / Advanced; Pixel Pup).
4. Learner identity selection screenshot (Student / Self-taught learner / Career switcher / Professional; Pixel Pup).
5. Six-pet chooser screenshot: Pixel Pup, Byte Cat, Nova Owl, Loop Fox, Chip Bunny, Glitch Dino, robot guide.
6. Additional learner-identity visual screenshot. Preserve as provided; when two screenshots depict the same screen differently, ask Bri which screenshot to use at implementation time rather than silently picking or merging.
7. Code City district/Courses montage: HTML Town, CSS District, JavaScript City, Python Lab, Data Vault; Courses list, module breakdown, lesson selection.
8. Playground screenshot with code editor, live preview, helper pet, controls, skyline, navbar.
9. My Pet screenshot with futuristic cyber bedroom, pet, room options and evolution.
10. Lesson: Headings screenshot with companion, teaching content, code exercise, preview, quick symbols, check button.
11. Quick Review screenshot with exercise/preview/hint/check UI.
12. Level Complete screenshot with celebration, rewards, pet-bond progression.

### NON-NEGOTIABLE IMPLEMENTATION RULE
- **Do not generate or replace any user-approved imagery**, logo, mascot, scenery, labels, UI placement, or theme with approximations. Do not reimagine these images. Build matching functional screens from the screenshots.
- **Separate interactable UI from background images** while preserving the exact screenshot appearance. A screenshot itself is not functional; use approved artwork assets for backgrounds/elements, wire real inputs/buttons, and verify on the target phone-size viewport. If necessary artwork exists only embedded in the screenshot, extract/crop/reconstruct for functional pieces without inventing new design. Alert Bri if exact visual fidelity cannot be guaranteed rather than claim otherwise.
- Do not add/remove onboarding steps, new features, alternate mascots or layout modifications without explicit user approval. Review duplicated/contradictory references only when the specific screen is being implemented.
- User wants a screen-by-screen rebuild but **does NOT want to approve each already-approved screenshot again**. Ask only essential implementation questions.

## Code City scrolling world — approved (2026-10-02)
- A **single vertically scrolling, continuous Candy Crush-like road**, in a gently top-down/flat-lay game-map view. NOT a single overview showing every level at once.
- Phone viewport shows approximately **3–5 numbered checkpoint stones at a time**; user scrolls to see subsequent levels.
- **Seamless visual district transitions while scrolling**, with NO separate district pages or loading screens.
- Exact district progression: **HTML Town → CSS District → JavaScript City → Python Lab → Data Vault**.
- Each district gets its own approved architectural palette, signage, landscape and theme, while the road remains continuous. The approved illustrated screenshots remain reference; the one-image overview generated afterward is a CONCEPT MAP ONLY, not the in-app viewport or final art.
- Match checkpoint coordinates and the depicted road precisely; checkpoints must be located ON the road, rather than added as a disconnected CSS overlay.

## Code City checkpoint interaction — approved
Tapping an unlocked numbered checkpoint on the continuous Code City road **opens its lesson directly**, with no intermediate preview card and no second Start button. Checkpoints are themselves interactive and remain correctly aligned with the illustrated road. (Approved by Bri, 2026-10-02.)

## Code City checkpoint completion visuals — selected by assistant at Bri's request
- Completed checkpoints stay BLUE and show a glowing CYAN CHECKMARK.
- Current/unlocked next checkpoint glows brighter for navigation.
- Locked future checkpoints appear dimmed (remain consistent with the blue art style).
- GOLD is reserved for coins and special rewards; do not use all-gold completed stones.
