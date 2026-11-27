# UI/UX Engineering Skill

An **independent, open-source AI agent skill** for auditing existing interfaces and designing production-grade UI/UX—grounded in **200+ visual examples**, **24 UX/psychology laws**, **15 component engineering playbooks**, **WCAG accessibility standards**, and **anti-AI-slop rules**.

Works with **Antigravity**, **Claude Code**, **Cursor**, **Windsurf**, and any agent supporting the `SKILL.md` standard.

---

## Why This Skill Exists

Most AI-generated UIs fail in two predictable ways:
1. They look like generic "vibe-coded" templates (purple gradients, bento grids everywhere, sparkle icons, zero hierarchy).
2. They only design the "happy path"—forgetting empty states, slow networks, blur validation, keyboard navigation, focus traps, and layout shifts.

`ui-ux-engineering` fixes both by giving your AI agent **concrete engineering thresholds** (`<250ms` ease-out motion, `8pt` spacing grids, `48dp` touch targets, `4.5:1` contrast, `inner_radius = outer_radius - padding`) paired with **207 side-by-side visual screenshots**.

---

## Key Features

- **Dual-Mode Architecture:**
  - **Review & Fix Mode:** Audits existing codebases in **tracked batches of 1–3 screens** using `.ui_audit_tracker.json` (`pending` / `audited` / `planned` / `fixed`), so large apps are upgraded systematically without context overload.
  - **Create Mode:** Enforces non-negotiable UI/UX defaults when building new screens, forms, modals, dashboards, or landing pages.
- **10 Mandatory UI States:** Empty, Loading (skeletons), Error, No Internet, Slow Network, No Search Results, Permission Denied, Session Expired, Form Validation, Success.
- **24 UX & Psychology Laws:** Fitts's, Hick's, Miller's, Jakob's, Doherty Threshold (`<400ms`), Tesler's, Postel's, Parkinson's, Goal-Gradient, Peak-End, Zeigarnik, Von Restorff, Serial Position, Closure, Figure-Ground, Banner Blindness, Proximity, Similarity, Common Region, Continuity, Connectedness, Choice Overload, Occam's Razor, Principle of Least Effort.
- **15 Component Engineering Playbooks:** Dropdowns, Animation/Motion, Loading, Navigation, Settings, File Uploads, Filters, Date Pickers, Form Validation, Pagination, Error States, Onboarding, Search, Modals/Dialogs, Accessibility.
- **6-Decision Polish Specs:** Exact pixel spacing, concentric corner radius math, 3 text tiers + 1 accent, top-down lighting, and `100ms`/`300ms` interaction choreography.
- **Zero External Dependencies:** Includes 207 visual reference screenshots and a distilled digest of 6 top community design-engineering skill repos.

---

## Installation

### Antigravity / Global Agent Skills
```bash
git clone https://github.com/<your-github-username>/ui-ux-engineering.git ~/.gemini/config/skills/ui-ux-engineering
```

### Claude Code
```bash
git clone https://github.com/<your-github-username>/ui-ux-engineering.git ~/.claude/skills/ui-ux-engineering
```

### Project-Local (Cursor / Windsurf / Repo)
```bash
git clone https://github.com/<your-github-username>/ui-ux-engineering.git .agents/skills/ui-ux-engineering
```

---

## Usage

- **Audit an existing app (Batch Mode):**
  > *"Use `ui-ux-engineering` to audit my app screens."*  
  The agent scans your project, creates/reads `.ui_audit_tracker.json`, lists all screens with their status, and asks you to pick **1–3 screens** to audit and fix.
- **Review a single screen or component:**
  > *"Review `LoginScreen` using `ui-ux-engineering`."*
- **Build new UI:**
  > *"Design a new pricing table / checkout form / dashboard following `ui-ux-engineering`."*

---

## Repository Structure

```text
ui-ux-engineering/
├── SKILL.md                          # Core dual-mode agent instructions
├── README.md                         # Documentation & installation guide
├── LICENSE                           # MIT License
├── CONTRIBUTING.md                   # Contribution guidelines
└── references/
    ├── playbook.md                   # Complete visual playbook (207 inline screenshots)
    ├── external_skills_digest.md     # Distilled rules from 6 open-source design repos
    └── screenshots/                  # 207 side-by-side UI/UX reference images
```

---

## Credits & Sources
- Visual UI/UX rules & screenshots compiled from **Strategy Fox** (`strategyfox.in`) and **`@motion_ui_interface`**.
- External design-engineering principles distilled from `emilkowalski/skills`, `jakubkrehel/skills`, `ConardLi/garden-skills`, `elayadesign/ai-design-skills`, `MengTo/Skills`, and `Owl-Listener/designer-skills`.

---

## Recommended GitHub Topics (SEO)
`ui-ux` · `design-system` · `ai-agent-skill` · `claude-skills` · `ux-laws` · `frontend-engineering` · `accessibility` · `micro-interactions` · `design-engineering`
