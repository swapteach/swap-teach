# 協作說明

這份文件說明如何在這個 repo 裡新增與修改資料。給 AI 的完整規則在 [AGENTS.md](AGENTS.md)。

## 規則摘要

1. **中文為準。** 所有文件用繁體中文寫。
2. **不要動 `en/`。** 那是 Antony 的英文鏡像，他會自己同步。
3. **用 [CONTEXT.md](CONTEXT.md) 裡的名詞。** 例如寫「時間幣」，不要寫「點數」。
4. **一處改，處處改。** 改了一個地方，要檢查其他文件有沒有提到同一件事。
5. **不要改原始檔。** `reference/` 與 `docs/competition/submissions/` 只能看、不能改。
6. **重要的變更寫進 [LOG.md](LOG.md)**（錯字不用）。
7. **直接 push 到 `main`**，不需要開 Pull Request。

## 怎麼編輯（由推薦到不推薦）

### 1. 電腦上的 AI 工具（推薦）

把 repo 下載到電腦，用能讀整個資料夾的 AI 工具，例如 Claude Code、Cursor、Codex、VS Code 的 Copilot。這些工具會**自動讀取 [AGENTS.md](AGENTS.md)**，自己遵守上面的規則，包括更新相關文件、寫 LOG、commit 與 push。

```bash
git clone https://github.com/swapteach/swap-teach.git
```

### 2. GitHub 網頁直接編輯

小修改可以直接在 GitHub 網頁上改：打開檔案 → 右上角鉛筆圖示 → 修改 → Commit changes。這種方式沒有 AI 幫你檢查，記得自己更新 LOG.md 與相關文件。

### 3. 網頁版 AI（ChatGPT、Claude 網頁版等）

網頁版 AI **看不到這個 repo 的規則**。請在對話一開始貼上以下提示詞，並把相關檔案的內容一起貼上：

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

## 會議紀錄

複製 [docs/meetings/_template.md](docs/meetings/_template.md)，存成 `docs/meetings/YYYY-MM-DD.md`。會議中做的決定也要寫進 LOG.md。

## 任務與進度

用 GitHub Issues 記錄任務，並放到 GitHub Projects 看板上。標題中英並列，例如：`整理 20 萬筆公開資料來源 / Find 200k-record open data source`。

## 個人筆記（`.local/`）

`.local/` 資料夾不會被 commit，每個人可以放自己的筆記。如果你建立 `.local/session-log.md`，AI 工具會在每次開始時讀它、結束時更新它，方便你換一個對話後接續之前的工作。

## 英文鏡像（`en/`）

`en/` 是所有文件的英文翻譯，由 Antony 的 AI 從中文版同步過去。英文版可能會比中文版晚一點更新，**以中文版為準**。
