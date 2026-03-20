<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.md">English</a> | <a href="README.pt-BR.md">Português (BR)</a>
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

Wrapper npm per [Portlight](https://github.com/mcp-tool-shop-org/portlight) — un'interfaccia a riga di comando (CLI) per una strategia marittima incentrata sul commercio. Un solo comando, non è necessario Python.

## Cos'è Portlight?

Portlight è un gioco di strategia a terminale in cui si costruisce una carriera commerciale in un'economia mediterranea e dell'Africa occidentale in continua evoluzione. Si acquistano merci a basso prezzo, si percorrono rotte pericolose, si vendono a prezzi elevati e si reinvestono i profitti in infrastrutture, reputazione e vantaggi commerciali.

A differenza della maggior parte dei giochi di commercio che semplificano il commercio in un semplice numero in aumento, Portlight considera il commercio come una disciplina commerciale:

- **I prezzi reagiscono alle vostre transazioni.** Se scaricate grandi quantità di grano in un porto, il prezzo crolla. Ogni vendita modifica il mercato locale.
- **I viaggi comportano rischi reali.** Tempeste, pirati, ispezioni: le vostre provviste, lo scafo e l'equipaggio sono importanti.
- **I contratti richiedono prove.** È necessario consegnare le merci giuste al porto giusto, con una tracciabilità della provenienza.
- **Le infrastrutture modificano il modo in cui commerciate.** I magazzini stoccano le merci, i broker migliorano i contratti, le licenze sbloccano l'accesso a funzionalità avanzate.
- **La finanza è un'arma a doppio taglio.** Il credito vi permette di agire più rapidamente. Se non riuscite a ripagarlo, vi verranno chiuse le porte.
- **Quattro percorsi per la vittoria.** Casa commerciale legale, rete clandestina, influenza oceanica o impero commerciale: il gioco valuta ciò che avete effettivamente costruito.

Tre tipi di capitani (Mercante, Contrabbandiere, Navigatore), 10 porti, 8 merci, 17 rotte, 27 tappe e un sistema completo di assicurazione/credito.

## Avvio rapido

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

Oppure, installate globalmente:

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## Come funziona

Questo pacchetto scarica il file binario precompilato di Portlight per la vostra piattaforma da GitHub Releases e lo memorizza localmente. Non è necessaria l'installazione di Python.

| Considerazioni | Dettagli |
|---------|--------|
| **Network** | Solo HTTPS verso il CDN di `github.com` |
| **Filesystem** | Scrive solo nella cache dell'utente (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | Controllo del checksum SHA256 ad ogni download |
| **Telemetry** | Nessuno. Nessun tracciamento, nessuna analisi, nessuna trasmissione di dati. |
| **Platforms** | Windows (x64), macOS (x64/arm64), Linux (x64) |

## Disponibile anche tramite pip

Se avete Python installato:

```bash
pip install portlight
```

## Sicurezza

- Scarica i file binari esclusivamente da `github.com` tramite HTTPS
- Verifica del checksum SHA256 ad ogni download
- Scrive solo nella directory di cache specifica dell'utente: non tocca mai le directory di sistema
- Nessuna telemetria, nessun segreto, nessuna credenziale memorizzata
- Nessun accesso alla rete oltre al download iniziale del file binario

Consultare il file [SECURITY.md](SECURITY.md) per la politica di sicurezza completa.

## Licenza

MIT

Creato da <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
