# 02_Knowledge_Base — 餵資料

存放 Agents 執行任務時需要參考的穩定資料。

## 資料夾
| 資料夾 | 用途 |
|---|---|
| `approved_references/` | 已批准可讓 agent 學習：已批准 SOP、公開 FAQ、內部可分享政策摘要 |
| `examples/` | 安全的範例：fake HR case、sample customer question |
| `templates/` | 可重用模板：meeting note template、reply template |

## 使用方式
- 適合放「不常變動、會被重複參考」的內容
- 不適合放「一次性、正在處理中」的任務內容，那應該放在 `../01_Action_Center/`

## 注意
內容不得包含密碼、API key、私人資料、薪酬資料、員工紀錄或客戶紀錄。此資料夾內容會被推送到 **public** GitHub repository，請格外小心。
