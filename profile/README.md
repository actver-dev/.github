# ActVer

[日本語](README.ja.md)

[![ActVer](https://img.shields.io/badge/ActVer-actver.dev-blue)](https://actver.dev)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-support-orange?logo=buy-me-a-coffee&logoColor=white)](https://buymeacoffee.com/yetanother_yk)

**ActVer** is a free service that makes it easy to look up the latest GitHub Actions versions and commit SHAs — via REST API, MCP server, and web UI.

Stop digging through release pages. Get the version you need in one request.

## What We Offer

**[actver.dev](https://actver.dev)** — Web UI & REST API for GitHub Actions version lookup

- Get the latest version + full commit SHA with a single GET request
- No rate-limit headaches — cached and fast
- MCP server for AI coding agents (Claude Code, Cursor, Copilot, etc.)

**[actver-dev/skills](https://github.com/actver-dev/skills)** — Plugin & skills for AI coding agents

- **Pin actions to SHA** — secure your workflows against supply-chain attacks
- **Upgrade actions** — bump to latest versions automatically
- **Audit workflows** — detect security issues in your CI/CD pipelines

## Quick Start

### Use the Plugin (recommended)

```bash
# Claude Code
claude plugin install actver-dev/skills

# Other agents (Cursor, Copilot, etc.)
npx skills add actver-dev/skills
```

### Use the MCP Server

Add to your `.mcp.json`:

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

### Use the API

```bash
curl https://actver.dev/v1/actions/actions/checkout
```

## Support

ActVer is a free service. If you find it useful:

- [Buy Me a Coffee](https://buymeacoffee.com/yetanother_yk)
- [GitHub Sponsors](https://github.com/sponsors/actver-dev)
