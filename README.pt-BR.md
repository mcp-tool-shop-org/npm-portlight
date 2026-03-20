<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.md">English</a>
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

Wrapper npm para [Portlight](https://github.com/mcp-tool-shop-org/portlight) — uma ferramenta de linha de comando (CLI) para estratégias marítimas focadas em comércio. Um único comando, sem necessidade de Python.

## O que é Portlight?

Portlight é um jogo de estratégia para terminal onde você constrói uma carreira comercial em uma economia mediterrânea e africana vibrante. Compre barato, navegue por rotas perigosas, venda caro e reinvesta seus lucros em infraestrutura, reputação e vantagens comerciais.

Ao contrário da maioria dos jogos de comércio que simplificam o comércio em um número que aumenta, Portlight trata o comércio como uma disciplina comercial:

- **Os preços reagem às suas transações.** Despejar grãos em um porto faz com que o preço caia. Cada venda altera o mercado local.
- **As viagens envolvem riscos reais.** Tempestades, piratas, inspeções — suas provisões, casco e tripulação são importantes.
- **Os contratos exigem comprovação.** Entregue os produtos corretos no porto certo, com rastreabilidade.
- **A infraestrutura muda a forma como você comercializa.** Armazéns preparam a carga, corretores melhoram os contratos, licenças desbloqueiam acesso premium.
- **As finanças são uma alavancagem com consequências.** O crédito permite que você avance mais rápido. Se você não pagar, as portas se fecham.
- **Quatro caminhos para a vitória.** Casa de Comércio Legal, Rede Clandestina, Alcance Oceânico ou Império Comercial — o jogo avalia o que você realmente construiu.

Três tipos de capitães (Mercador, Contrabandista, Navegador), 10 portos, 8 produtos comerciais, 17 rotas, 27 marcos e um sistema completo de seguros/crédito.

## Início Rápido

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

Ou instale globalmente:

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## Como Funciona

Este pacote baixa o binário pré-compilado do Portlight para sua plataforma do GitHub Releases e o armazena localmente. Não é necessária a instalação do Python.

| Preocupações | Detalhes |
|---------|--------|
| **Network** | Apenas HTTPS para o CDN `github.com` |
| **Filesystem** | Escreve apenas no cache do usuário (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | Checksum SHA256 em cada download |
| **Telemetry** | Nenhum. Sem rastreamento, sem análises, sem envio de dados. |
| **Platforms** | Windows (x64), macOS (x64/arm64), Linux (x64) |

## Também disponível via pip

Se você tiver o Python instalado:

```bash
pip install portlight
```

## Segurança

- Baixa binários exclusivamente de `github.com` via HTTPS
- Verificação de checksum SHA256 em cada download
- Escreve apenas no diretório de cache do usuário — nunca acessa diretórios do sistema
- Sem telemetria, sem segredos, sem credenciais armazenadas
- Sem acesso à rede além do download inicial do binário

Consulte [SECURITY.md](SECURITY.md) para a política de segurança completa.

## Licença

MIT

Desenvolvido por <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a
