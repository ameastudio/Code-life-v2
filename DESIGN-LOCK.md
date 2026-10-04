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

## Evolution-gated Pet Shop cosmetics — approved (2026-10-02)
Pet Shop outfits and accessories **unlock gradually as the player's chosen Code Pet evolves**. Unlocked items are then purchasable using earned Code Coins only, except exclusive items awarded for Boss Builds. Eligible equipped items may grant the previously approved small activity-based XP bonuses. Evolution milestones and specific unlock tables will be specified separately.

## Town-based pet evolution — approved (2026-10-02)
Chosen Code Pets **evolve by completing entire Code City towns**, not by accumulating general XP. Award the evolution at completion of that town's final Boss Build along with the existing pet celebration. Evolution adds tech-inspired/glowing upgrades and maintains the pet's original recognizable identity and approved design; pets do not age or change into unrelated creatures. New shop outfits and accessories unlock based on town-based evolution milestones.

## Pet bedroom customization — declined (2026-10-02)
Do **not** add purchasable bedroom customization or furniture decorating with coins. Keep the approved futuristic pet bedroom design intact. The Pet Shop may still sell previously approved pet outfits, accessories and Streak Freezes.

## Interactive pet reactions — approved (2026-10-02)
In the approved My Pet bedroom, **tapping the player's chosen pet triggers playful animated reactions**, including jumping, responding and playing/interacting with the player. Keep each original approved pet design recognizable and intact (no cropped ears, paws or tail). This is an interaction, not permission to redesign pets or the bedroom.

## Pet autonomous bedroom movement — approved in principle (2026-10-02)
The player's chosen Code Pet may **occasionally move naturally around its approved cyber bedroom on its own** (subtle walking, blinking, sitting or idle behaviors), while also reacting when tapped. Implement and visually verify a **proper, uncropped, full-body rig of the EXACT approved Pixel Pup first**; only then scale the same technique to the other five approved pets. Do not claim flawless motion before device testing, or merely translate the existing cropped static PNG as a substitute for full-body articulated animation. Keep bedroom artwork and original pet designs unchanged.

## Arcade — deferred by Bri (2026-10-02)
Do not decide or build arcade minigame types yet. Bri explicitly requested that arcade planning happen later. Keep the previously approved physical-controller arcade entry point in the pet bedroom design, but defer its gameplay and implementation until Bri chooses to revisit it.

