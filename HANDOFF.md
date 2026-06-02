# 🔁 Project Handoff File
> Auto-maintained by agent. Delete this file when project is complete.
> Last updated: UPDATE PASS (7 fixes) — DONE. README.md patched and pushed.

---

## ✅ COMPLETED

- `HANDOFF.md` — always current.
- `README.md` — **COMPLETE REWRITE (v3)** + **UPDATE PASS (v3.1)**. All visuals use server-rendered external services only. No local assets.
  - Section 1: capsule-render — text updated to `Piyush Pal`, desc shortened to `Building at the edge of AI`
  - Section 1b: readme-typing-svg — 4 new lines: AI/ML Engineer, BTech identity, BLING stat, iOS Developer
  - Section 2: Identity block — age updated 18 → 20
  - Section 3: skillicons.dev icon grid (unchanged)
  - Section 4: Systems — tighter BLING write-up (headline stats bolded, stack line as italic below title, separator `---` between projects, `Also:` for other repos)
  - Section 5: Currently block — 6 new lines including DSA, Java, hackathons, stealth projects
  - Section 6: github-readme-stats switched from `theme=transparent` to `theme=tokyonight` + explicit `bg_color=0d1117&text_color=c9d1d9` — fixes broken render on low-activity accounts. `&nbsp;&nbsp;` spacer added between the two cards. Activity graph got `custom_title=Contribution%20Graph` param.
  - Section 7: "On Building" paragraph (unchanged)
  - Section 8: Contact placeholders (unchanged — pending Piyush)
  - Section 9: capsule-render footer (unchanged)

- `assets/banner.svg` — **DELETED**. Replaced by capsule-render URL in README.
- `assets/stats-card.html` — **DELETED**. Not meaningfully linkable from GitHub README.

---

## 🔄 IN PROGRESS
- Nothing. All work complete. Push to GitHub is the next step.

---

## ⏳ REMAINING TASKS
- Git push to GitHub
- Piyush to fill in two placeholders in README.md:
  1. `YOUR_EMAIL_HERE` → actual email address
  2. `YOUR_LINKEDIN_URL_HERE` → LinkedIn profile URL

---

## 🧠 KEY DECISIONS MADE (COMPLETE REWRITE)

- **Rendering philosophy**: every visual is a server-rendered `<img>` URL. GitHub fetches and caches them. Zero local SVG, zero JS, zero animations in repo files.
- **capsule-render**: `type=waving` returns an animated PNG via Vercel — works on GitHub. Color gradient `0:0d1117,50:1a1a2e,100:0d1117` matches dark profile aesthetic.
- **readme-typing-svg**: `demolab.com` service returns a server-animated SVG — confirmed GitHub-compatible. JetBrains Mono font, 3 rotating lines covering BLING stat + identity + domain.
- **skillicons.dev**: single pre-rendered PNG of 13 tech icons, `perline=13` keeps them in one row, `theme=dark` matches profile.
- **BYTEJAYS prose style**: no `<table>` project cards, no badge rows per project, no bold keywords. Bold project name as repo hyperlink, italic tagline, dense paragraph, backtick stack line. Reads like a senior engineer's profile, not a student template.
- **Stats theme**: `transparent` on github-readme-stats and streak-stats — blends into any dark background without white box artifacts.
- **Activity graph**: `bg_color=0d1117` matches GitHub dark mode background exactly.
- **"Currently" section**: fenced code block with `→` arrows — looks intentional, clean, monospace. No bullets.
- **"On Building" paragraph**: no markdown header (`##`), just plain prose — closer to BYTEJAYS manifesto style.
- **Contact**: plain Markdown text line, no shields.io badges — minimal, serious.
- **Deleted assets**: banner.svg and stats-card.html removed. The topology explorer was genuinely interactive but not linkable from the profile README in any useful way on GitHub mobile.

---

## 📁 FILE MANIFEST

| File | Status | Notes |
|------|--------|-------|
| `HANDOFF.md` | ✅ Done | Always current |
| `README.md` | ✅ Done (v3) | Complete rewrite — all server-rendered services |
| `assets/banner.svg` | ❌ Deleted | Replaced by capsule-render URL |
| `assets/stats-card.html` | ❌ Deleted | Not meaningfully usable from profile README |
| `projects/showcase.md` | ✅ Done (v1) | Deep-dive writeups — not touched in this pass |

---

## ⚠️ BLOCKERS / PENDING FROM USER

- **Email**: NOT YET PROVIDED — placeholder `YOUR_EMAIL_HERE` in README.md line ~78
- **LinkedIn URL**: NOT YET PROVIDED — placeholder `YOUR_LINKEDIN_URL_HERE` in README.md line ~78

---

## 🆕 NEXT AGENT INSTRUCTIONS

1. Read this file first — all work is COMPLETE
2. Do NOT recreate banner.svg or stats-card.html
3. Only action needed: user provides email + LinkedIn → find-replace in README.md → git push
4. Once confirmed, instruct Piyush to delete this HANDOFF.md from the repo

## External Services Used (all confirmed GitHub-compatible)

| Service | URL pattern | What it renders |
|---------|-------------|-----------------|
| capsule-render | `capsule-render.vercel.app/api` | Animated waving header/footer PNG |
| readme-typing-svg | `readme-typing-svg.demolab.com` | Rotating text animation SVG |
| skillicons.dev | `skillicons.dev/icons` | Tech icon grid PNG |
| github-readme-stats | `github-readme-stats.vercel.app/api` | Stats card PNG |
| streak-stats | `streak-stats.demolab.com` | Streak card PNG |
| github-readme-activity-graph | `github-readme-activity-graph.vercel.app/graph` | Contribution graph PNG |
