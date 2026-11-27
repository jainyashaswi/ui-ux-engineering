---
name: ui-ux-engineering
description: >-
  Audit existing UI screens or design new interfaces using 200+ visual UI/UX engineering rules, psychological laws, component playbooks, accessibility standards, and anti-AI-slop principles. Use this skill whenever the user asks to review, audit, critique, fix, polish, or improve an existing UI/screen/app, OR asks to design, build, or mockup a new screen, component, form, modal, dashboard, or landing page. In Review Mode on multi-screen projects, tracks audit progress in `.ui_audit_tracker.json` and processes 1–3 screens at a time. Do NOT use for pure backend APIs, database migrations, CLI tools, or non-visual business logic.
---

# UI/UX Engineering

This skill turns UI/UX craft into repeatable engineering checks. It works in two modes—**Review & Fix Mode** (auditing existing screens in tracked batches of 1–3) and **Create Mode** (building new interfaces with zero AI-slop defaults)—backed by visual examples in `references/playbook.md` and distilled industry engineering rules in `references/external_skills_digest.md`.

---

## Mode Detection

- **Review & Fix Mode:** User asks to audit, review, critique, find flaws, or improve existing UI/screens/flows.
- **Create Mode:** User asks to design, mockup, or build a new screen, component, form, or page.

If both apply (e.g., "audit my app and upgrade it"), run **Review & Fix Mode** first, then apply **Create Mode** rules when building the fixes.

---

## Mode 1: Review & Fix Mode (Tracked Batch Workflow)

Reviewing an entire app in one pass produces shallow, generic feedback. Always work in **batches of 1 to 3 screens** and persist state so progress survives across sessions.

### Step 1: Discover & Sync `.ui_audit_tracker.json`
1. Check `<project_root>/.ui_audit_tracker.json`.
2. If it does not exist, scan the project's screens/pages/routes (e.g. `ARCHITECTURE.md`, `lib/screens/`, `src/pages/`, `app/`) and create `.ui_audit_tracker.json` with every screen initialized to `"status": "pending"`:
   ```json
   {
     "project": "<repo-name>",
     "updated_at": "YYYY-MM-DD",
     "screens": [
       {
         "id": 1,
         "name": "Home / Discovery",
         "path": "lib/screens/home_screen.dart",
         "status": "pending",
         "notes": ""
       }
     ]
   }
   ```
   Valid statuses: `pending` | `audited` | `planned` | `fixed`.

### Step 2: Present List & Ask User to Pick 1–3 Screens
Show a numbered summary grouped by status (`pending`, `audited`, `planned`, `fixed`) so the user immediately sees what is already done vs remaining. Ask the user to select **1, 2, or 3 screens max** for this batch (never run more than 3 screens at once).

*Exception:* If the user already named 1–3 specific files/screens in their prompt, skip asking and audit those directly.

### Step 3: Deep Audit Against the 5 Pillars
Read the source code (and any screenshots/mockups) of the selected 1–3 screens and inspect them against:

