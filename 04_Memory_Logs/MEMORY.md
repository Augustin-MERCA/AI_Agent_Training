# Memory（工作區整體）

## 偏好
- 每次檔案變更後，自動 `git add` → `commit` → `push`
- Folder 結構變更：Agent 可以建議，但 `move`／`rename`／`delete`／`overwrite` 一律要先問過使用者才能執行；新增全新檔案／資料夾不受限

## 紅線（絕對不能做）
- 不得要求或記錄：密碼、API key、私人資料、薪酬資料、員工紀錄、客戶紀錄
- 不得自動執行高風險指令（delete、force、admin 權限、credential 相關）——一律先解釋再等確認
- 此 repository 為 **public**，任何 commit 前都要留意內容是否洩漏敏感資訊

## 重複修正
（目前尚無）

## 踩坑紀錄
- PowerShell 每次工具呼叫是獨立 session，`git`/`gh` 用之前要重新載入 PATH
- winget 安裝互動視窗在非互動環境會被判定取消，改用 `--silent` + 背景執行

## 重要決策
- 2026-07-07：採用 Folder Routing Map，把 Inbox / Action Center / Knowledge Base / Memory Logs 提升到工作區根目錄，`03_Agents/` 底下放各個 agent 本體（目前只有 Personal_AI_Assistant）