## Code City main visual reference — confirmed by Bri (2026-10-03)
**Option A ONLY:** Use the **original futuristic BLUE floating highway screenshot** (first image in Bri's 2026-10-02 reference collection) as the principal, exact visual reference. Blue elevated winding road, floating islands, waterfalls, sky/clouds, high-tech district landmarks, and glowing numbered checkpoint stones. Maintain the separately approved continuous vertical Candy Crush-style scrolling map (3–5 checkpoints visible at once) through HTML Town → CSS District → JavaScript City → Python Lab → Data Vault. Other colorful town montage imagery is NOT the main style reference; districts must evolve within the original futuristic blue floating-highway design, not switch to a separate cartoon/village art style. Preserve the original screenshot's look and feel rather than reimagining it.

## Code City resume position — approved (2026-10-03)
When the player reopens Code Life, Code City **automatically scrolls to their currently unlocked checkpoint**, with their **chosen Code Pet hovering above that stone**. Resume without making players manually search the long continuous map. Preserve saved progress and the original futuristic blue floating-highway style.

## Auto-advance map camera — approved (2026-10-03)
After a learner completes a lesson, their chosen Code Pet animates to hover above the **next unlocked checkpoint**, and Code City's vertical map **automatically scrolls to follow the pet and center/bring the new checkpoint into view**. Do not require manual scrolling to find the next stone. Maintain a smooth scrolling transition consistent with the continuous floating-road map and respect reduced-motion accessibility settings.

## Visibility of future Code City checkpoints — assistant-selected at Bri's request (2026-10-03)
Keep **future locked level stones visible but softly dimmed along the continuous blue floating highway**, so players can see where they are headed. Use only a subtle cloud/mist veil over more distant, not-yet-reached town scenery for atmosphere; never hide nearby numbered checkpoints or obscure the winding road. The next active checkpoint remains brightly blue-glowing, while completed ones show their cyan checkmarks. Maintain the exact approved original floating-highway look.

## Revisiting earlier towns — assistant-selected at Bri's request (2026-10-03)
Players may **freely scroll backward** along the same continuous floating road to explore towns and tap completed checkpoints to replay their lessons for revision. Their chosen pet continues to mark their **current active checkpoint**, not whichever old lesson they happen to view. Include a discreet **Return to My Level** control that smoothly scrolls back to the current checkpoint. Future locked stones remain visible but cannot be entered; exploring completed areas never resets progression.

## Code City signs and numbered checkpoints — approved (2026-10-03)
- District transitions use **modest futuristic roadside signs or billboards**, seamlessly integrated into the original blue floating-highway map, not giant welcome screens.
- The floating world remains futuristic blue/cyan; each district's road sign may have a subtle identifying accent color. **HTML Town specifically uses BLUE** (not orange). Other district sign accents are provisional until the visuals are finalized.
- Level checkpoints are **glowing futuristic tech pads**, not plain circles or conventional stones. Each checkpoint pad displays its **NUMBER ONLY**, with no book or code icon.
- Preserve existing states: completed pads blue with cyan checkmarks; current pad brighter; future pads softly dimmed. Keep checkpoint numbering prominent and aligned directly on the continuous road.

## Code City animation scope — simplified following Bri's concern (2026-10-03)
Keep **floating-road scenery, buildings, waterfalls and district backgrounds STATIC** for reliability and fidelity to the approved screenshot. Limit Code City motion to only (1) the chosen pet's movement between completed/current checkpoints, and (2) smooth camera auto-scroll to follow that pet. Test both separately on mobile before considering any other decorative motion. Do not promise untested complex animation or add it without explicit approval.

## Boss Build checkpoint appearance — approved (2026-10-03)
At the end of each town, the **Boss Build checkpoint is noticeably larger and more impressive** than ordinary numbered tech pads, while retaining the approved original blue futuristic floating-highway visual language. Keep ordinary checkpoints as number-only glowing pads; distinguish Boss Builds visually without changing the continuous scrolling road or adding decorative animation.

## Code City district length — approved (2026-10-03)
**Level counts vary by town based on its real teaching curriculum**, not equal-length or decorative district sizes. Map each meaningful short lesson/quiz to a checkpoint, include the previously approved topic challenges and final Boss Build, and adjust the physical length/number of checkpoint pads to fit. Reuse the established HTML/CSS/JavaScript lesson plan where suitable; plan Python Lab and Data Vault lessons fully before inventing their exact counts. Do not force an identical number of levels in each district.

## Code City map navigation — approved (2026-10-03)
Code City uses **vertical scrolling only**, like Candy Crush. Do **not** implement pinch-to-zoom, zoom buttons or a draggable/zoomable map. Keep all checkpoint pads, signs and roads at their designed scale, with automatic scrolling to the player's current checkpoint as approved.

## Code City progression direction — approved (2026-10-03)
Code City progression moves **UPWARD**: the player begins toward the lower part of the long vertical map and advances upward along the continuous futuristic blue floating highway toward each next island/town. Ordinary navigation remains vertical scrolling only. On reopening or completing lessons, auto-scroll upward/to the currently unlocked checkpoint, with the chosen pet hovering above the active pad. Maintain seamless district transitions.

## Locked checkpoint tap behavior — assistant-selected at Bri's request (2026-10-03)
When a player taps a future **locked** Code City checkpoint, their chosen Code Pet displays a **brief, unobtrusive speech bubble** explaining which prerequisite lesson or Boss Build needs completing first (e.g., "Finish Level 7 first!"). Do not navigate away, open a blocking modal, reveal answers, skip lessons, or change saved progress. Keep the futuristic road and numbered checkpoint layout unchanged.

## Continuous checkpoint numbering — assistant-selected at Bri's request (2026-10-03)
Checkpoint numbers **continue sequentially across all five towns** instead of restarting from 1 in each district. This supports the seamless, upward-scrolling road. District names remain on modest roadside billboards and define town boundaries; ordinary glowing tech pads display the global level number only. Boss Build pads are visually larger, as approved.
