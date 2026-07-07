# Folder Routing Map｜我應該把 file 放邊？

如果你不知道某份 file 應該放哪裏，先用這張表。

| 情況 | 放到哪裏 | 例子 |
|---|---|---|
| 未整理、未決定、只是先收住 | `00_Inbox/` | 一條 FAQ idea、一段 copied note、一個未確認 SOP |
| 本月一定要處理 | `01_Action_Center/Now.md` | 完成 Personal Assistant v1 |
| 本季排隊中 | `01_Action_Center/Next.md` | 之後建立第二位 FAQ/SOP agent |
| 等別人回覆 / 等資料 | `01_Action_Center/Waiting.md` | 等同事提供 approved FAQ |
| 好想法但暫時做不到 | `01_Action_Center/Someday.md` | 之後做 advanced automation |
| Agent 產出的草稿 | `01_Action_Center/outputs/drafts/` | Hermes instruction draft、FAQ agent draft |
| 測試或改進紀錄 | `01_Action_Center/outputs/test_logs/` | sensitive question test log、improvement log |
| 完成但暫時不需要用 | `01_Action_Center/outputs/archive/` | 舊版草稿、已替換的 output |
| 已批准可讓 agent 學習 | `02_Knowledge_Base/approved_references/` | 已批准 SOP、公開 FAQ、內部可分享政策摘要 |
| 安全 examples | `02_Knowledge_Base/examples/` | fake HR case、sample customer question |
| 可重用模板 | `02_Knowledge_Base/templates/` | meeting note template、reply template |
| AI 員工本體 | `03_Agents/` | Personal_AI_Assistant |
| 最新交接狀態 | `04_Memory_Logs/Latest_State.md` | 下次第一眼要知道的事 |
| 長期偏好 / 踩坑 / 決策 | `04_Memory_Logs/MEMORY.md` | 「不要貼真實 candidate data」 |
| 每次 session 摘要 | `04_Memory_Logs/Daily_Summaries/` | 260624_day1_setup.md |

## Training rule
不肯定放哪裏時，先放 `00_Inbox/`，再叫 agent 幫你分流。
