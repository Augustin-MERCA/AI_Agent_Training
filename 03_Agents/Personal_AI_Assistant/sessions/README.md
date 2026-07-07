# Memory Logs — 交接

這裡不是普通日記，而是一套**交接系統**：讓下一次 session（不管是你自己回來看，還是 AI 重新開始）能快速接上進度，不用重新翻聊天記錄。

| File / Folder | 用途 |
|---|---|
| `Latest_State.md` | 下次開場最快讀：上次做了什麼、下一步是什麼、急需注意什麼 |
| `MEMORY.md` | 長期記憶：偏好、紅線、重複修正、踩坑、重要決策 |
| `Daily_Summaries/` | 按日期保存每次 session 發生過什麼 |

Agent 專屬的交接紀錄不放在這裡，而是放在該 agent 自己的資料夾下，例如 `../agents/<agent_name>/sessions/`（見 `../agents/README.md`）。

## 使用方式
- 每次 session 結束前（或開始前先看）：更新 `Latest_State.md`，保持只放「現在最需要知道的事」，舊資訊移到 `Daily_Summaries/`
- 遇到重複犯的錯、踩過的坑、使用者明確要求的規則 → 記進 `MEMORY.md`，不要只留在某一天的摘要裡
- `Daily_Summaries/` 用 `YYYY-MM-DD.md` 命名，一天一份，記錄當天做了什麼、遇到什麼問題、怎麼解決的

## 注意
內容不得包含密碼、API key、私人資料、薪酬資料、員工紀錄或客戶紀錄（見 `../scope.md`）。此資料夾內容會被推送到 **public** GitHub repository。
