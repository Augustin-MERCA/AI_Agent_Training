# AI_Agent_Training

工作區依照 [Folder_Routing_Map.md](./Folder_Routing_Map.md) 的五個角色分工：

| 角色 | 資料夾 | 功能 |
|---|---|---|
| Inbox 收集 | `00_Inbox/` | 暫存尚未處理的想法、任務、請求 |
| Action Center 推進 | `01_Action_Center/` | 追蹤任務狀態（Now / Next / Waiting / Someday）與 agent 產出（outputs/） |
| Knowledge Base 餵資料 | `02_Knowledge_Base/` | 提供 agent 執行時參考的穩定資料 |
| Agents 做事 | `03_Agents/` | 各個 AI 員工本體（目前：`Personal_AI_Assistant`） |
| Memory Logs 交接 | `04_Memory_Logs/` | 工作區整體的交接紀錄（每個 agent 自己的交接紀錄在該 agent 資料夾下的 `sessions/`） |

## 不確定 file 要放哪裡？
先讀 [Folder_Routing_Map.md](./Folder_Routing_Map.md)；還是不確定就先丟進 `00_Inbox/`，再叫 agent 幫忙分流。

## 安全規則
每個 agent 有自己的 `scope.md`（例如 [03_Agents/Personal_AI_Assistant/scope.md](./03_Agents/Personal_AI_Assistant/scope.md)），列出安全範圍與規則。這個 repository 是 **public**，所有內容都不得包含密碼、API key、私人資料、薪酬資料、員工紀錄或客戶紀錄。
