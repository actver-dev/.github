# ActVer

[English](README.md)

[![ActVer](https://img.shields.io/badge/ActVer-actver.dev-blue)](https://actver.dev)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-support-orange?logo=buy-me-a-coffee&logoColor=white)](https://buymeacoffee.com/yetanother_yk)

**ActVer** は GitHub Actions の最新バージョンとコミット SHA を簡単に取得できる無料サービスです — REST API、MCP サーバー、Web UI を提供しています。

リリースページを探し回る必要はもうありません。1 リクエストで欲しいバージョンが手に入ります。

## 提供しているもの

**[actver.dev](https://actver.dev)** — GitHub Actions バージョン検索の Web UI & REST API

- 最新バージョン＋フルコミット SHA をワンリクエストで取得
- レート制限の心配なし — キャッシュ済みで高速
- AI コーディングエージェント向け MCP サーバー（Claude Code、Cursor、Copilot 等）

**[actver-dev/skills](https://github.com/actver-dev/skills)** — AI コーディングエージェント向けプラグイン＆スキル

- **SHA ピン留め** — サプライチェーン攻撃からワークフローを保護
- **Actions アップグレード** — 最新バージョンへ自動更新
- **ワークフロー監査** — CI/CD パイプラインのセキュリティ問題を検出

## クイックスタート

### プラグインを使う（推奨）

```bash
# Claude Code
claude plugin marketplace add actver-dev/skills
claude plugin install actver

# その他のエージェント（Cursor、Copilot 等）
npx skills add actver-dev/skills
```

### MCP サーバーを使う

`.mcp.json` に追加:

```json
{
  "mcpServers": {
    "actver": {
      "type": "http",
      "url": "https://actver.dev/mcp"
    }
  }
}
```

### API を使う

```bash
curl https://actver.dev/v1/actions/actions/checkout
```

## サポート

ActVer は無料サービスです。もしお役に立てたら:

- [Buy Me a Coffee](https://buymeacoffee.com/yetanother_yk)
- [GitHub Sponsors](https://github.com/sponsors/actver-dev)
