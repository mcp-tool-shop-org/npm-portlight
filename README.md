<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/mcp-tool-shop-org/brand/main/logos/portlight/readme.png" width="400" alt="Portlight">
</p>

<p align="center">
  <a href="https://github.com/mcp-tool-shop-org/npm-portlight/actions"><img src="https://github.com/mcp-tool-shop-org/npm-portlight/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <a href="https://www.npmjs.com/package/@mcptoolshop/portlight"><img src="https://img.shields.io/npm/v/@mcptoolshop/portlight" alt="npm"></a>
  <a href="https://github.com/mcp-tool-shop-org/npm-portlight/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
  <a href="https://mcp-tool-shop-org.github.io/npm-portlight/"><img src="https://img.shields.io/badge/docs-landing_page-blue" alt="Landing Page"></a>
</p>

npm wrapper for [Portlight](https://github.com/mcp-tool-shop-org/portlight) — a trade-first maritime strategy CLI. One command, no Python required.

## What is Portlight?

Portlight is a terminal strategy game where you build a merchant career across a living Mediterranean and West African economy. Buy low, sail dangerous routes, sell high, and reinvest your profits into infrastructure, reputation, and commercial leverage.

Unlike most trading games that flatten trade into a number going up, Portlight treats trade as a commercial discipline:

- **Prices react to your trades.** Dump grain at a port and the price crashes. Every sale shifts the local market.
- **Voyages carry real risk.** Storms, pirates, inspections — your provisions, hull, and crew matter.
- **Contracts require proof.** Deliver the right goods to the right port with tracked provenance.
- **Infrastructure changes how you trade.** Warehouses stage cargo, brokers improve contracts, licenses unlock premium access.
- **Finance is leverage with teeth.** Credit lets you move faster. Default, and doors close.
- **Four victory paths.** Lawful Trade House, Shadow Network, Oceanic Reach, or Commercial Empire — the game reads what you actually built.

Three captain types (Merchant, Smuggler, Navigator), 10 ports, 8 trade goods, 17 routes, 27 milestones, and a full insurance/credit system.

## Quick Start

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

Or install globally:

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## How It Works

This package downloads the pre-built Portlight binary for your platform from GitHub Releases and caches it locally. No Python installation required.

| Concern | Detail |
|---------|--------|
| **Network** | HTTPS only to `github.com` CDN |
| **Filesystem** | Writes to user cache only (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | SHA256 checksum on every download |
| **Telemetry** | None. No tracking, no analytics, no phone-home. |
| **Platforms** | Windows (x64), macOS (x64/arm64), Linux (x64) |

## Also Available via pip

If you have Python installed:

```bash
pip install portlight
```

## Security

- Downloads binaries exclusively from `github.com` over HTTPS
- SHA256 checksum verification on every download
- Writes only to user-scoped cache directory — never touches system directories
- No telemetry, no secrets, no credentials stored
- No network access beyond the initial binary download

See [SECURITY.md](SECURITY.md) for the full security policy.

## License

MIT

Built by <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
