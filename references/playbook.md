# Complete UI/UX Engineering Playbook (Visual AI Reference)

Compiled from **Strategy Fox** (`strategyfox.in`) & **Motion UI Interface** (`@motion_ui_interface`).  
Every single rule below includes its **own inline UI screenshot** so an AI or engineer can see the exact visual pattern without guessing.

---

# PART I — STRATEGY FOX (`strategyfox.in`)

## 1. 10 UI States You Must Design Before Shipping
> [Reel](https://www.facebook.com/reel/1829906794685478/)

### 1.1 Empty state
**Rule:** Say why it is empty, then give one next step (`Browse bestsellers`).  
![01 Empty State](screenshots/01_empty.jpg)

### 1.2 Loading state
**Rule:** Show the shape of what is coming (skeletons), not a spinner.  
![02 Loading State](screenshots/02_loading.jpg)

### 1.3 Error state
**Rule:** State what went wrong, whose fault it is, and how to fix it (`Try another card` / `Pay with UPI instead`).  
![03 Error State](screenshots/03_error.jpg)

### 1.4 No internet
**Rule:** Keep cached content on screen, say what still works, and show `Reconnecting...`.  
![04 No Internet](screenshots/04_no_internet.jpg)

### 1.5 Slow network
**Rule:** Show real progress (`Loading images · 3 of 6 · 50%`) and offer a lighter path (`Switch to lite mode`).  
![05 Slow Network](screenshots/05_slow_network.jpg)

### 1.6 No search results
**Rule:** Fix the typo for them (`Did you mean blue shoes?`) and suggest a next search.  
![06 No Search Results](screenshots/06_no_search.jpg)

### 1.7 Permission denied
**Rule:** Explain why you need it (`Nothing is stored`) and give a way back (`Allow in Settings` / `Upload a photo instead`).  
![07 Permission Denied](screenshots/07_permission.jpg)

### 1.8 Session expired
**Rule:** Save their work before signing them out, confirm it is saved, and give `Sign in and continue`.  
![08 Session Expired](screenshots/08_session_expired.jpg)

### 1.9 Form validation
**Rule:** Flag the exact field inline with how to fix it (`Add a domain, like name@strategyfox.in`).  
![09 Form Validation](screenshots/09_form_validation.jpg)

### 1.10 Success state
**Rule:** Confirm, reassure with key details (order ID, arrival, address), then show what happens next.  
![10 Success State](screenshots/10_success.jpg)

---

## 2. 10 Important UI Laws
> [Reel](https://www.facebook.com/reel/1823438042320648/)

### 2.1 Peak-End Rule
**Rule:** Best moment + last moment. Make checkout feel like a win and end on a thank you.  
![Peak-End Rule](screenshots/uilaw_01_peak_end.jpg)

### 2.2 Zeigarnik Effect
**Rule:** Unfinished = unforgettable. Show a profile at 80% ("1 step left") so users come back to finish.  
![Zeigarnik Effect](screenshots/uilaw_02_zeigarnik.jpg)

### 2.3 Doherty Threshold
**Rule:** Respond in `0.4s` (`< 400ms`), or fake it with a `0.1s` skeleton so it never feels frozen.  
![Doherty Threshold](screenshots/uilaw_03_doherty.jpg)

### 2.4 Tesler's Law
**Rule:** You carry the complexity—take the PIN code and auto-fill City & State.  
![Tesler's Law](screenshots/uilaw_04_tesler.jpg)

### 2.5 Aesthetic-Usability Effect
**Rule:** Pretty feels easy. Better spacing and typography make the same form feel easier.  
![Aesthetic-Usability Effect](screenshots/uilaw_05_aesthetic.jpg)

### 2.6 Postel's Law
**Rule:** Accept anything, store one. Accept any phone format and normalize it on save.  
![Postel's Law](screenshots/uilaw_06_postel.jpg)

### 2.7 Parkinson's Law
**Rule:** Give less time, get it done. Show `"takes 2 min"` + autofill.  
![Parkinson's Law](screenshots/uilaw_07_parkinson.jpg)

### 2.8 Goal-Gradient Effect
**Rule:** Show the finish line. Give 2 free loyalty stamps out of 10 so users start 20% done.  
![Goal-Gradient Effect](screenshots/uilaw_08_goal_gradient.jpg)

### 2.9 Occam's Razor
**Rule:** Remove until it breaks. Keep only image, price, and one primary button.  
![Occam's Razor](screenshots/uilaw_09_occams.jpg)

### 2.10 Principle of Least Effort
**Rule:** Make the easy path yours—1-tap `Pay with UPI` beats a 14-field form.  
![Principle of Least Effort](screenshots/uilaw_10_least_effort.jpg)

---

## 3. 10 UX & Psychology Laws
> [Reel](https://www.facebook.com/reel/1807778290477289/)

### 3.1 Jakob's Law
**Rule:** Familiar beats clever. Put the cart where users already look (top right).  
![Jakob's Law](screenshots/uxlaw_01_jakob.jpg)

### 3.2 Hick's Law
**Rule:** Fewer options = faster action. Cutting 10 options to 3 drops decision time from `6.2s` to `1.1s`.  
![Hick's Law](screenshots/uxlaw_02_hick.jpg)

### 3.3 Miller's Law
**Rule:** Chunk it (`7 ± 2` limit). Split 16-digit card numbers into `4 x 4` blocks.  
![Miller's Law](screenshots/uxlaw_03_miller.jpg)

### 3.4 Law of Proximity
**Rule:** Close = related. Place each label closer to its own input field than to the field above it.  
![Law of Proximity](screenshots/uxlaw_04_proximity.jpg)

### 3.5 Law of Similarity
**Rule:** Same look = same job. Keep all links the same color and style so none are missed.  
![Law of Similarity](screenshots/uxlaw_05_similarity.jpg)

### 3.6 Law of Common Region
**Rule:** A border makes a group. Wrap image, title, price, and CTA inside one card.  
![Law of Common Region](screenshots/uxlaw_06_common_region.jpg)

### 3.7 Law of Continuity
**Rule:** Lead the eye. Let the last card peek off the edge of a horizontal carousel so users know to swipe.  
![Law of Continuity](screenshots/uxlaw_07_continuity.jpg)

### 3.8 Von Restorff Effect
**Rule:** The odd one wins. Make your primary CTA (`Buy now`) pop from secondary actions.  
![Von Restorff Effect](screenshots/uxlaw_08_von_restorff.jpg)

### 3.9 Serial Position Effect
**Rule:** Ends stick, middle slips. Put key offers (`Free shipping`, `Buy 1 get 1`) first and last.  
![Serial Position Effect](screenshots/uxlaw_09_serial_position.jpg)

### 3.10 Fitts's Law
**Rule:** Big targets in the thumb zone get tapped fastest (`0.5s` vs `2.4s`).  
![Fitts's Law](screenshots/uxlaw_10_fitts.jpg)

---

## 4. Top 3 Before & After Redesigns
> [Reel](https://www.facebook.com/reel/1800100851259210/)

### 4.1 The Run Log
Replace 5 plain text lines in a grey box with a hero metric (`5.2 KM`), drawn route map, and charted pace graph.  
![Run Log After](screenshots/ba_03_run_log.jpg)

### 4.2 The Job Card
Pull the title beside the logo, turn metadata into chips, and use relative dates (`Posted 2 days ago`).  
![Job Card After](screenshots/ba_02_job_card.jpg)

### 4.3 The Dashboard
Replace 14 white boxes with a dark canvas + glass cards, one hero metric per block, and color only where it carries meaning.  
![Dashboard After](screenshots/ba_01_dashboard.jpg)

---

## 5. Top 6 Font Combos
> [Reel](https://www.facebook.com/reel/1968481161022226/)

### Rank 6: Plus Jakarta Sans + Lora (Clean, safe SaaS)
![Plus Jakarta Sans + Lora](screenshots/font_06_jakarta.jpg)

### Rank 5: Space Grotesk + Inter (Developer tools & technical pages)
![Space Grotesk + Inter](screenshots/font_05_space_grotesk.jpg)

### Rank 4: Windsor + Ano (Warm, human D2C brands)
![Windsor + Ano](screenshots/font_04_windsor.jpg)

### Rank 3: Syne + DM Mono (Loud, sharp creative studios)
![Syne + DM Mono](screenshots/font_03_syne.jpg)

### Rank 2: Bricolage Grotesque + Manrope (Expressive display + calm body for startups)
![Bricolage Grotesque + Manrope](screenshots/font_02_bricolage.jpg)

### Rank 1: SF Pro Display (`> 20px`) + SF Pro Text (`<= 20px`)
![SF Pro Display + SF Pro Text](screenshots/font_01_sf_pro.jpg)

---

## 6. Top 6 Website Color Combos
> Formula: *Pick two colors that do the heavy lifting, then let one unexpected accent break the rules.* ([Reel](https://www.facebook.com/reel/1718370492982533/))

### Rank 6: Electric Purple `#7E02FD` + Deep Violet `#440489` + Soft Blush Pink `#F8D7E6`
![Rank 6 Color](screenshots/color_06_purple.jpg)

### Rank 5: Sky Blue `#0169D9` + White `#FFFFFF` + Hot Pink `#E83395`
![Rank 5 Color](screenshots/color_05_sky.jpg)

### Rank 4: Deep Blue `#08278D` + Pure White `#FFFFFF` + Bubblegum Pink `#F081CC`
![Rank 4 Color](screenshots/color_04_deep_blue.jpg)

### Rank 3: Electric Yellow `#FCE000` + Deep Cobalt `#0F0A87` + Hot Pink `#FC02B4`
![Rank 3 Color](screenshots/color_03_yellow.jpg)

### Rank 2: Powder Blue `#AEC0C5` + Pure White `#FFFFFF` + Vibrant Racing Orange `#F45B0B`
![Rank 2 Color](screenshots/color_02_racing.jpg)

### Rank 1: Midnight Black `#02070A` + Electric Blue `#0287DE` + Cantaloupe Orange `#FC7D4F`
![Rank 1 Color](screenshots/color_01_midnight.jpg)

---

## 7. 10 Website Design Styles
> [Reel](https://www.facebook.com/reel/2543503519471609/)

1. **Skeuomorphism** — Buttons that look like real buttons.  
![Skeuomorphism](screenshots/style_01_skeuomorphism.jpg)
2. **Minimalism** — White space does the talking.  
![Minimalism](screenshots/style_02_minimalism.jpg)
3. **Glassmorphism** — Frosted panels floating over color.  
![Glassmorphism](screenshots/style_03_glassmorphism.jpg)
4. **Neumorphism** — Soft shapes pressed into the surface.  
![Neumorphism](screenshots/style_04_neumorphism.jpg)
5. **Claymorphism** — Puffy, rounded, touchable.  
![Claymorphism](screenshots/style_05_claymorphism.jpg)
6. **Neo brutalism** — Thick borders, flat color, nothing polite.  
![Neo Brutalism](screenshots/style_06_neobrutalism.jpg)
7. **Bento grid** — Tiles of different sizes on one neat board.  
![Bento Grid](screenshots/style_bento.jpg)
8. **Retro Y2K** — Chrome, gradients, 2003 nostalgia.  
![Retro Y2K](screenshots/style_08_retroy2k.jpg)
9. **Liquid glass** — Depth and refraction, like water on the screen.  
![Liquid Glass](screenshots/style_liquid_glass.jpg)
10. **Flat design** — No shadows, no textures, just color and shape.  
![Flat Design](screenshots/style_10_flat.jpg)

---

## 8. 17 Tells Your Design Was "Vibe Coded" (Avoid These)
> [Reel](https://www.facebook.com/reel/1133425995874370/)

1. **Lucide icons on every screen**  
![Lucide Icons](screenshots/vibe_01_lucide.jpg)
2. **Emojis in every heading**  
![Emojis](screenshots/vibe_02_emojis.jpg)
3. **Generic liquid glass everywhere**  
![Liquid Glass](screenshots/vibe_03_liquid_glass.jpg)
4. **3+ em dashes (`—`) per sentence**  
![Em Dashes](screenshots/vibe_04_em_dashes.jpg)
5. **Defaulting to Inter, Geist, or Space Grotesk**  
![Default Fonts](screenshots/vibe_05_fonts.jpg)
6. **Three feature cards in a row**  
![Three Cards](screenshots/vibe_06_three_cards.jpg)
7. **Bento grids everywhere**  
![Bento Grids](screenshots/vibe_07_bento.jpg)
8. **Fake terminal windows**  
![Terminal Window](screenshots/vibe_08_terminal.jpg)
9. **"It's not X, it's Y" copywriting**  
![Not X Its Y](screenshots/vibe_09_not_x_y.jpg)
10. **Placeholder "coming soon" instead of real demos**  
![No Real Demos](screenshots/vibe_10_no_demos.jpg)
11. **Purple + black palettes**  
![Purple and Black](screenshots/vibe_11_purple_black.jpg)
12. **Glowing radial orbs**  
![Radial Orbs](screenshots/vibe_12_radial_orbs.jpg)
13. **Dot grids behind sections**  
![Dot Grids](screenshots/vibe_13_dot_grids.jpg)
14. **Sparkle icons on every AI button**  
![Sparkle Icons](screenshots/vibe_14_sparkles.jpg)
15. **Animated arrows on every link**  
![Animated Arrows](screenshots/vibe_15_arrows.jpg)
16. **Same `translateY(-4px) scale(1.01)` hover on every card**  
![Hover Animations](screenshots/vibe_16_hover.jpg)
17. **Rainbow pastel coloring across feature cards**  
![Rainbow Coloring](screenshots/vibe_17_rainbow.jpg)

**Recommended GitHub Design Skills:**  
![6 GitHub Claude Design Skills](screenshots/vibe_06_skills.jpg)

---

# PART II — MOTION UI INTERFACE (`@motion_ui_interface`)

## 9. UX Laws in Action (Parts 1, 2 & 4)

### 9.1 Part 1 — Fitts, Hick, Chunking, Doherty, Proximity, Von Restorff
> [Reel](https://www.instagram.com/reel/Dd25eCoBJGr/)

1. **Fitts's Law:** Make the main action big and close (`0.28s` vs `0.66s`).  
![Fitts's Law](screenshots/ig_ux1_01_fitts.jpg)
2. **Hick's Law:** Show the few that matter (4 + More = `0.46s`), hide the rest (`0.74s`).  
![Hick's Law](screenshots/ig_ux1_02_hick.jpg)
3. **Chunking:** Working memory holds ~4 chunks. Group 10 digits into `415 555 0123`.  
![Chunking](screenshots/ig_ux1_03_chunking.jpg)
4. **Doherty Threshold:** Respond within `400ms` (`0.1s` feedback), even for slow work.  
![Doherty Threshold](screenshots/ig_ux1_04_doherty.jpg)
5. **Proximity:** Keep labels closest to their field (`8px` to own field vs `24px` to next).  
![Proximity](screenshots/ig_ux1_05_proximity.jpg)
6. **Von Restorff Effect:** One standout, never three. Highlight only the recommended plan.  
![Von Restorff](screenshots/ig_ux1_06_von_restorff.jpg)

### 9.2 Part 2 — Goal Gradient, Postel, Tesler, Similarity, Serial Position, Peak-End
> [Reel](https://www.instagram.com/reel/Dd4UtBDBsIS/)

1. **Goal Gradient:** Never start progress at zero (`34%` finish vs `19%` when 2/10 stamps pre-filled).  
![Goal Gradient](screenshots/ig_ux2_01_goal.jpg)
2. **Postel's Law:** Accept any format (`(415) 555-0123`, spaces, dashes), then clean it up.  
![Postel's Law](screenshots/ig_ux2_02_postel.jpg)
3. **Tesler's Law:** Let the system carry the work—ask ZIP first, autofill City & State (`16` keys vs `31`).  
![Tesler's Law](screenshots/ig_ux2_03_tesler.jpg)
4. **Law of Similarity:** Make what taps look tappable (add `>` chevrons to tappable settings rows).  
![Similarity](screenshots/ig_ux2_04_similarity.jpg)
5. **Serial Position:** Put key actions first or last (`Cart` at slot 5 instead of buried in slot 3).  
![Serial Position](screenshots/ig_ux2_05_serial.jpg)
6. **Peak-End Rule:** Design the last screen on purpose (`8/10` warm finish vs `4.5/10` plain receipt).  
![Peak-End](screenshots/ig_ux2_06_peak_end.jpg)

### 9.3 Part 4 — Closure, Figure-Ground, Banner Blindness, Parkinson, Connectedness, Choice Overload
> [Reel](https://www.instagram.com/reel/Del7XTgsuwI/)

1. **Law of Closure:** Let the next card peek (`32%` showing) so users know the row scrolls.  
![Closure](screenshots/ig_ux4_01_closure.jpg)
2. **Figure-Ground:** Dim what's behind the focus (`70%` backdrop drops background contrast from `17.4:1` to `2.5:1`).  
![Figure-Ground](screenshots/ig_ux4_02_figure_ground.jpg)
3. **Banner Blindness:** Don't make important notices look like ads—style them like feed content.  
![Banner Blindness](screenshots/ig_ux4_03_banner_blindness.jpg)
4. **Parkinson's Law:** Fill in what you already know (postcode lookup = `7` keys vs `30`).  
![Parkinson's Law](screenshots/ig_ux4_04_parkinson.jpg)
5. **Uniform Connectedness:** Connect the steps of a flow with one line (`1` group instead of `4` loose circles).  
![Connectedness](screenshots/ig_ux4_05_connectedness.jpg)
6. **Choice Overload:** Show fewer options upfront (`6` flavors = `30%` conversion vs `24` flavors = `3%`).  
![Choice Overload](screenshots/ig_ux4_06_choice_overload.jpg)

---

## 10. Component Engineering Playbooks ("6 Mistakes" Series)

### 10.1 Dropdowns ([Reel](https://www.instagram.com/reel/Dc0YIw_I7F5/))
1. **Over 10 options? Let them type** (type-to-filter).  
![Dropdown Filter](screenshots/ig_dd_01_filter.jpg)
2. **Let them type the date** (don't force clicking back 390 months).  
![Dropdown Dates](screenshots/ig_dd_02_dates.jpg)
3. **Multi-select stays open** with checkboxes + `Done` button.  
![Dropdown Multi](screenshots/ig_dd_03_multi.jpg)
4. **Flip it before it clips** (collision-aware portal opening upward).  
![Dropdown Flip](screenshots/ig_dd_04_flip.jpg)
5. **Say why it's off** (inline blocker + unlock CTA, not silent grey).  
![Dropdown Reasons](screenshots/ig_dd_05_reasons.jpg)
6. **Under five? Show them all** (segmented control/radios instead of a menu).  
![Dropdown Under 5](screenshots/ig_dd_06_under5.jpg)

### 10.2 Animation & Motion ([Reel](https://www.instagram.com/reel/DcRHJKGoMS-/))
1. **Keep UI motion under `250ms`** (`180ms` feels crisp; `600ms` feels broken).  
![Anim 250ms](screenshots/ig_anim_01_250ms.jpg)
2. **Ease out. Never linear** (`cubic-bezier(.2, .8, .2, 1)`).  
![Anim Ease Out](screenshots/ig_anim_02_easeout.jpg)
3. **Bounce is a reward, not a default** (menus should land cleanly without overshoot).  
![Anim No Overshoot](screenshots/ig_anim_03_overshoot.jpg)
4. **Grow it from what opened it** (`transform-origin: top right` on the trigger).  
![Anim Origin](screenshots/ig_anim_04_origin.jpg)
5. **Honour reduced motion** (`@media (prefers-reduced-motion)` -> opacity fade only, 0px travel).  
![Anim Reduced Motion](screenshots/ig_anim_05_reduced.jpg)
6. **Animate `transform`, never layout** (`scaleX` = 60fps vs `width` = 12fps jank).  
![Anim Transform](screenshots/ig_anim_06_transform.jpg)

### 10.3 Loading States ([Reel](https://www.instagram.com/reel/Db6CwOhBC3x/))
1. **Show the shape, not the spin** (skeleton mirroring layout).  
![Load Skeleton](screenshots/ig_load_01_skeleton.jpg)
2. **Answer the click in `100ms`** and lock the button to prevent double-orders.  
![Load 100ms](screenshots/ig_load_02_100ms.jpg)
3. **Reserve the space first** (`0px` layout shift so late content never steals clicks).  
![Load No Shift](screenshots/ig_load_03_shift.jpg)
4. **Name the step. Show the number** (`File 4 of 5 · 76% · ~2s left`).  
![Load Honest Bars](screenshots/ig_load_04_bars.jpg)
5. **Load in parts, not in one lump** (stream shell first, fill regions independently).  
![Load Stream](screenshots/ig_load_05_stream.jpg)
6. **Give every load a deadline** (timeout + `Try again` / `Go back`).  
![Load Timeout](screenshots/ig_load_06_timeout.jpg)

### 10.4 Navigation ([Reel](https://www.instagram.com/reel/DcYD10Rs39R/))
1. **Label every destination** (icons + text labels, never mystery meat).  
![Nav Labels](screenshots/ig_nav_01_labels.jpg)
2. **Always mark where they are** (active tab + breadcrumb trail).  
![Nav Active](screenshots/ig_nav_02_active.jpg)
3. **Show the nav. Don't fold it** into a desktop hamburger.  
![Nav Top Level](screenshots/ig_nav_03_toplevel.jpg)
4. **Flatten it into one panel** instead of 4-level cascading flyouts.  
![Nav Flat](screenshots/ig_nav_04_flat.jpg)
5. **Give every step a URL** so Back returns one step, not to the start.  
![Nav URL](screenshots/ig_nav_05_url.jpg)
6. **Five tabs. Forty-eight pixels** on mobile bottom nav, always labelled.  
![Nav Tabs](screenshots/ig_nav_06_tabs.jpg)

### 10.5 Settings ([Reel](https://www.instagram.com/reel/DdRneVWhBSY/))
1. **Confirm every save** in-place (`✓ Saved just now`).  
![Settings Confirm](screenshots/ig_set_01_confirm.jpg)
2. **Put the scope on the row** (personal vs workspace-wide blast radius).  
![Settings Scope](screenshots/ig_set_02_scope.jpg)
3. **Make settings searchable** + grouped into sections.  
![Settings Search](screenshots/ig_set_03_search.jpg)
4. **A label is not an explanation**—add one line explaining the consequence.  
![Settings Explain](screenshots/ig_set_04_explain.jpg)
5. **Mark what changed** and give a 1-tap `Reset` per row.  
![Settings Reset](screenshots/ig_set_05_reset.jpg)
6. **Say when it takes effect** (e.g., `"Applies after restart"`) before they flip it.  
![Settings Restart](screenshots/ig_set_06_restart.jpg)

### 10.6 File Uploads ([Reel](https://www.instagram.com/reel/Dc5WPlDBSj0/))
1. **Make the whole card the drop zone** (drop, click, or paste).  
![Upload Dropzone](screenshots/ig_up_01_dropzone.jpg)
2. **Show percent, size, speed, and a Cancel button**.  
![Upload Progress](screenshots/ig_up_02_progress.jpg)
3. **Validate at the drop** (refuse unsupported types before sending bytes).  
![Upload Precheck](screenshots/ig_up_03_precheck.jpg)
4. **Print the limits on the zone** (`PNG, JPG or PDF · up to 25 MB`).  
![Upload Limits](screenshots/ig_up_04_limits.jpg)
5. **Fail the file, not the batch** (retry the 1 failed file, keep the 4 good ones).  
![Upload Per-File](screenshots/ig_up_05_perfile.jpg)
6. **Upload in the background** (docked corner tray, never a blocking modal).  
![Upload Dock](screenshots/ig_up_06_dock.jpg)

### 10.7 Filters ([Reel](https://www.instagram.com/reel/Dc-xIHBIzq_/))
1. **Never blank the results** on every tick—hold the old list and mark it stale.  
![Filter Stale](screenshots/ig_flt_01_stale.jpg)
2. **Show what's applied** as removable chips above the list.  
![Filter Chips](screenshots/ig_flt_02_chips.jpg)
3. **Put the count on the option** so users see `0` before tapping.  
![Filter Counts](screenshots/ig_flt_03_counts.jpg)
4. **Name what killed it** when 0 results match, and offer a 1-tap `Drop it`.  
![Filter Culprit](screenshots/ig_flt_04_culprit.jpg)
5. **Total the Apply button** on mobile (`Show 49 results`).  
![Filter Mobile](screenshots/ig_flt_05_mobile.jpg)
6. **Filters belong in the URL** so refresh, back, and share all work.  
![Filter URL](screenshots/ig_flt_06_url.jpg)

### 10.8 Date Pickers ([Reel](https://www.instagram.com/reel/DdjqDCyBDTg/))
1. **Let them type the date** (`14/3/1987` -> calendar jumps).  
![Date Type](screenshots/ig_dt_01_type.jpg)
2. **Preset the ranges they ask for** (`Today`, `Last 7 days`, `Last 30 days`, `This quarter`).  
![Date Presets](screenshots/ig_dt_02_presets.jpg)
3. **Grey needs a reason** + link to the next open date.  
![Date Grey](screenshots/ig_dt_03_grey.jpg)
4. **Echo the date back in words** (`Wed 4 March 2026`) so `03/04` isn't ambiguous.  
![Date Echo](screenshots/ig_dt_04_echo.jpg)
5. **A phone gets a sheet** (`48px` cells), never a tiny `26px` desktop popover.  
![Date Sheet](screenshots/ig_dt_05_sheet.jpg)
6. **Name both timezones** (`9:00 AM GMT+1 · 8:00 AM GMT`).  
![Date Timezone](screenshots/ig_dt_06_tz.jpg)

### 10.9 Form Validation ([Reel](https://www.instagram.com/reel/Db3U7U8Blq6/))
1. **Validate on blur** (when they leave the field), not all at once on submit.  
![Form Blur](screenshots/ig_frm_01_blur.jpg)
2. **Say yes, not just no** (green check when valid).  
![Form Green](screenshots/ig_frm_02_green.jpg)
3. **Name the fix, not the fault** (`Add 2 more characters` instead of `Invalid input`).  
![Form Fix](screenshots/ig_frm_03_fix.jpg)
4. **Put the error where the eye is** (inline under the field, not a top summary).  
![Form Inline](screenshots/ig_frm_04_inline.jpg)
5. **Show the rules before they fail** (live password checklist).  
![Form Rules](screenshots/ig_frm_05_rules.jpg)
6. **Design all 6 field states:** Default, Focus, Filled, Error, Success, Disabled.  
![Form 6 States](screenshots/ig_frm_06_states.jpg)

### 10.10 Pagination ([Reel](https://www.instagram.com/reel/DdtzWoMhLtW/))
1. **Show them the total** (`Page 3 of 48 · 1,187 results`).  
![Pagination Total](screenshots/ig_pg_01_total.jpg)
2. **Reserve the space first** so rows loading above don't shove the tapped row.  
![Pagination Shift](screenshots/ig_pg_02_shift.jpg)
3. **A footer has to be reachable** (use `Load more` instead of endless infinite scroll).  
![Pagination Footer](screenshots/ig_pg_03_footer.jpg)
4. **Put the page in the URL** (`?page=3&sort=price`).  
![Pagination URL](screenshots/ig_pg_04_url.jpg)
5. **Say when it's over** (`End of results · 1,187 shown · Back to top`).  
![Pagination End](screenshots/ig_pg_05_end.jpg)
6. **Back means back**—restore scroll position and highlight the row they tapped.  
![Pagination Back](screenshots/ig_pg_06_back.jpg)

### 10.11 Error States ([Reel](https://www.instagram.com/reel/Dc6h6w1BwZ3/))
1. **No action fails silently** (500 must surface an inline failure + `Try again`).  
![Error Silent](screenshots/ig_err_01_silent.jpg)
2. **Name it, then offer the fix** (cause, cost, action—never a raw hex code).  
![Error Name](screenshots/ig_err_02_name.jpg)
3. **Never clear on failure**—preserve every word they typed.  
![Error Keep](screenshots/ig_err_03_keep.jpg)
4. **One boundary per widget** (one failed API card must not crash healthy widgets).  
![Error Scope](screenshots/ig_err_04_scope.jpg)
5. **Retry the request, not the page** (keep filters & state intact).  
![Error Retry](screenshots/ig_err_05_retry.jpg)
6. **Offline is a state, not a crash** (queue the action and send on reconnect).  
![Error Offline](screenshots/ig_err_06_offline.jpg)

### 10.12 Onboarding ([Reel](https://www.instagram.com/reel/DcfnGcxIZgZ/))
1. **Ask permissions at the moment you need them**, with a reason attached.  
![Onboarding Perm](screenshots/ig_onb_01_perm.jpg)
2. **Cut the 5-slide tour. Open the product** and teach in place.  
![Onboarding Tour](screenshots/ig_onb_02_tour.jpg)
3. **Let them try before they join** (account saves their work, doesn't gate an empty room).  
![Onboarding Signup](screenshots/ig_onb_03_signup.jpg)
4. **Show `Step 2 of 4`** and a progress bar that moves.  
![Onboarding Steps](screenshots/ig_onb_04_steps.jpg)
5. **One question per screen** instead of 14 fields on day one.  
![Onboarding One Ask](screenshots/ig_onb_05_oneask.jpg)
6. **Always leave the door open** (`Skip for now`, `Back`, `Close`).  
![Onboarding Skip](screenshots/ig_onb_06_skip.jpg)

### 10.13 Search ([Reel](https://www.instagram.com/reel/DcT2phFhWsS/))
1. **Never end on "no results"**—offer spelling fixes, filter clears, and related categories.  
![Search Exit](screenshots/ig_src_01_exit.jpg)
2. **Debounce (`200ms`), then cancel in-flight requests** so stale responses never win.  
![Search Debounce](screenshots/ig_src_02_debounce.jpg)
3. **Tolerate typos** (fuzzy match ±2 edits) and say what you corrected.  
![Search Fuzzy](screenshots/ig_src_03_fuzzy.jpg)
4. **Fill the empty box before they type** (recent + trending shortcuts on focus).  
![Search Recent](screenshots/ig_src_04_recent.jpg)
5. **Highlight the match. Show the context** (source path / snippet).  
![Search Match](screenshots/ig_src_05_match.jpg)
6. **Own the arrow keys** (`↑`, `↓`, `Enter`, `Esc` with `aria-activedescendant`).  
![Search Arrows](screenshots/ig_src_06_arrows.jpg)

### 10.14 Modals & Dialogs ([Reel](https://www.instagram.com/reel/Db8e_pjB-9D/))
1. **Three exits on every dialog:** `X` button, `Esc` key, and backdrop click.  
![Modal Exits](screenshots/ig_mod_01_exits.jpg)
2. **Trap the focus inside, then hand it back** on close.  
![Modal Focus](screenshots/ig_mod_02_focus.jpg)
3. **Name what's about to be lost** (`4 files, 128 comments`) and default to the safe action (`Keep it`).  
![Modal Destructive](screenshots/ig_mod_03_sure.jpg)
4. **On mobile, use a bottom sheet** so actions stay in the thumb arc.  
![Modal Sheet](screenshots/ig_mod_04_sheet.jpg)
5. **One layer. Swap the contents**—never stack a modal on a modal.  
![Modal Stack](screenshots/ig_mod_05_stack.jpg)
6. **Dismiss should never destroy**—check for dirty unsaved edits before closing.  
![Modal Dirty Check](screenshots/ig_mod_06_dirty.jpg)

### 10.15 Accessibility ([Reel](https://www.instagram.com/reel/DcwLKv_B34o/))
1. **`4.5:1` contrast is the floor** for body copy (`3:1` for large text > 24px and icons).  
![A11y Contrast](screenshots/ig_a11y_01_contrast.jpg)
2. **Say where the link goes** (`compare all plans`, never `click here`).  
![A11y Links](screenshots/ig_a11y_02_links.jpg)
3. **Labels stay. Placeholders hint**—never use placeholder as the only label.  
![A11y Labels](screenshots/ig_a11y_03_label.jpg)
4. **Every control needs a name** (visible label or `aria-label`).  
![A11y Icons](screenshots/ig_a11y_04_icons.jpg)
5. **Show focus on every stop** (`:focus-visible`, 2px ring, never `outline: none`).  
![A11y Focus](screenshots/ig_a11y_05_focus.jpg)
6. **Let the layout reflow at 200% zoom** (no fixed-height clipping boxes).  
![A11y Zoom](screenshots/ig_a11y_06_zoom.jpg)

---

## 11. UI Polish Specs ("Level Up — 6 Decisions" Series)

### 11.1 Primary Button Polish ([Reel](https://www.instagram.com/reel/Ddy5RJOha1U/) & [Buttons](https://www.instagram.com/reel/DcBt6RkoSmN/))
1. **Size:** `48px` tall (min `44px`), `24px` side padding.  
![Btn Size](screenshots/ig_exp_01_size.jpg)
2. **Label:** `17px`, weight `600`, sentence case, `verb + object` (`Add to cart`, never `OK` or `Submit`).  
![Btn Label](screenshots/ig_exp_02_label.jpg)
3. **Contrast:** Label `>= 4.5:1`, 1px rim `>= 3:1` against page.  
![Btn Contrast](screenshots/ig_exp_03_contrast.jpg)
4. **Depth:** Light from above—lit top edge, recessed track, downward shadow (`y: 8, blur: 24`).  
![Btn Depth](screenshots/ig_exp_04_depth.jpg)
5. **Pill & Icon:** `radius = height / 2` (`24px`), one `20px` icon `10px` from label.  
![Btn Pill](screenshots/ig_exp_05_pill.jpg)
6. **Motion:** Feedback in `100ms`, done in `300ms` (hover rim, press sink 1px, spinner -> check).  
![Btn Motion](screenshots/ig_exp_06_motion.jpg)
7. **Secondary Buttons:** Give bare text a border so it reads as clickable.  
![Btn Border](screenshots/ig_btn_02_border.jpg)

### 11.2 Login Form Polish ([Reel](https://www.instagram.com/reel/DdxddtWBsl_/))
1. **Hierarchy:** Big bold title, one primary button, everything else is a link.  
![Login Hier](screenshots/ig_log_01_hier.jpg)
2. **Spacing (8pt grid):** `56px` fields, `16px` between, `32px` before button.  
![Login Space](screenshots/ig_log_02_space.jpg)
3. **Labels:** Label above (`14px`), placeholder is a hint/example (`you@company.com`).  
![Login Label](screenshots/ig_log_03_label.jpg)
4. **Color & Focus:** 3 text tiers, 1 accent, `2px` focus ring always visible.  
![Login Color](screenshots/ig_log_04_color.jpg)
5. **Depth & Corners:** `24px` outer card radius, `12px` inner fields/buttons, hairline border + downward shadow.  
![Login Depth](screenshots/ig_log_05_depth.jpg)
6. **Motion:** Focus ring `150ms`, press `120ms`, spinner -> check `300ms`.  
![Login Motion](screenshots/ig_log_06_motion.jpg)

### 11.3 Product Card Polish ([Reel](https://www.instagram.com/reel/DduCKRKBmdx/))
1. **Hierarchy:** One loud element (`24px` title), quieter details (`13px`), weighted price (`20px`).  
![Card Hier](screenshots/ig_crd_01_hier.jpg)
2. **Spacing:** `8pt` grid (`24px` padding, `16px` between groups, `8px` between lines).  
![Card Space](screenshots/ig_crd_02_space.jpg)
3. **Color:** 3 text tiers (white, soft grey, faint grey) + 1 accent for price & button.  
![Card Color](screenshots/ig_crd_03_color.jpg)
4. **Depth:** `1px` border, top-lit surface gradient, soft downward shadow.  
![Card Depth](screenshots/ig_crd_04_depth.jpg)
5. **Nested Corners:** `inner_radius = outer_radius - padding` (`24 - 8 = 16`).  
![Card Corners](screenshots/ig_crd_05_corners.jpg)
6. **Motion:** `40ms` enter stagger, hover lift, press scale, `150–300ms` ease-out.  
![Card Motion](screenshots/ig_crd_06_motion.jpg)

### 11.4 Pricing Table Polish ([Reel](https://www.instagram.com/reel/DeCaoUihav4/))
1. **Hierarchy:** One loud number per column (`52px` bold price, `14px` caps plan name).  
![Pricing Hier](screenshots/ig_prc_01_hier.jpg)
2. **Spacing:** More space between plans (`20px`) than inside them (`14px` rows).  
![Pricing Space](screenshots/ig_prc_02_space.jpg)
3. **Emphasis:** One recommended plan (`MOST POPULAR` badge + accent border + the only filled button).  
![Pricing Emph](screenshots/ig_prc_03_emph.jpg)
4. **Depth:** Raise the recommended choice (`16px` elevation, soft shadow), not everything.  
![Pricing Depth](screenshots/ig_prc_04_depth.jpg)
5. **Anchor:** Default to Yearly (`-20%` chip) and show the struck-through old price (`$30 -> $24/mo`).  
![Pricing Anchor](screenshots/ig_prc_05_anchor.jpg)
6. **Motion:** Hover lift (`4px`), rolling price numbers on toggle (`300ms`), spinner -> check.  
![Pricing Motion](screenshots/ig_prc_06_motion.jpg)
