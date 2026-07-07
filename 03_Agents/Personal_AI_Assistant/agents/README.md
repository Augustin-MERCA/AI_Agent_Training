# Agents — 做事

定義實際執行任務的 agent：各自的角色、範圍、可用工具、輸入輸出格式。

## 使用方式
- 每個 agent 一個資料夾，例如 `agents/research_agent/`
- 內容建議包含：這個 agent 負責什麼、不負責什麼、會參考 `../knowledge_base/` 的哪些資料、完成後如何回報到 `../action_center/`
- Agent 的行為規則仍須遵守 `../scope.md` 的安全規則（高風險指令先問、不處理敏感資料等）

## 每個 agent 自己的交接紀錄
每個 agent 資料夾底下可以有自己的 `sessions/`，用來記錄**這個 agent 專屬**的執行交接紀錄（跟 `../sessions/` 整體專案的 Memory Logs 分開）：

```
agents/
└── research_agent/
    ├── README.md          這個 agent 的定義
    └── sessions/
        ├── Latest_State.md
        └── Daily_Summaries/
```

目前還沒有任何 agent，等第一個 agent 定義出來時再建立對應資料夾。

## 注意
內容不得包含密碼、API key、私人資料、薪酬資料、員工紀錄或客戶紀錄（見 `../scope.md`）。
