<p align="center">
  <a href="README.md">English</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
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

[Portlight](https://github.com/mcp-tool-shop-org/portlight) の npm ラッパーです。これは、海事戦略を支援するコマンドラインツールです。1つのコマンドで利用でき、Python は不要です。

## Portlight とは？

Portlight は、地中海と西アフリカの経済圏を舞台にした、ターミナル上で動作する戦略ゲームです。安く商品を購入し、危険な航路を使い、高く商品を販売し、利益をインフラ、評判、商業的な優位性へと再投資します。

ほとんどのトレーディングゲームが、取引を単なる数値の増加として扱うのに対し、Portlight は取引を商業的な規律として扱います。

- **価格はあなたの取引によって変動します。** ある港に穀物を大量に供給すると、価格が暴落します。すべての販売が、地域の市場に影響を与えます。
- **航海には実際の危険が伴います。** 嵐、海賊、検査など、積載物、船体、乗組員の状況が重要になります。
- **契約には証拠が必要です。** 追跡可能な産地情報とともに、正しい商品を正しい港に配達する必要があります。
- **インフラは取引方法を変えます。** 倉庫は貨物を一時保管し、仲介業者は契約を改善し、ライセンスは特別な機能へのアクセスを解放します。
- **金融は強力なレバレッジです。** 信用はより迅速な行動を可能にします。しかし、デフォルトすると、機会が失われます。
- **勝利への道は4つあります。** 正当な貿易会社、秘密結社、広大な海洋支配、または商業帝国。ゲームは、あなたが実際に構築したものを評価します。

船長タイプは3種類（商人、密輸業者、航海士）、港は10、取引商品は8種類、航路は17、マイルストーンは27、そして完全な保険/信用システムを備えています。

## クイックスタート

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

または、グローバルにインストールします。

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## 仕組み

このパッケージは、GitHub Releases からあなたのプラットフォームに対応したあらかじめビルドされた Portlight の実行ファイルをダウンロードし、ローカルにキャッシュします。Python のインストールは不要です。

| 注意点 | 詳細 |
|---------|--------|
| **Network** | `github.com` CDN への HTTPS 通信のみ |
| **Filesystem** | ユーザーキャッシュディレクトリ (`~/.cache/mcptoolshop/portlight/`) への書き込みのみ |
| **Verification** | ダウンロードごとに SHA256 チェックサムを確認 |
| **Telemetry** | 特になし。トラッキング、分析、テレメトリーは一切ありません。 |
| **Platforms** | 対応プラットフォーム：Windows (x64)、macOS (x64/arm64)、Linux (x64) |

## pip からも利用可能

Python がインストールされている場合：

```bash
pip install portlight
```

## セキュリティ

- 実行ファイルは、HTTPS を使用して `github.com` からのみダウンロードされます。
- ダウンロードごとに SHA256 チェックサムによる検証を行います。
- ユーザーのキャッシュディレクトリへの書き込みのみ。システムディレクトリには一切アクセスしません。
- テレメトリー、機密情報、認証情報は一切保存しません。
- 実行ファイルのダウンロード以外、ネットワークアクセスはありません。

詳細なセキュリティポリシーについては、[SECURITY.md](SECURITY.md) を参照してください。

## ライセンス

MIT

開発：<a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
