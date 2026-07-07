# Personal AI Assistant

這是 `AI_Agent_Training` 培訓中的第一個實作專案：一個 Personal AI Assistant。

## 目的
在安全、範圍受限的環境下，練習與 AI agent 協作，並建立清楚的規則與紀錄習慣。

## 架構：五個角色
這個 assistant 依照以下五個角色分工：

| 角色 | 資料夾 | 功能 |
|---|---|---|
| Inbox 收集 | `inbox/` | 暫存尚未處理的想法、任務、請求 |
| Action Center 推進 | `action_center/` | 追蹤任務狀態，把事情往前推 |
| Knowledge Base 餵資料 | `knowledge_base/` | 提供 Agents 執行時參考的穩定資料 |
| Agents 做事 | `agents/` | 定義實際執行任務的 agent |
| Memory Logs 交接 | `sessions/` | 交接系統：`Latest_State.md`（下次開場最快讀）、`MEMORY.md`（長期記憶）、`Daily_Summaries/`（按日紀錄） |

## 資料夾結構
```
Personal_AI_Assistant/
├── README.md            本檔案
├── scope.md              使用範圍與安全規則（重要，請先閱讀）
├── inbox/                收集
├── action_center/        推進
├── knowledge_base/       餵資料
├── agents/               做事（每個 agent 未來會有自己的 sessions/ 交接紀錄）
└── sessions/             記憶交接（專案整體）
    ├── Latest_State.md
    ├── MEMORY.md
    └── Daily_Summaries/
```

## 使用前必讀
請先閱讀 [scope.md](./scope.md)，了解哪些是工具內建機制、哪些是本專案額外要求 AI 遵守的規則。
