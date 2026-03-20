# @mcptoolshop/portlight

npm wrapper for [Portlight](https://github.com/mcp-tool-shop-org/portlight) — trade-first maritime strategy CLI.

## Quick start

```bash
npx @mcptoolshop/portlight new
npx @mcptoolshop/portlight status
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
```

## How it works

This package downloads the pre-built Portlight binary for your platform from GitHub Releases and caches it locally. No Python installation required.

- **Network:** HTTPS only to `github.com` CDN
- **Filesystem:** Writes to user cache only (`~/.cache/mcptoolshop/portlight/`)
- **Verification:** SHA256 checksum verification on every download
- **No telemetry.** No secrets.

## Also available via pip

```bash
pip install portlight
```

## License

MIT
