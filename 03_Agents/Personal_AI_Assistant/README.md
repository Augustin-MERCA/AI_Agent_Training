# Personal AI Assistant

這是 `AI_Agent_Training` 培訓中的第一個 agent。

## 目的
在安全、範圍受限的環境下，練習與 AI agent 協作，並建立清楚的規則與紀錄習慣。

## 這個資料夾在整體工作區的位置
Inbox / Action Center / Knowledge Base / Memory Logs 現在是**整個工作區共用**的角色，放在 `AI_Agent_Training/` 根目錄（見根目錄 `README.md` 與 `Folder_Routing_Map.md`）。這個資料夾本身只是 `03_Agents/` 底下**其中一個 agent 的本體**，內容包括：

| 內容 | 用途 |
|---|---|
| `scope.md` | 這個 agent 的使用範圍與安全規則 |
| `sessions/` | 這個 agent**自己專屬**的交接紀錄（跟工作區整體的 `../../04_Memory_Logs/` 分開） |

## 資料夾結構
```
Personal_AI_Assistant/
├── README.md            本檔案
├── scope.md              使用範圍與安全規則（重要，請先閱讀）
└── sessions/             這個 agent 專屬的記憶交接
    ├── Latest_State.md
    ├── MEMORY.md
    └── Daily_Summaries/
```

## 使用前必讀
請先閱讀 [scope.md](./scope.md)，了解哪些是工具內建機制、哪些是本專案額外要求 AI 遵守的規則。
