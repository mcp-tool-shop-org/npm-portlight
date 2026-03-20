---
title: Portlight npm Wrapper
description: Zero-prerequisite installer for the Portlight maritime strategy CLI
sidebar:
  order: 0
---

The `@mcptoolshop/portlight` npm package lets you play [Portlight](https://github.com/mcp-tool-shop-org/portlight) without installing Python. It downloads the pre-built binary for your platform, verifies its SHA256 checksum, and caches it locally.

## What is Portlight?

Portlight is a terminal strategy game where you build a merchant career across a living Mediterranean and West African economy. Buy low, sail dangerous routes, sell high, and reinvest into infrastructure, reputation, and commercial leverage.

Three captain types, 10 ports, 8 trade goods, 17 routes, 27 milestones, and full insurance/credit systems.

## How the wrapper works

1. On first run, the wrapper downloads the Portlight binary from GitHub Releases
2. The binary is verified via SHA256 checksum
3. It's cached in `~/.cache/mcptoolshop/portlight/`
4. All subsequent runs use the cached binary — no download needed
5. Your arguments are passed straight through to Portlight

The wrapper adds no overhead beyond the initial download. It's a thin launcher powered by [`@mcptoolshop/npm-launcher`](https://github.com/mcp-tool-shop-org/npm-launcher).
