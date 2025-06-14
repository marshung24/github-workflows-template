---
name: 🚀 Feature PR
about: 新功能開發合併 PR 模板
title: "[Code] Ticket標題"
labels: [feature]
assignees: []
---

# Feature Pull Request Template

## 🚀 新功能 PR
> Git Flow: feature to develop/release

### 🔗 Ticket 連結
- Feature Ticket：
  - `[Code Ticket標題]()`

### ✅ 檢查清單
- [ ] 本地端測試通過
- [ ] 通知主管及職代審核
- [ ] 主管及職代審核完畢
  - [ ] 需求確認、設計思路、測試方法
  - [ ] 可讀性/可維護性：程式碼風格、文件/範例/註解、OpenAPI/Postman、程式架構、Commit
  - [ ] 效能、資安、上線/退版步驟
  - [ ] 沒有不相關的調整
- [ ] 送測，Ticket 狀態更新為「Ready for QA」
- [ ] QA測試通過
- [ ] Rebase至最新根節點，解衝突(如有)
  - [ ] 有衝突請重測衝突的地方
- [ ] 合併分支並通知相關人員

