<!-- mirror-of: CONTRIBUTING.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [CONTRIBUTING.md](../CONTRIBUTING.md). The Chinese version is authoritative.

# Contributing

How to add and change things in this repo. The full rules for AI tools are in [AGENTS.md](AGENTS.md).

## Rules in short

1. **Chinese is authoritative.** Every doc is written in Traditional Chinese.
2. **Don't touch `en/`.** It's Antony's English mirror; he keeps it in sync himself.
3. **Use the terms in [CONTEXT.md](../CONTEXT.md).** E.g. write 時間幣 (Time Coin), not 點數 (points).
4. **Change it once, change it everywhere.** When you change something, check whether other docs mention the same thing.
5. **Don't edit originals.** `reference/` and `docs/competition/submissions/` are read-only.
6. **Log meaningful changes in [LOG.md](LOG.md)** (not typos).
7. **Push straight to `main`.** No pull requests.

## How to edit (most to least recommended)

### 1. An AI tool on your computer (recommended)

Clone the repo and use an AI tool that can read the whole folder, e.g. Claude Code, Cursor, Codex, or Copilot in VS Code. These **read [AGENTS.md](AGENTS.md) automatically** and follow the rules above on their own: updating related docs, writing the log, committing and pushing.

```bash
git clone https://github.com/swapteach/swap-teach.git
```

### 2. Editing on the GitHub website

Small edits can be made directly on GitHub: open the file → pencil icon (top right) → edit → Commit changes. No AI checks anything this way, so update LOG.md and related docs yourself.

### 3. Browser AI chats (ChatGPT, Claude on the web, etc.)

Browser AI chats **can't see this repo's rules**. Paste the prompt below at the start of the chat, together with the contents of the relevant files. (The prompt is in Chinese because it tells the AI to write Chinese.)

```text
你正在協助我修改「換你教 SwapTeach」專題 repo 中的文件。請遵守以下規則：
1. 所有文件用繁體中文（台灣用語）撰寫。
2. 專有名詞使用我提供的 CONTEXT.md 中的用詞。
3. 修改後，告訴我還有哪些文件可能提到同一件事、需要一起修改。
4. 若資訊不確定或互相矛盾，不要自己猜，標記「⚠️ 待確認」。
5. 最後幫我寫一筆 LOG.md 紀錄，格式：
   ## YYYY-MM-DD — 標題
   - **作者：** / **變更：** / **原因：** / **檔案：** / **決策：**
```

Translation: "You're helping me edit docs in the SwapTeach project repo. Rules: 1. Write in Traditional Chinese (Taiwan). 2. Use the terms in the CONTEXT.md I provide. 3. After editing, tell me which other docs may mention the same thing and need updating. 4. If information is uncertain or contradictory, don't guess; mark it ⚠️ 待確認. 5. Finally, write a LOG.md entry in this format: …"

## Meeting notes

Copy [docs/meetings/_template.md](docs/meetings/_template.md) to `docs/meetings/YYYY-MM-DD.md`. Decisions made in the meeting also go into LOG.md.

## Tasks and progress

Track tasks as GitHub Issues on a GitHub Projects board. Titles are bilingual, e.g. `整理 20 萬筆公開資料來源 / Find 200k-record open data source`.

## Personal notes (`.local/`)

The `.local/` folder is never committed; everyone can keep their own notes there. If you create `.local/session-log.md`, AI tools read it at the start of each session and update it at the end, so you can pick up where you left off in a new chat.

## English mirror (`en/`)

`en/` holds English translations of every doc, synced from the Chinese by Antony's AI. It may lag slightly behind; **the Chinese version is authoritative**.
