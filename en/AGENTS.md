<!-- mirror-of: AGENTS.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [AGENTS.md](../AGENTS.md). The Chinese version is authoritative and is the one AI tools actually read.

# AI collaboration rules

These rules are for AI tools (Claude Code, Codex, Cursor, Copilot, etc.). The human-readable version is [CONTRIBUTING.md](CONTRIBUTING.md).

Users may not remind you of these rules every time. **Follow them on your own.**

## Background

- This repo is the project folder for SwapTeach 換你教. It holds only docs so far, no code. See [docs/project/overview.md](docs/project/overview.md).
- Team members mainly use Traditional Chinese; one member (Antony) uses English.

## Language

1. Write every doc in **Traditional Chinese (Taiwan usage)**. Chinese is the only authoritative version.
2. When a user talks to you in English, still write the content into the docs in Chinese.
3. **Do not modify the `en/` folder** and do not use it as a source. It is an English mirror maintained separately by Antony. Skip `en/` when searching and updating.
4. Use the terms in [CONTEXT.md](../CONTEXT.md) and avoid the ones listed under _Avoid_. When a new project-specific term comes up, add it to CONTEXT.md (in both Chinese and English).

## Before starting work

1. Run `git pull --rebase` to get the latest version.
2. Read [CONTEXT.md](../CONTEXT.md).
3. If `.local/session-log.md` exists, read it to continue the user's previous work.

## When editing docs

1. **Change it once, change it everywhere.** After editing a doc, search the whole repo (skipping `en/`) for related content and update it too, so docs never contradict each other. E.g. if a feature changes, check `docs/project/`, `CONTEXT.md`, and the requirements table in `docs/course/`.
2. Never modify the original files in `reference/` or anything in `docs/competition/submissions/` (frozen as submitted).
3. Course rules come from the official slides PDF and the syllabus PDF in `reference/`. The `.txt` in `reference/` is unofficial and AI-generated; **never rely on it**.
4. If docs contradict each other or information is uncertain, don't guess: mark it "⚠️ 待確認" (to be confirmed) in the doc and tell the user.
5. For a major, hard-to-reverse decision, add an ADR in `docs/adr/` (format in [docs/adr/README.md](docs/adr/README.md)) and link it from LOG.md.

## LOG.md

Every meaningful change (doc content added or changed, decisions, scope changes, meeting decisions) gets an entry at the **top** of [LOG.md](LOG.md). Typos and formatting don't. Format:

```markdown
## YYYY-MM-DD — Title

- **作者 (Author):** name
- **變更 (Change):** what changed
- **原因 (Reason):** why
- **檔案 (Files):** files involved
- **決策 (Decision):** (if any) what was decided
```

## Meeting notes

Go in `docs/meetings/YYYY-MM-DD.md`, starting from a copy of [docs/meetings/_template.md](docs/meetings/_template.md). Decisions made in meetings also go into LOG.md and the relevant docs.

## GitHub Issues

Title format: `中文標題 / English title`.

## Before finishing

1. Commit with a short **English** message (e.g. `docs: add course grading rules`).
2. `git pull --rebase`, then `git push` to `main` (no pull requests). Merge conflicts carefully and **never overwrite other people's work**; ask the user if unsure.
3. If `.local/session-log.md` exists, add an entry at the top: date, what was done, what's unfinished, next steps. `.local/` is never committed.
