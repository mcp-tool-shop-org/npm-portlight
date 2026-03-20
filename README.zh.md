<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.md">English</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
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

npm 包装器，用于 [Portlight](https://github.com/mcp-tool-shop-org/portlight)——一个以贸易为先的航运战略命令行工具。 只需要一条命令，无需 Python。

## 什么是 Portlight？

Portlight 是一款终端策略游戏，您可以在一个充满活力的地中海和西非经济环境中，构建您的贸易事业。 低价购买，走危险的航线，高价出售，并将您的利润再投资于基础设施、声誉和商业优势。

与大多数将贸易简化为数值上升的贸易游戏不同，Portlight 将贸易视为一种商业纪律：

- **价格会根据您的交易而变化。** 在一个港口倾销粮食，价格就会暴跌。 每次销售都会改变当地市场。
- **航行存在真实的风险。** 暴风雨、海盗、检查——您的补给、船体和船员都至关重要。
- **合同需要证明。** 将正确的货物运送到正确的港口，并提供可追溯的来源证明。
- **基础设施会改变您的贸易方式。** 仓库用于存放货物，经纪人可以改善合同，许可证可以解锁高级权限。
- **金融是具有实际意义的杠杆。** 信用可以帮助您更快地发展。 如果违约，机会就会关闭。
- **有四种胜利途径。** 可以是合法的贸易公司、秘密网络、海洋霸权或商业帝国——游戏会根据您实际构建的内容进行判断。

有三种船长类型（商人、走私犯、航海家），10 个港口，8 种贸易商品，17 条航线，27 个里程碑，以及完整的保险/信用系统。

## 快速开始

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

或者，全局安装：

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## 工作原理

此包会从 GitHub 发布页面下载适用于您平台的预构建 Portlight 二进制文件，并将其缓存在本地。 无需安装 Python。

| 注意事项 | 详细信息 |
|---------|--------|
| **Network** | 仅通过 HTTPS 连接到 `github.com` CDN |
| **Filesystem** | 只写入用户缓存目录 (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | 每次下载都会进行 SHA256 校验和验证 |
| **Telemetry** | 无。 不进行跟踪，不收集分析数据，不进行任何数据传输。 |
| **Platforms** | Windows (x64), macOS (x64/arm64), Linux (x64) |

## 也可通过 pip 安装

如果您已安装 Python：

```bash
pip install portlight
```

## 安全性

- 仅通过 HTTPS 从 `github.com` 下载二进制文件
- 每次下载都会进行 SHA256 校验和验证
- 仅写入用户范围的缓存目录，不会修改系统目录
- 不收集任何遥测数据，不存储任何密钥或凭据
- 除了初始的二进制文件下载之外，没有其他网络访问

请参阅 [SECURITY.md](SECURITY.md) 以获取完整的安全策略。

## 许可证

MIT

构建者：<a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
