# AI Team Workflow SOP

## 分支策略
- `main`: 穩定版本，僅合併經審核的 PR
- `dev`: 開發分支，所有新功能先在此完成

## Pull Request 流程
1. 開發者在 `dev` 分支完成功能
2. 建立 PR → 指派 Reviewer
3. CI/CD Pipeline 自動測試
4. Reviewer 審核通過 → 合併到 `main`

## 模型檔案規範
- 命名格式：`model_vX.Y_backtestYYYYMMDD.pkl`
- 每次更新需附回測報告 (Markdown/PDF)

## 工具整合
- GitHub Actions → 自動測試 / 模型驗證
- Notion → 知識庫 / 報告存檔
- Slack → PR / CI/CD 通知
