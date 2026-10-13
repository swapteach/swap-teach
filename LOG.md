# 變更與決策紀錄

最新的紀錄在最上面。格式見 [AGENTS.md](AGENTS.md#logmd)。只記錄有意義的變更；錯字等小修看 git 歷史即可。搜尋「**決策**」可找到所有決策。

---

## 2026-10-13 — 新增第一堂課逐字稿與重點整理

- **作者：** Antony
- **變更：** 在 `reference/` 新增第一堂課（2026-09-15）的語音轉文字逐字稿，並整理成 [docs/course/first-lecture.md](docs/course/first-lecture.md)。依老師的口頭說明更新評分與要求文件：解決「競賽 15% 或 20%」與「不到 0.01」兩個待確認項目；補充互評的三個面向（完整度、創意、可用性）、「屍體」規則、沒參加比賽最高 85 分、歷屆專題被打 X 的原因、APP 優先與先查有沒有人做過。AGENTS.md 中「`.txt` 不可作為依據」的規則改為只指 AI 生成的那份 `.txt`。
- **原因：** 投影片只有規則與 X 數，逐字稿有老師的解釋；這些資訊對選題很重要。
- **檔案：** `reference/2026-09-15-第一堂課逐字稿.txt`、`reference/README.md`、`docs/course/first-lecture.md`、`docs/course/grading.md`、`docs/course/requirements.md`、`docs/course/timeline.md`、`AGENTS.md`
- **決策：** 逐字稿可作為補充資料，但與官方投影片、課程大綱不一致時以官方為準。

## 2026-10-05 — 建立專案文件架構

- **作者：** Antony
- **變更：** 建立 repo 與文件架構：README、協作說明、AI 規則（AGENTS.md）、名詞表、本紀錄、課程要求與評分整理、專題概述、競賽資料、會議紀錄範本、ADR 說明，以及參考資料說明。
- **原因：** 讓全組有一個集中存放資料與文件的地方，在開始寫程式前先整理好。
- **檔案：** 全部
- **決策：**
  - 使用 GitHub 組織 `swapteach` 下的私人 repo，日後可能公開。
  - **中文是唯一的正式版本**；`en/` 是英文鏡像，只由 Antony 維護，其他人不用管。
  - 名詞表（CONTEXT.md）中英並列，作為翻譯用詞的依據。
  - 直接 push 到 `main`，不使用 Pull Request，不需要審核；由 AI 依 AGENTS.md 檢查一致性。
  - 只記錄有意義的變更；commit 訊息用英文。
  - 任務用 GitHub Issues + Projects，標題中英並列。
  - 專題概述以「教育AI組」版本為準；兩份已提交的概述文件保留為凍結版本。
  - 課程規定以官方投影片與課程大綱為準；`reference/` 中的 `.txt` 是非官方 AI 生成文件，不作為依據。
  - 每個人可在 `.local/`（不進版本控制）放個人筆記與 AI 對話紀錄。
