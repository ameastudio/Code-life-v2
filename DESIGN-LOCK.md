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

## Sequential checkpoint unlocking — approved (2026-10-02)
Players must **complete their current lesson before the next Code City checkpoint unlocks**. No skipping ahead on the map. Previously completed lessons remain accessible for review.

## Personalized pet marker movement — approved (2026-10-02)
- The player's **one chosen Code Pet** hovers immediately **above the current numbered Code City checkpoint**, acting as their map marker.
- Upon successfully completing that checkpoint's lesson, the pet **moves to hover above the next newly unlocked checkpoint**. The move should look animated, not an instant pet swap/teleport, while keeping all checkpoints aligned with the illustrated road.
- Previous checkpoints remain blue with glowing cyan checkmarks; pet follows the active checkpoint as progression advances.

## End-of-district celebration — approved (2026-10-02)
Completing the final lesson/challenge in any Code City district triggers a **big celebration with the player's chosen Code Pet**, before they continue into the seamlessly connected next district. The pet remains the player's chosen character and then advances to the next unlocked checkpoint.

## District Boss Builds — approved (2026-10-02)
Each Code City district ends with a larger **Boss Build** project that requires using skills learned in that district. Passing the Boss Build triggers the previously approved big celebration with the player's chosen pet, then unlocks continued progression to the next district. For Web Foundations, retain the earlier plan for HTML, CSS, and JavaScript Boss Builds to develop **the same growing interactive website** rather than three unrelated projects.

## Boss Build rewards — approved (2026-10-02)
Completing each district's Boss Build awards **bonus XP**, **bonus Code Coins**, and **exclusive pet accessories** for the player's chosen Code Pet, in addition to the approved end-of-town celebration. Rewards must be earned from learning/project completion rather than used to purchase level progression.

## Lesson hearts — approved (2026-10-02)
Lessons use a **three-heart system**. The user selected three hearts instead of unlimited retries. Exact heart deduction, refill and recovery behavior will be specified separately; do not assume or invent it.

## Blue hearts recovery — assistant-selected per Bri's request (2026-10-02)
- Display **three BLUE hearts** (not red) for lesson attempts.
- Wrong answers cost one heart; a successful review exercise can restore one blue heart (maximum three).
- Hearts also regenerate automatically: **one heart every 20 minutes** until full, so learners never get stuck permanently.
- When hearts run out, offer review exercises to earn them back while new lessons pause. The player can still review completed material; do not charge coins for hearts or gate learning behind purchases.

## Incorrect-answer behavior — approved (2026-10-02)
When a learner answers incorrectly, their **chosen Code Pet gives a helpful hint** and offers another attempt rather than immediately revealing the answer. Maintain the previously approved three-blue-heart system.

## Progressive, SideMe-style lessons — approved (2026-10-02)
- Model the **learning progression** on the short, step-by-step style Bri calls "SideMe": teach one small idea per screen, then guided micro-practice, independent practice, and a short end-of-lesson quiz. Increase difficulty gradually, building on what was learned in earlier lessons rather than jumping into an advanced task.
- Provide **instant feedback**, chosen-pet reactions and helpful hints on mistakes (do not immediately reveal answers), with a maximum of three blue hearts and the separately approved heart-recovery policy.
- Revisit previously taught material via spaced quick reviews and interleave it into future exercises; advance when the learner demonstrates understanding.
- Match Bri's **already approved lesson, quick-review and completion screenshots exactly**. Do not replace the screenshot layout with a generic quiz UI; progression concerns lesson behavior, not permission to redesign.

## Lesson quiz progression gate — approved (2026-10-02)
A learner must **pass the short end-of-lesson quiz before the next Code City lesson checkpoint unlocks**. Failed attempts do not advance progression; use the approved chosen-pet hints and three-blue-heart rules. Passing threshold: **80%**. Missed quiz concepts receive a brief correction/review so errors are not simply skipped.

## Daily lesson limit — approved (2026-10-02)
Limit learners to **4 new lessons per day**. After reaching the daily limit, users can still revisit completed lessons, do quick reviews, practice in Playground, and work on available projects without being locked out of the app. New-lesson count resets at the start of the next local day. Preserve the approved lesson-screen designs.

## Daily completion reward — approved (2026-10-02)
Completing all **4 new daily lessons** awards a bonus of **XP and Code Coins**. This is a reward for learning, not a requirement for reviewing or using Playground. Exact reward quantities will be set during implementation.

## Daily streak and milestone rewards — approved (2026-10-02)
Add a **daily learning streak** with the previously approved **blue cyber-flame icon**. Award milestone rewards for streak achievements. Exact streak qualifying activity, milestone schedule and streak-freeze rules will be decided separately. Keep the visual styling aligned with Bri's approved screenshots.

## Meaningful revision maintains streak — assistant-selected per Bri's request (2026-10-02)
YES: Successfully completing **at least one real revision exercise** counts as learning activity toward maintaining the daily streak, even if the learner does not complete a new lesson that day. Completing a new lesson also qualifies. Simply opening the app or tapping around does not qualify. This lets learners keep their streak on review-focused days. Distinguish this streak activity from the separate bonus for finishing all four new daily lessons.

## Coin-purchased Streak Freezes — approved (2026-10-02)
Players may spend **earned Code Coins** to buy **Streak Freezes**, protecting a daily learning streak if they miss a day. Freezes are a convenience/reward, never required to access lessons or reviews. Exact coin cost, inventory limit and automatic/manual activation can be decided during implementation.

## Streak Freeze shop location — approved (2026-10-02)
Streak Freezes are **purchased with earned Code Coins in the in-app Shop**. Keep purchase separate from the question of when a bought freeze activates; activation behavior is not yet approved.

## Streak Freeze automatic activation — assistant-selected per Bri's request (2026-10-02)
Purchased Streak Freezes are stored in the player's Shop inventory. If the player misses a day of qualifying learning activity, **one owned Streak Freeze activates automatically**, protecting the streak for that missed day, and its inventory count decreases by one. Clearly tell the player that their freeze was used on their next visit. A freeze does not generate lesson-completion rewards or count as a completed lesson.

## Pet Shop outfit XP bonuses — approved (2026-10-02)
Pet Shop outfits and accessories can provide **small XP bonuses** when equipped, in addition to changing the pet's appearance. XP is still earned by actually completing learning activities; outfitting the pet cannot unlock lessons, bypass quizzes, or earn passive progression by itself. Exact bonus values and stacking rules to be set during implementation.

## Pet Shop coins only — approved (2026-10-02)
Pet Shop outfits and accessories are purchased using **earned Code Coins only**. Do not add real-money purchases for these items. Equipped outfits/accessories may grant the previously approved small XP bonuses, but do not provide passive XP or bypass lessons.
