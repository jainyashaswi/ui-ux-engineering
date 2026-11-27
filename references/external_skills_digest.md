# External Design-Engineering Skills Digest

Distilled rules from the 6 open-source design skill repositories recommended for eliminating generic "AI-slop" UIs. Bundled directly so no external installation is required.

---

## 1. `emilkowalski/skills` (Design Engineering & Motion)
- **Should it animate?**
  - `100+ times/day` (keyboard shortcuts, command palette): **Never animate.**
  - `Tens of times/day` (hover, list nav): Remove or drastically reduce.
  - `Occasional` (modals, drawers, toasts): Standard animation (`< 300ms` for UI; modals/drawers up to `500ms`).
- **Custom Easing Curves (never built-in `ease-in`):**
  - `--ease-out: cubic-bezier(0.23, 1, 0.32, 1)` (entrances/exits — fast start, feels instant)
  - `--ease-in-out: cubic-bezier(0.77, 0, 0.175, 1)` (on-screen movement/morphs)
  - `--ease-drawer: cubic-bezier(0.32, 0.72, 0, 1)` (iOS-like sheet/drawer curve)
- **Press & Origin:**
  - Buttons must respond on `:active` (`transform: scale(0.97)`).
  - Popovers/menus scale from their trigger (`transform-origin`), starting from `scale(0.95); opacity: 0` (nothing in the real world appears from `scale(0)`).
- **Perceived Speed:** Fast-spinning spinners and `180ms` dropdowns feel measurably faster than `400ms` ones; after the first tooltip opens, skip delay/animation on sibling tooltips.

---

## 2. `jakubkrehel/skills` (`better-ui`, `better-layout`, `better-typography`, `better-colors`, `better-motion`, `better-accessibility`, `interface-review`)
- **Concentric Corner Radius:** `outer_radius = inner_radius + padding + border_width` (when inset is even and `<= 24px`).
- **Optical Alignment:** Nudge by eye where geometric centering looks off (`2px` less padding on icon side of a button; shift play triangles toward their point).
- **Shadows vs Borders:** Use layered transparent shadows for elevation; keep `1px` borders for dividers, table cells, selected states, and form inputs (which need `3:1` non-text contrast). Keep `border: 1px solid transparent` under shadow rings for forced-colors mode.
- **Image Outlines:** Give content images a `1px` inset outline (`rgba(0,0,0,0.1)` light / `rgba(255,255,255,0.1)` dark) so edges don't bleed into matching backgrounds.
- **Touch & Scroll:** Wrap hover styles in `@media (hover: hover)` so touch taps don't latch; set `overscroll-behavior: contain` on scrollable dialogs/drawers.
- **Icons:** Match icon stroke weight to adjacent text weight (`1.5px` at 400 -> `2.5px` at 700); use one icon library per surface and `currentColor` for states.
- **Change-Scoped Review Discipline:** Always inspect removed lines (`-` side of diff) for accidentally deleted `aria-label`, focus outlines, or reduced-motion rules, and expand blast radius 1 hop to consumers.

---

## 3. `ConardLi/garden-skills` (`web-design-engineer`)
- **Assets > Hex Codes:** Brand recognition comes from real logos, product imagery, and real UI screenshots—never substitute CSS silhouettes or hand-drawn SVGs for real product photos.
- **Design Read Before Code:** Define `visual-language`, `visual-variance (1-10)`, `motion-intensity (1-10)`, `information-density (1-10)`, and `brand-fidelity (1-10)` before picking tokens.
- **Four Positioning Questions:** Narrative role, viewing distance (`10cm` phone / `1m` laptop / `10m` projector), visual temperature, and capacity check (will content overflow?).
- **Code > Screenshots:** When both codebase and screenshots exist, extract design tokens from code rather than guessing from pixels.

---

## 4. `elayadesign/ai-design-skills` (`landing-page-design`)
- **One Offer -> One Audience -> One Primary Action:** Never place competing CTAs above the fold.
- **Above-the-Fold Formula:** Headline (outcome + audience) -> Subheadline (how + specificity) -> Primary CTA (verb + what they get, never "Submit"/"Learn more") -> One proof signal -> Hero visual.
- **Specificity Over Fluff:** Replace *"Save time and streamline"* with *"Cut weekly reporting from 4 hours to 15 minutes"*.
- **Risk Reversal & Proof Placement:** Put proof directly beside the claim it supports, and move FAQs earlier for high-friction offers.

---

## 5. `MengTo/Skills` (`audit-ai-design-slop` & `build-awwwards-quality-sites`)
- **The Removal Test (Default to Subtraction):** For every visual element, ask what information, state, action, or hierarchy it provides; if removing it improves clarity without losing that role, delete it.
- **Flag 6 Slop Categories:**
  1. **Decorative stacking:** Glow + gradient text + glass + borders + grid + particles competing together.
  2. **Template repetition:** Card treatment on every block, identical 3-up icon tiles, nested rounded boxes with no hierarchy.
  3. **Typography/copy clutter:** Empty superlatives, duplicate labels, centered walls of text.
  4. **Motion theater:** Motion that delays access, moves tap targets, or ignores `prefers-reduced-motion`.
  5. **Fake proof:** Invented metrics, stock testimonials, or logo walls with no real proof.
  6. **Established UI failures:** Competing primary actions, low contrast, clipping/overflow, hover-only info, missing states.
- **Single Smooth-Scroll Engine:** Never mix Lenis + Locomotive; always keep static first frames usable without JS/WebGL.

---

## 6. `Owl-Listener/designer-skills` (`design-critique` & `visual-critique`)
- **Structured Critique Format:** Separate exploration critiques from refinement critiques; frame observations concretely (*"I notice..."*, *"I wonder..."*, *"What if..."*) and always tie feedback to user goals and task completion rather than personal taste.
