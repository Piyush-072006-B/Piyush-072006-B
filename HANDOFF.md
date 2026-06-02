# 🔁 Project Handoff File
> Auto-maintained by agent. Delete this file when project is complete.
> Last updated: DIVIDER PASS — DONE. 10 `---` dividers replaced with capsule-render gradient bars.

---

## ✅ COMPLETED

- `HANDOFF.md` — always current.
- `README.md` — **v3.3 (divider pass)**. 10 standalone `---` dividers replaced with `capsule-render type=rect` gradient bars (`0d1117 → 4c1d95 → 6d28d9 → 4c1d95 → 0d1117`, height=2). Fenced code block interior untouched. All 10 were decorative — none were structural.
  - Fix 1: Typing SVG trimmed to 2 lines (`AI/ML Engineer in the Making` + `B.Tech CSE (AI/ML) • Building Real Systems`). BLING + iOS lines removed.
  - Fix 2: Broken `github-readme-stats.vercel.app` cards DELETED. Replaced with `github-profile-summary-cards.vercel.app` (`profile-details`, `repos-per-language`, `most-commit-language`) — more reliable renderer for low-activity accounts.
  - Fix 3: Plain text contact line REPLACED with three shields.io badge-image links. Email and LinkedIn **fully resolved** — no more placeholders.
    - Email: piyush34305@gmail.com
    - LinkedIn: https://www.linkedin.com/in/piyush-pal-pp034305
  - Fix 4: MoodNest description expanded to 7 lines — covers daily logging, pattern tracking, no third-party deps, ships on iOS, design philosophy (not too clinical, not too cluttered).
  - Fix 5: skillicons.dev updated — `java,cpp` added after `swift`, `perline=13` → `perline=15`.

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

- **Email**: ✅ RESOLVED — `piyush34305@gmail.com` (filled in as badge image)
- **LinkedIn**: ✅ RESOLVED — `https://www.linkedin.com/in/piyush-pal-pp034305` (filled in as badge image)
- **HANDOFF.md**: Ready to be deleted by Piyush once he confirms the profile looks correct.

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
