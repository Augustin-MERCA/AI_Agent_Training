# Personal AI Assistant（Audrey Ines）

這是 `AI_Agent_Training` 培訓中的第一個 agent，名字是 **Audrey Ines**。

## 目的
在安全、範圍受限的環境下，練習與 AI agent 協作，並建立清楚的規則與紀錄習慣。

## 這個資料夾在整體工作區的位置
Inbox / Action Center / Knowledge Base / Memory Logs 現在是**整個工作區共用**的角色，放在 `AI_Agent_Training/` 根目錄（見根目錄 `README.md` 與 `Folder_Routing_Map.md`）。這個資料夾本身只是 `03_Agents/` 底下**其中一個 agent 的本體**。

## Agent Profile（8 件套）
Hiring Brief 已拆解成以下 8 份檔案，方便個別更新、個別引用：

| 檔案 | 內容 |
|---|---|
| `AGENTS.md` | 她是誰、扮演什麼角色（Name + Role） |
| `SOUL.md` | 個性、溝通風格、行為界線（Tone + Boundaries） |
| `TOOLS.md` | 可用工具與不可授權的權限 |
| `BRAIN.md` | 決策邏輯（什麼事自己處理、什麼事要先問） |
| `MEMORY.md` | 她自己的偏好、紅線、常見修正（跟 `sessions/MEMORY.md` 不同，見該檔案開頭說明） |
| `HEARTBEAT.md` | 每日開始／結束的固定流程 |
| `TASKS.md` | 核心工作職責 |
| `LOG.md` | 實際執行任務的紀錄（`YYMMDD-主題` 命名，空白起始） |

`Hiring_Brief.md` 是完整版原文，保留作為參考來源，8 件套的內容都是從這裡拆出來的。

## 其他內容
| 內容 | 用途 |
|---|---|
| `scope.md` | 這個 agent 的使用範圍與安全規則 |
| `Hiring_Brief.md` | 完整版 Hiring Brief 原文 |
| `sessions/` | 這個 agent**自己專屬**的交接紀錄（跟工作區整體的 `../../04_Memory_Logs/` 分開） |

## 資料夾結構
```
Personal_AI_Assistant/
├── README.md            本檔案
├── scope.md              使用範圍與安全規則（重要，請先閱讀）
├── Hiring_Brief.md       完整版原文
├── AGENTS.md
├── SOUL.md
├── TOOLS.md
├── BRAIN.md
├── MEMORY.md
├── HEARTBEAT.md
├── TASKS.md
├── LOG.md
└── sessions/             這個 agent 專屬的記憶交接
    ├── Latest_State.md
    ├── MEMORY.md
    └── Daily_Summaries/
```

## 使用前必讀
請先閱讀 [scope.md](./scope.md)，了解哪些是工具內建機制、哪些是本專案額外要求 AI 遵守的規則。
