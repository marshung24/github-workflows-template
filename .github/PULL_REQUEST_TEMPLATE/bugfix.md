---
name: Bugfix PR
about: 修正錯誤的 PR 模板
title: "[Bugfix] "
labels: bug
---

# Bugfix Pull Request Template

## 🐛 錯誤修復 PR
> Git Flow: feature to develop/release

### 🔗 Ticket 連結
- Bug Ticket：
  - `[Code Ticket標題]()`

### ✅ 檢查清單
- [ ] 問題可被重現並成功修復
- [ ] 本地端測試通過
- [ ] 設定並通知審核：Reviewers (審核者：主管及職代) 與 Assignees (所有 committers 比如 PR 建立者自己)
- [ ] 審核完畢
  - [ ] 需求確認、設計思路、測試方法
  - [ ] 可讀性/可維護性：程式碼風格、文件/範例/註解、OpenAPI/Postman、程式架構、Commit
  - [ ] 效能、資安、上線/退版步驟
  - [ ] 沒有不相關的調整
- [ ] 送測，Ticket 狀態更新為「Ready for QA」
- [ ] QA測試通過
- [ ] Rebase更新分支 `git fetch --all && git rebase origin/mian --autostash` 若有更新請記得 `git push`
  - [ ] 如有衝突請解衝突，並重測衝突的地方
- [ ] 合併分支並通知相關人員


