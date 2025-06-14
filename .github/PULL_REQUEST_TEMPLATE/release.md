---
name: 📦 Release PR
about: 發布合併 PR 模板
title: "[Release] "
labels: [release]
assignees: []
---

# Release Pull Request Template

## 📦 發布合併 PR
> Git Flow: develop/release to main

### 📋 Release Note
- 版本號：v1.2.3
- 包含功能或修補項目簡述（可列出 Ticket 編號）
  - ✅ [Code] 新增註冊功能
  - 🐛 [Code] 修正付款錯誤

### ✅ 檢查清單
- [ ] main 與 develop 已同步代碼
- [ ] 已 tag 正確版本號
- [ ] Ticket 發布狀態已切為「Done」



## ✅ 檢查清單

### 🔧 上線內容確認
- [ ] 檢查待上線Ticket清單
- [ ] QA測試全部通過
- [ ] 上線時間
- [ ] 上線負責人

### 📦 系統部署檢查
- [ ] 是否需要更新 `.env` 設定檔（如新增環境變數）
- [ ] 是否需要執行 DB Migration？（請附上 migration 檔）
- [ ] 是否影響或依賴其他子系統？（請說明）

### ⛓️ 相依性與版本順序
- [ ] 是否與其他系統 Ticket 同步上版？（請列出）
- [ ] 是否與其他系統（BE / FE / OS 套件）相依？（請說明）
- [ ] 是否需要特定上版順序或多次上版？（請描述順序）

### 🚨 其他可能影響因素
- [ ] 是否涉及第三方服務串接？（請說明）
- [ ] 是否涉及排程工具或後台 cronjob？（請列出）
- [ ] 有沒有停機上版的必要？
  > DB Migration過久、鎖表、可能造成資料錯誤、新舊版程式及資料不相容