1. **10 Required UI States:** Empty (why + 1 next step), Loading (skeletons, no frozen spinner), Error (cause + whose fault + fix, preserve input), No Internet (cached content + reconnecting), Slow Network (real progress + lite fallback), No Search Results (typo fix + escape hatches), Permission Denied (why + Settings + fallback), Session Expired (save work first), Form Validation (inline fix on blur), Success (confirm + details + next step).
2. **24 UX & Psychology Laws:** Jakob's (familiar placement), Hick's (cut options), Miller's (chunk `4x4`), Fitts's (`48dp` thumb targets), Doherty (`<400ms` response / `100ms` click feedback), Tesler's (system auto-fills ZIP/city), Postel's (accept any format, normalize), Parkinson's (time estimate + autofill), Goal-Gradient (never start at 0%), Peak-End (warm finish), Zeigarnik (show remaining steps), Von Restorff (1 standout CTA), Serial Position (key items first/last), Closure (peek next card 32%), Figure-Ground (dim backdrop), Banner Blindness (style notices like content), Proximity (`8px` to own field vs `24px` to next), Similarity (tappable rows look tappable), Common Region (card border groups), Continuity, Connectedness (1 line connects flow steps), Choice Overload, Occam's Razor (remove until it breaks), Least Effort (1-tap path).
3. **Component Playbooks (`references/playbook.md` §10):** Check every Dropdown (`>10` = searchable, `<5` = segmented/radios), Filter (preserve stale list, chips above, option counts, URL state), Pagination (total count, 0px layout shift, reachable footer, restore scroll on Back), Date Picker (typeable + presets + echo in words), Form (validate on blur, green checks, all 6 states), Modal (3 exits: X/Esc/backdrop, focus trap, 1 layer only, dirty check), Upload (whole card dropzone, pre-drop validation, background tray), Settings (auto-save confirm, scope label, search, reset), Search (200ms debounce + abort, fuzzy ±2, recent on focus, arrow keys), Accessibility (`4.5:1` text / `3:1` UI, `:focus-visible`, 200% zoom reflow).
4. **6-Decision Polish Specs (`references/playbook.md` §11):** `8pt` spacing grid, 3 text tiers + 1 accent, concentric corners (`inner_radius = outer_radius - padding`), top-down light + downward shadow, `<250ms` ease-out motion (`transform` only).
5. **17 Vibe-Coded AI Tells & Slop Removal Test (`references/external_skills_digest.md` §5):** Flag decorative stacking (glow + glass + dot grids + radial orbs), generic 3-card rows, sparkle icons on every button, rainbow pastel cards, and ungrounded proof. Apply the **Removal Test**: if deleting an element improves clarity without losing state/hierarchy, remove it.

### Step 4: Output Structured Findings & Solutions
Present findings in a **Before / After / Law or Playbook / Fix** table ordered by severity (`P0` -> `P1` -> `P2`), referencing visual examples in `references/playbook.md` where helpful.

### Step 5: Update `.ui_audit_tracker.json`
After presenting the audit (status -> `audited`), creating mockups/plan (`planned`), or implementing code (`fixed`), update `.ui_audit_tracker.json` with the new status, date, and a 1-line note.

---

## Mode 2: Create Mode (New UI / Redesigns)

Before writing UI code for a new screen or component, enforce these non-negotiable engineering defaults:

1. **System & Hierarchy:** Declare 1 primary action per viewport, 3 text tiers (primary, secondary, muted), and 1 accent color (1–3% of screen).
2. **Layout & Geometry:** Use an `8pt` spacing grid (`8 / 16 / 24 / 32`). Enforce concentric radii (`inner_radius = outer_radius - padding`). Minimum tap target `48x48dp` (`44px` floor).
3. **Typography:** Pair a distinct display face with a readable body face; reserve monospace/tabular figures for numbers and metrics.
4. **All States Designed Upfront:** Every view ships with Empty, Loading (skeleton), Error (with retry + preserved input), Offline, and Success states. Every input ships with Default, Focus, Filled, Error, Success, and Disabled states.
5. **Motion & Performance:** Feedback within `100ms`, transitions `150–250ms` using custom `ease-out` (`cubic-bezier(0.23, 1, 0.32, 1)`), animate `transform`/`opacity` only (never `width`/`height`/`top`), and honor `prefers-reduced-motion`. Never animate actions triggered 100+ times/day (e.g., command palettes).
6. **Accessibility Floor:** `>= 4.5:1` body text contrast, `>= 3:1` large text/icon/border contrast, persistent labels above inputs (placeholders are hints only), visible focus rings, and 200% zoom reflow.

---

## Bundled References
- **Visual Playbook (207 screenshots):** Read `references/playbook.md` when you need concrete visual ❌ vs ✅ examples for any law, state, or component.
- **External Design Skills Digest:** Read `references/external_skills_digest.md` for motion curves, concentric radius recipes, anti-slop removal rules, and landing-page conversion structure.
