# ディレクトリ構成（※本記載は記入例です-プロジェクトに合わせて内容を更新してください-）

以下のディレクトリ構造に従って実装を行ってください：

```
/
├── app/                          # Next.jsのアプリケーションディレクトリ
│   ├── api/                      # APIエンドポイント
│   │   └── [endpoint]/
│   │       └── route.ts
│   ├── components/               # アプリケーションコンポーネント
│   │   ├── ui/                   # 基本UI（button, card等）
│   │   └── layout/               # レイアウト関連
│   ├── hooks/                    # カスタムフック
│   ├── lib/                      # ユーティリティ
│   │   ├── api/                  # API関連処理
│   │   │   ├── client.ts         # 変更禁止: AIモデル設定
│   │   │   ├── types.ts          # 変更禁止: 型定義
│   │   │   └── config.ts         # 変更禁止: 環境設定
│   │   └── utils/                # 共通関数
│   ├── styles/                   # スタイル定義
│   ├── favicon.ico               # ファビコン
│   ├── globals.css               # グローバルスタイル
│   ├── layout.tsx                # ルートレイアウト
│   └── page.tsx                  # ホームページ
├── public/                       # 静的ファイル
├── node_modules/                 # 依存パッケージ
├── .git/                         # Gitリポジトリ
├── .cursor/                      # Cursor設定
├── package.json                  # プロジェクト設定
├── package-lock.json             # 依存関係ロックファイル
├── tsconfig.json                 # TypeScript設定
├── next-env.d.ts                 # Next.js型定義
├── next.config.ts                # Next.js設定
├── postcss.config.mjs            # PostCSS設定
├── eslint.config.mjs             # ESLint設定
└── .gitignore                    # Git除外設定
```

### 配置ルール
- UIコンポーネント → `app/components/ui/`
- APIエンドポイント → `app/api/[endpoint]/route.ts`
- 共通処理 → `app/lib/utils/`
- API関連処理 → `app/lib/api/`
