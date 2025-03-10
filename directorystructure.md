# ディレクトリ構成

以下のディレクトリ構造に従って実装を行ってください：

```
/
├── app/                          # Laravelアプリケーションディレクトリ
│   ├── Http/                     # HTTPリクエスト処理
│   │   ├── Controllers/          # コントローラークラス
│   │   │   └── Auth/             # 認証関連コントローラー
│   │   └── Requests/             # フォームリクエスト
│   ├── Models/                   # Eloquentモデル
│   ├── Providers/                # サービスプロバイダー
│   └── View/                     # Viewコンポーネント
├── bootstrap/                    # アプリケーション起動
├── config/                       # 設定ファイル
├── database/                     # データベース関連
│   ├── factories/                # モデルファクトリー
│   ├── migrations/               # マイグレーションファイル
│   └── seeders/                  # シーダークラス
├── public/                       # 公開ディレクトリ
├── resources/                    # リソースファイル
│   ├── css/                      # CSSファイル
│   ├── js/                       # JavaScriptファイル
│   └── views/                    # Bladeテンプレート
│       ├── auth/                 # 認証関連ビュー
│       ├── components/           # 共通コンポーネント
│       └── layouts/              # レイアウトテンプレート
├── routes/                       # ルーティング
├── storage/                      # ストレージディレクトリ
├── tests/                        # テストファイル
├── vendor/                       # Composerパッケージ
├── node_modules/                 # npmパッケージ
├── .env                          # 環境変数（Gitで管理しない）
├── .gitignore                    # Git除外設定
├── composer.json                 # Composer設定
├── package.json                  # npm設定
├── tailwind.config.js            # Tailwind CSS設定
└── vite.config.js                # Vite設定
```

### 配置ルール
- コントローラー → `app/Http/Controllers/`
- モデル → `app/Models/`
- ビュー → `resources/views/`
- マイグレーション → `database/migrations/`
- ルート定義 → `routes/web.php`
- API定義 → `routes/api.php` 