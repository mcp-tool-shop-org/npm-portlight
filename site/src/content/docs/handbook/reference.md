---
title: Command Reference
description: All Portlight commands available through the npm wrapper
sidebar:
  order: 2
---

All Portlight commands work identically through the npm wrapper. Prefix with `npx @mcptoolshop/portlight` (or just `portlight` if installed globally).

## Game commands

| Group | Commands | Description |
|-------|----------|-------------|
| **Setup** | `new`, `load`, `save` | Create captains, manage save files |
| **Trading** | `market`, `buy`, `sell`, `cargo` | Inspect prices, trade goods |
| **Navigation** | `routes`, `sail`, `advance`, `port` | Plan and execute voyages |
| **Ship** | `provision`, `repair`, `hire` | Maintain your vessel |
| **Contracts** | `contracts`, `accept`, `obligations`, `abandon` | Commercial agreements |
| **Finance** | `credit`, `repay` | Credit and debt management |
| **Infrastructure** | `infra`, `warehouse`, `broker`, `license` | Build your trade house |
| **Career** | `milestones`, `status`, `ledger` | Track progress and history |
| **Help** | `guide` | In-game command reference |

## Wrapper-specific behavior

The npm wrapper is transparent — it passes all arguments directly to the Portlight binary. There are no wrapper-specific flags or commands.

### Binary location

The cached binary lives at:

- **Linux/macOS:** `~/.cache/mcptoolshop/portlight/`
- **Windows:** `%LOCALAPPDATA%/mcptoolshop/portlight/`

### Updating

When a new Portlight release is published, update the npm package:

```bash
npm install -g @mcptoolshop/portlight@latest
```

The new version will download the updated binary on first run.

## Security

- Downloads from `github.com` over HTTPS only
- SHA256 checksum verification on every download
- No telemetry, no tracking, no phone-home
- Binary runs with your user permissions — no elevated access needed
