# AI Agent Training Home — 使用約定

本文件記錄使用者與 AI 確認過的 folder routing 偏好，之後所有 session 都依此執行。

## 每一層 folder 的用途

| Folder | 用途（一句話） |
|---|---|
| `00_Inbox/` | 收集未整理的素材 |
| `01_Action_Center/` | 追蹤任務狀態、暫存 agent 產出等待確認 |
| `02_Knowledge_Base/` | 存放已核准或安全的參考資料 |
| `03_Agents/` | 存放各個 AI 員工（agent）本體 |
| `04_Memory_Logs/` | 工作區整體的交接與長期記憶 |

## 我的 routing 偏好

1. **Inbox** — 丟入的素材類型：ideas、links、尚未分類的主題
2. **Action Center 分類邏輯**：依時間急迫性
   - `Now.md` = 本週要做
   - `Next.md` = 已排入計畫但未開始
   - `Waiting.md` = 卡住了，等別人回覆或等資料
   - `Someday.md` = 沒有時間表的純想法
3. **Outputs**：agent 產出的草稿、test logs 一律先放 `01_Action_Center/outputs/`，等使用者確認後才搬去 `02_Knowledge_Base/`（變正式參考資料）或 `outputs/archive`（封存）
4. **Knowledge Base 分流標準**：內容是否「真實發生過、且已核准可分享」？
   - 是 → `approved_references/`
   - 不是（虛構、未核准，即使看起來像真的）→ `examples/`
5. **Agents**：目前只有 `Personal_AI_Assistant` 一位 agent。未來新增第二位 agent（如 FAQ/SOP agent）時，是否平行放在 `03_Agents/` 底下、還是放進 `Personal_AI_Assistant` 內部，屆時再決定，暫不預設
6. **Memory Logs 分工**：
   - `Latest_State.md` — 最新狀態、任何 pending 中的事
   - `Daily_Summaries/` — 每日任務摘要
   - `MEMORY.md` — 只記重要、不會變動的事：規則、規定、長期原則（不是逐次對話全部塞進去）
7. **命名格式**：`YYMMDD_主題.md`（例如 `260707_folder_setup.md`）

## AI 之後會遵守的規則

- Folder 結構可以建議，但 `move`／`rename`／`delete`／`overwrite` 一律要先問過使用者才能執行；新增全新檔案／資料夾不受此限制
- 每次檔案變更後，自動 `git add` → `commit` → `push`（除非內容疑似敏感，會先暫停詢問）
- 不要求提供密碼、API key、私人資料、薪酬資料、員工紀錄或客戶紀錄
- 高風險指令（delete、force、admin 權限、credential 相關）一律先解釋再等使用者確認
- 發現內容有問題時，只指出問題，由使用者決定怎麼處理

## 哪些資料不可放入任何 folder

不論放在哪一層（包含 `examples/`、`approved_references/`、任何 session 記錄），一律不得包含：
- 密碼、API key、token、憑證
- 私人資料
- 薪酬資料
- 員工紀錄
- 客戶紀錄

（此 repository 為 **public**，以上規則格外重要）
