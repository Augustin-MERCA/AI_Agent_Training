# Agents — 做事

定義實際執行任務的 agent：各自的角色、範圍、可用工具、輸入輸出格式。

## 使用方式
- 每個 agent 一個檔案，例如 `research_agent.md`、`summarizer_agent.md`
- 內容建議包含：這個 agent 負責什麼、不負責什麼、會參考 `../knowledge_base/` 的哪些資料、完成後如何回報到 `../action_center/`
- Agent 的行為規則仍須遵守 `../scope.md` 的安全規則（高風險指令先問、不處理敏感資料等）

## 注意
內容不得包含密碼、API key、私人資料、薪酬資料、員工紀錄或客戶紀錄（見 `../scope.md`）。
