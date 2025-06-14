## PR 建立者確認清單

- [ ] Ticket 連結：
  - [請填入對應任務]()
- [ ] 更新本地分支：`git fetch --all && git rebase origin/main --autostash`（若有衝突記得解決並 `git push`）
- [ ] 設定 `Reviewer` 與 `Assignees` (所有 committers 或自己)
- [ ] 建立 PR 時選擇「Create draft pull request」
- [ ] 確認相關環境需求（請於 Ticket 中補充）
  - 是否需要更新 `.env`？
  - 是否需執行 `DB Migration`？
  - 是否涉及`資料處理`或`排程工具`？
  - 是否`依賴`其他子系統？
  - 是否需特殊上線流程（如相容性、多段部署）或退版處理？
- [ ] 通知 `Reviewer` 開始審核

> 參考：
> - [Atomic Git Commit](https://dev.to/samuelfaure/how-atomic-git-commits-dramatically-increased-my-productivity-and-will-increase-yours-too-4a84)：一次只做一件事，提高效率與可維護性
> - [Google - Small CLs](https://google.github.io/eng-practices/review/developer/small-cls.html)：小變更更安全、審查更快

---

## 審核者確認清單

> 工具推薦：[GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)

- [ ] 閱讀並審核程式碼，提出必要建議
- [ ] 若需調整，請通知建立者更新
  - 檢查需求邏輯、設計思路與測試方法
  - 程式碼可讀性與可維護性（風格、註解、API 文件、架構、Commit）
  - 效能、安全性、上/退版流程
  - 沒有 無關變更（如格式、debug 殘留）
- [ ] 通知 RD 送交 QA 測試

> 參考：
> - [Google - Code Review 指南](https://google.github.io/eng-practices/review/reviewer/looking-for.html#summary)
> - [Code Smells](https://refactoring.guru/refactoring/smells)
> - [Clean Code PHP](https://github.com/piotrplenik/clean-code-php) / [JavaScript](https://github.com/ryanmcdermott/clean-code-javascript)
> - [命名參考](https://github.com/kettanaito/naming-cheatsheet)
> - 團隊風格指引：  
>   [PER Coding Style](https://www.php-fig.org/per/coding-style/) / [Airbnb JS Style](https://github.com/airbnb/javascript)

---

## PR 建立者上線前確認

> ⚠️ 此區請於收到上線通知後執行

- [ ] 確認 `Reviewer` 為「Approved」狀態
- [ ] 確認 QA 測試已通過  
  - 測試紀錄連結：[請填寫]()
- [ ] 更新分支：`git fetch --all && git rebase origin/main --autostash` → `git push`
- [ ] 通知上線負責人並附上 PR 連結  
  - 如有環境或部署需求，請一併說明

---

## 上線者確認清單

- [ ] 確認 Review、測試、上線準備完成
- [ ] 確認 RD 說明的環境條件皆已處理：
  - `.env` 變更？
  - `DB Migration`？
  - 是否涉及`資料處理`或`排程工具`？
  - 是否`依賴`其他子系統？
  - 是否需特殊上線流程（如相容性、多段部署）或退版處理？
- [ ] 登記上線版本號
- [ ] 通知團隊上線完成

> 註：本樣板提供 PR 確認項目參考，內容可視情況調整。