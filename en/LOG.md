<!-- mirror-of: LOG.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [LOG.md](../LOG.md). The Chinese version is authoritative.

# Change and decision log

Newest entries at the top. Format in [AGENTS.md](AGENTS.md#logmd). Only meaningful changes are logged; see git history for small fixes. Search for "**決策**" (Decision) to find every decision.

---

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
