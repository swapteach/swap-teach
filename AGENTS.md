# AI 協作規則

本檔是給 AI 工具（Claude Code、Codex、Cursor、Copilot 等）的規則。人類版說明見 [CONTRIBUTING.md](CONTRIBUTING.md)。

使用者可能不會每次都提醒你這些規則，**請你主動遵守**。

## 專案背景

- 本 repo 是「換你教 SwapTeach」的專題資料夾，目前只有文件，尚未有程式碼。專案概述見 [docs/project/overview.md](docs/project/overview.md)。
- 組員主要使用繁體中文，其中一位組員（Antony）使用英文。

## 語言

1. 所有文件以**繁體中文（台灣用語）**撰寫。中文是唯一的正式版本。
2. 使用者用英文跟你溝通時，照樣把內容以中文寫進文件。
3. **不要修改 `en/` 資料夾**，也不要把它當作資料來源。那是英文鏡像，由 Antony 另外維護。搜尋與更新時一律略過 `en/`。
4. 專有名詞一律使用 [CONTEXT.md](CONTEXT.md) 中的用詞，避免「_避免_」列出的說法。出現新的專有名詞時，把它加進 CONTEXT.md（中文與英文都要填）。

## 開始工作前

1. 執行 `git pull --rebase`，取得最新版本。
2. 讀 [CONTEXT.md](CONTEXT.md)。
3. 若 `.local/session-log.md` 存在，讀它，以接續使用者上一次的工作。

## 修改文件時

1. **一處改，處處改。** 改完一個文件後，搜尋整個 repo（略過 `en/`）中所有相關內容並一起更新，避免文件互相矛盾。例如：改了某個功能 → 檢查 `docs/project/`、`CONTEXT.md`、`docs/course/` 中的要求對照。
2. 不可修改 `reference/` 中的原始檔，也不可修改 `docs/competition/submissions/`（已提交的凍結版本）。
3. 課程規定以 `reference/` 中的官方投影片 PDF 與課程大綱 PDF 為準。`reference/` 中的 `.txt` 是非官方、AI 生成的文件，**不可作為依據**。
4. 發現文件之間有矛盾或資訊不確定時，不要自己猜：在文件中標記「⚠️ 待確認」，並告訴使用者。
5. 重大且難以逆轉的決策，在 `docs/adr/` 新增一份 ADR（格式見 [docs/adr/README.md](docs/adr/README.md)），並在 LOG.md 連結它。

## LOG.md

有意義的變更（新增或修改文件內容、決策、範圍變更、會議決議）都要在 [LOG.md](LOG.md) **最上方**新增一筆。錯字、排版等小修不用記。格式：

```markdown
## YYYY-MM-DD — 標題

- **作者：** 姓名
- **變更：** 改了什麼
- **原因：** 為什麼改
- **檔案：** 相關檔案
- **決策：** （若有）做了什麼決定
```

## 會議紀錄

放在 `docs/meetings/YYYY-MM-DD.md`，複製 [docs/meetings/_template.md](docs/meetings/_template.md) 開始。會議中的決策也要寫進 LOG.md 與相關文件。

## GitHub Issues

標題格式：`中文標題 / English title`。

## 結束工作前

1. Commit：訊息用**英文**，簡短（例：`docs: add course grading rules`）。
2. 先 `git pull --rebase` 再 `git push` 到 `main`（不開 Pull Request）。遇到衝突時小心合併，**絕不覆蓋別人的內容**；不確定就問使用者。
3. 若 `.local/session-log.md` 存在，在最上方記錄：日期、做了什麼、還沒完成的事、下一步。`.local/` 不會被 commit。
