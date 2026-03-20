# Security Policy

[日本語](#セキュリティポリシー)

## Supported Versions

| Project | Supported |
|---------|-----------|
| [actver.dev](https://actver.dev) (API / MCP server) | :white_check_mark: |
| [actver-dev/skills](https://github.com/actver-dev/skills) (Plugin & skills) | :white_check_mark: |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

Use [GitHub Security Advisories](https://github.com/actver-dev/.github/security/advisories/new) to report vulnerabilities privately.

When reporting, please include:

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if any)

## Response

- We will acknowledge receipt within **72 hours**
- We aim to provide an initial assessment within **1 week**
- Critical vulnerabilities affecting the production service will be prioritized

## Scope

| In scope | Out of scope |
|----------|--------------|
| actver.dev API endpoints | Third-party dependencies (report upstream) |
| MCP server (`/mcp`) | GitHub Actions themselves |
| actver-dev/skills plugin | Theoretical attacks with no PoC |
| Web UI (webapp) | |

---

# セキュリティポリシー

## サポート対象バージョン

| プロジェクト | サポート |
|-------------|---------|
| [actver.dev](https://actver.dev)（API / MCP サーバー） | :white_check_mark: |
| [actver-dev/skills](https://github.com/actver-dev/skills)（プラグイン＆スキル） | :white_check_mark: |

## 脆弱性の報告

**セキュリティの脆弱性は公開 Issue で報告しないでください。**

[GitHub Security Advisories](https://github.com/actver-dev/.github/security/advisories/new) からプライベートに報告してください。

報告時に以下を含めてください:

- 脆弱性の説明
- 再現手順
- 想定される影響
- 修正案（あれば）

## 対応方針

- **72 時間以内**に受領を確認します
- **1 週間以内**に初期評価を回答します
- 本番サービスに影響する重大な脆弱性は優先的に対応します

## 対象範囲

| 対象 | 対象外 |
|------|--------|
| actver.dev API エンドポイント | サードパーティの依存関係（上流に報告してください） |
| MCP サーバー (`/mcp`) | GitHub Actions 自体 |
| actver-dev/skills プラグイン | PoC のない理論上の攻撃 |
| Web UI（webapp） | |
