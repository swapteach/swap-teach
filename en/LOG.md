<!-- mirror-of: LOG.md @ 9f3e7e261689eea75be74350c9b6f782faa2996e -->
> 🌐 English mirror of [LOG.md](../LOG.md). The Chinese version is authoritative.

# Change and decision log

Newest entries at the top. Format in [AGENTS.md](AGENTS.md#logmd). Only meaningful changes are logged; see git history for small fixes. Search for "**決策**" (Decision) to find every decision.

---

## 2026-10-13 — Add first-lecture transcript and summary

- **Author:** Antony
- **Change:** Added the speech-to-text transcript of the first lecture (2026-09-15) to `reference/` and summarized it in [docs/course/first-lecture.md](docs/course/first-lecture.md). Updated the grading and requirements docs from the professor's spoken explanations: resolved the "competition 15% or 20%" and "below 0.01" open items; added the three peer-review criteria (completeness, creativity, usability), the "corpse" rule, the 85-point cap without a competition, the reasons past projects got X marks, the app-first preference, and checking for prior work. Narrowed the AGENTS.md rule "`.txt` files are not a source" to the AI-generated `.txt` only.
- **Why:** The slides only have rules and X counts; the transcript has the professor's explanations, which matter for choosing a topic.
- **Files:** `reference/2026-09-15-第一堂課逐字稿.txt`, `reference/README.md`, `docs/course/first-lecture.md`, `docs/course/grading.md`, `docs/course/requirements.md`, `docs/course/timeline.md`, `AGENTS.md`
- **Decision:** The transcript can be used as supplementary material, but the official slides and syllabus win wherever they disagree.

## 2026-10-05 — Set up project documentation structure

- **Author:** Antony
- **Change:** Created the repo and doc structure: README, contributing guide, AI rules (AGENTS.md), glossary, this log, course requirements and grading summaries, project overview, competition info, meeting template, ADR guide, and a guide to the reference files.
- **Reason:** Give the whole team one place for information and docs, organized before any code is written.
- **Files:** all
- **Decisions:**
  - Private repo under the GitHub organization `swapteach`; may go public later.
  - **Chinese is the only authoritative version**; `en/` is an English mirror maintained only by Antony. Nobody else needs to touch it.
  - The glossary (CONTEXT.md) is bilingual and is the reference for translated terms.
  - Push straight to `main`; no pull requests or approvals. AI tools check consistency per AGENTS.md.
  - Log only meaningful changes; commit messages in English.
  - Tasks in GitHub Issues + Projects, titles in both languages.
  - The project overview is based on the 教育AI組 (Education AI track) version; both submitted overviews are kept as frozen copies.
  - Course rules come from the official slides and syllabus; the `.txt` in `reference/` is an unofficial AI-generated doc and is not relied on.
  - Everyone may keep personal notes and AI chat logs in `.local/` (not version-controlled).
