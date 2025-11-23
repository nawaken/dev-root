

---
## フォルダ構成

dev-root/                ← すべてを統合する親
│
├── pnpm-workspace.yaml  ← 全プロジェクト管理
├── package.json         ← 共通scripts / 開発ツール
├── tsconfig.base.json   ← 全体共通の型設定
├── biome.json           ← 全体共通Lint
├── .npmrc               ← pnpm設定
│
├── scripts/             ← submodule（小物スクリプト）
│   ├── package.json
│   └── src/
│
├── automations/         ← submodule（n8n, API連携）
│   ├── package.json
│   └── src/
│
├── tools/               ← submodule（CLI/ユーティリティ）
│   ├── package.json
│   └── src/
│
├── notebooks/           ← submodule（調査コード）
│   ├── package.json
│   └── src/
│
└── apps/                ← ★将来追加する“本格アプリ”
    ├── web/             ← Next.js（Reactフロント）
    │   ├── package.json
    │   ├── next.config.js
    │   └── src/
    │
    ├── api/             ← 将来のNode/Express/Fastifyバックエンド
    │   ├── package.json
    │   └── src/
    │
    └── ui/              ← UIコンポーネント集（React）
        ├── package.json
        └── src/

---
