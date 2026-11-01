# AGENTS.md: Capstone_Project_ProcessFlow (TUP Thesis & Capstone Roadmap)

> Instructions for any AI agent (Claude Code, Codex, Gemini, Copilot, OpenCode…) working in this repo.
> Owner: Madz Amador. House rules: `~/.claude/skills/dev-playbook/SKILL.md`; global agent rules: `~/Documents/KnowledgeGraph/AGENTS.md`. This file overrides them where they differ.

## 1. What this is
An interactive guide for TUP Manila College of Science BSIS students doing their research, thesis and capstone projects: phase-by-phase instructions from topic selection to the final hardbound copy, document format samples (cover page, approval sheet, table of contents, acknowledgement, hardbound front), and Chart.js visuals of task distribution and quality thresholds such as the similarity-index limit. See [README.md](README.md).

## 2. Stack & commands
- Stack A: `index.html` + `styles.css` + `script.js`, Tailwind/Chart.js/Font Awesome from CDNs. No build, no tests.
- Run: open `index.html`, or `npx serve .`
- Verify: switch through every phase (sidebar on desktop, bottom bar on phone), open every sample image in the modal, check the charts; light/dark if present; phone width down to 344px.
- Deploy: GitHub Pages (README "Deployment to GitHub Pages").

## 3. Project memory
- `implementation_plan.md` (backlog) and `walkthrough.md` (dated log): create them on first change; add a walkthrough entry after every change.
- Work on `develop`, never directly on `main`. The old `agents/can-you-help-me-to-organize-the-code` branch is a past agent's branch; leave it alone unless the owner asks.

## 4. Domain rules (non-negotiable)
1. Requirements, deadlines and thresholds are the college's official rules; change them only from a source the owner gives, and say which in the commit.
2. Sample pages in `assets/` are the official formats; replace them, don't edit them.

## 5. Key files
- `index.html`: page structure and phase content; `script.js`: phase navigation, image modal (with loading spinner and missing-image fallback), charts; `styles.css`.
- `assets/`: logos (TUP, COS, CHED) and the sample document images.

## 6. Gotchas specific to this repo
- The README's project structure is out of date: it says everything is in `index.html` and lists asset names (`cover-page.jpg`, `approval-sheet.jpg`) that are now `coverPage.jpg`, `approvalSheet.jpg`, etc. Fix it when you touch structure.
- No `.gitignore`: `.DS_Store` has been committed before. Add one before committing other changes.

## 7. Before you finish
- [ ] Every phase and image checked on desktop and phone width
- [ ] `walkthrough.md` updated; commit on `develop` with a body that explains why
