# currency-alert-app

## 目的
任意の通貨ペアの為替レートを監視し、ユーザーに通知する

## 主な機能
- ユーザー登録・ログイン（JWT認証）
- 通貨ペアと通知条件の設定
- 定期的に為替レート取得 → 通知送信（LINE Notifyやメール）
- 過去のレート履歴をDBに保存
- APIで現在値・履歴を取得可能

## 技術スタック
- バックエンド: FastAPI（Python）
- DB: PostgreSQL
- クラウド: AWS EC2 + RDS（将来的にECS/Lambda）
- CI/CD: GitHub Actions
- IaC: Terraform
