<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.md">English</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
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

Wrapper npm pour [Portlight](https://github.com/mcp-tool-shop-org/portlight) — une interface en ligne de commande (CLI) pour une stratégie maritime axée sur le commerce. Une seule commande, sans Python requis.

## Qu'est-ce que Portlight ?

Portlight est un jeu de stratégie en terminal où vous construisez une carrière de commerçant dans une économie méditerranéenne et ouest-africaine dynamique. Achetez à bas prix, naviguez sur des routes dangereuses, vendez à prix élevé et réinvestissez vos bénéfices dans les infrastructures, la réputation et le pouvoir commercial.

Contrairement à la plupart des jeux de commerce qui réduisent le commerce à un simple chiffre qui augmente, Portlight considère le commerce comme une discipline commerciale :

- **Les prix réagissent à vos transactions.** Déchargez des céréales dans un port et le prix s'effondre. Chaque vente modifie le marché local.
- **Les voyages comportent de vrais risques.** Tempêtes, pirates, inspections — vos provisions, la coque et l'équipage sont importants.
- **Les contrats nécessitent des preuves.** Livrez les bons produits au bon port avec une traçabilité de l'origine.
- **Les infrastructures modifient votre façon de commercer.** Les entrepôts stockent les marchandises, les courtiers améliorent les contrats, les licences débloquent un accès premium.
- **La finance est un levier puissant.** Le crédit vous permet d'agir plus rapidement. Par défaut, les portes se referment.
- **Quatre voies vers la victoire.** Maison de commerce légale, réseau clandestin, portée océanique ou empire commercial — le jeu analyse ce que vous avez réellement construit.

Trois types de capitaines (Commerçant, Contrebandier, Navigateur), 10 ports, 8 produits de commerce, 17 routes, 27 étapes et un système complet d'assurance/crédit.

## Démarrage rapide

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

Ou installez-le globalement :

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## Comment ça marche

Ce paquet télécharge le fichier binaire de Portlight précompilé pour votre plateforme depuis les versions de GitHub et le met en cache localement. Aucune installation de Python n'est requise.

| Préoccupations | Détails |
|---------|--------|
| **Network** | HTTPS uniquement vers le CDN `github.com` |
| **Filesystem** | Écrit uniquement dans le cache de l'utilisateur (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | Vérification de la somme de contrôle SHA256 à chaque téléchargement |
| **Telemetry** | Aucune. Pas de suivi, pas d'analyses, pas de transmission de données. |
| **Platforms** | Windows (x64), macOS (x64/arm64), Linux (x64) |

## Également disponible via pip

Si vous avez Python installé :

```bash
pip install portlight
```

## Sécurité

- Télécharge les fichiers binaires exclusivement depuis `github.com` via HTTPS
- Vérification de la somme de contrôle SHA256 à chaque téléchargement
- Écrit uniquement dans le répertoire de cache spécifique à l'utilisateur — ne touche jamais les répertoires système
- Pas de télémétrie, pas de secrets, pas de données d'identification stockées
- Pas d'accès réseau au-delà du téléchargement initial du fichier binaire

Consultez [SECURITY.md](SECURITY.md) pour la politique de sécurité complète.

## Licence

MIT

Créé par <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
