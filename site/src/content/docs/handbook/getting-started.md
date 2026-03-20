---
title: Getting Started
description: Install and play Portlight in under a minute
sidebar:
  order: 1
---

## Run instantly with npx

No installation needed — npx downloads and runs the wrapper automatically:

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
```

The first run downloads the Portlight binary (~15 MB). Subsequent runs start instantly from cache.

## Install globally

For repeated play, install once:

```bash
npm install -g @mcptoolshop/portlight
```

Then use `portlight` directly:

```bash
portlight new "Captain Hawk" --type merchant
portlight market
portlight buy grain 10
portlight sail al_manar
portlight advance
portlight sell grain 10
```

## Your first session

1. **Create a captain** — choose Merchant (better prices), Smuggler (black market), or Navigator (faster ships)
2. **Check the market** — `portlight market` shows local prices. Look for cheap goods.
3. **Buy cargo** — `portlight buy grain 10` loads your hold
4. **Pick a route** — `portlight routes` shows where you can sail and what sells there
5. **Sail** — `portlight sail al_manar` starts the voyage
6. **Advance** — `portlight advance` progresses through the voyage (weather, events, arrival)
7. **Sell** — `portlight sell grain 10` at the destination for profit
8. **Reinvest** — upgrade your ship, lease a warehouse, or pursue a contract

## Also available via pip

If you have Python installed:

```bash
pip install portlight
```

## Supported platforms

| Platform | Architecture |
|----------|-------------|
| Windows  | x64         |
| macOS    | x64, arm64  |
| Linux    | x64         |
