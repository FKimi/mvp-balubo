# 技術スタック

## コア技術
- PHP: ^8.2.0
- Laravel: ^11.0
- **AIモデル: claude-3-7-sonnet (Anthropic Messages API 2023-06-01) ← バージョン変更禁止**

## フロントエンド
- Blade: Laravel 標準
- Tailwind CSS: ^3.4.0

## バックエンド
- MySQL: ^8.0.0
- Eloquent ORM: Laravel 11 標準

## 開発ツール
- Composer: ^2.0.0
- npm: ^10.0.0
- Vite: ^5.0.0

---

# API バージョン管理
## 重要な制約事項
- APIキーは `.env` ファイルで一元管理
- AI モデルのバージョンは環境設定で厳密に管理
- これらのファイルは変更禁止（変更が必要な場合は承認が必要）：
  - config/services.php  - APIキー設定の中核
  - .env.example        - 環境変数の例示

## 実装規則
- AIモデルのバージョンは config/services.php でのみ定義
- 環境変数の利用は .env 経由のみ許可
- 認証情報は絶対にバージョン管理に含めない 