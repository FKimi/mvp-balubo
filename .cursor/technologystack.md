# 技術スタック（※本記載は記入例です-プロジェクトに合わせて内容を更新してください-）

## コア技術
- TypeScript: ^5.0.0
- Node.js: ^20.0.0  
- **AIモデル: claude-3-7-sonnet-20250219 (Anthropic Messages API 2023-06-01) ← バージョン変更禁止**

## フロントエンド
- Next.js: ^15.1.3
- React: ^19.0.0
- Tailwind CSS: ^3.4.17
- shadcn/ui: ^2.1.8

## バックエンド
- SQLite: ^3.0.0
- Prisma: ^5.0.0

## 開発ツール
- npm: ^10.0.0
- ESLint: ^9.0.0
- TypeScript: ^5.0.0

---

# API バージョン管理
## 重要な制約事項
- APIクライアントは `app/lib/api/client.ts` で一元管理
- AI モデルのバージョンは client.ts 内で厳密に管理
- これらのファイルは変更禁止（変更が必要な場合は承認が必要）：
  - client.ts  - AIモデルとAPI設定の中核
  - types.ts   - 型定義の一元管理
  - config.ts  - 環境設定の一元管理

## 実装規則
- AIモデルのバージョンは client.ts でのみ定義
- 型定義は必ず types.ts を参照
- 環境変数の利用は config.ts 経由のみ許可
