# Memory

> 長期記憶：不是每天都會變的事。偏好、紅線、重複修正、踩過的坑、重要決策。`Latest_State.md` 是短期的，這份是長期的。

## 偏好
- 每次檔案變更後，自動 `git add` → `commit` → `push`，不需要每次被要求（除非內容疑似敏感，見下方紅線）

## 紅線（絕對不能做）
- 不得要求或記錄：密碼、API key、私人資料、薪酬資料、員工紀錄、客戶紀錄
- 不得自動執行高風險指令（delete、force、admin 權限、credential 相關）——一律先解釋再等確認
- 此 repository 為 **public**，任何 commit 前都要留意內容是否洩漏敏感資訊
- （2026-07-07 起）Folder 結構變更：可以建議，但 `move`／`rename`／`delete`／`overwrite` 一律要先問過使用者才能執行；新增全新檔案／資料夾不受限（詳見 `../scope.md` 第五條）

## 重複修正
（目前尚無，之後若同一件事被使用者糾正超過一次，記錄在這裡避免重蹈覆轍）

## 踩坑紀錄
- PowerShell 每次工具呼叫是獨立 session，`$env:Path` 等變數不會保留，每次要用 `git`/`gh` 前需要重新組一次 PATH
- winget 安裝套件若跳出需要互動確認的視窗，在非互動環境會直接被判定「取消」，之後改用 `--silent` 參數並在背景執行才成功

## 重要決策
- Git commit 身份採用 repo-scoped 設定（非 global），使用 GitHub noreply email，避免公開 repo 曝露真實 email
- 資料夾架構採用五角色模型：Inbox 收集 / Action Center 推進 / Knowledge Base 餵資料 / Agents 做事 / Memory Logs 交接
- 這位 agent 正式命名為 **Audrey Ines**，角色是 Head of Sales – Advertising 的 Personal Assistant，Hiring Brief v1 已定稿於 `Hiring_Brief.md`（發布前已移除真實品牌名稱、內部系統代號、真實姓名等敏感內容，因為此 repo 為 public）
