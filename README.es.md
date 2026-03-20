<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.md">English</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
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

Wrapper de npm para [Portlight](https://github.com/mcp-tool-shop-org/portlight): una herramienta de línea de comandos para estrategias marítimas centradas en el comercio. Un solo comando, no se requiere Python.

## ¿Qué es Portlight?

Portlight es un juego de estrategia en terminal donde construyes una carrera comercial en una economía mediterránea y africana en constante evolución. Compra barato, navega por rutas peligrosas, vende a precios altos y reinvierte tus ganancias en infraestructura, reputación y ventajas comerciales.

A diferencia de la mayoría de los juegos de comercio que simplifican el comercio a un número que aumenta, Portlight trata el comercio como una disciplina comercial:

- **Los precios reaccionan a tus transacciones.** Si inundas un puerto con grano, el precio se desploma. Cada venta altera el mercado local.
- **Los viajes implican riesgos reales.** Tormentas, piratas, inspecciones: tus provisiones, casco y tripulación son importantes.
- **Los contratos requieren pruebas.** Entrega los productos correctos al puerto correcto con un seguimiento de su origen.
- **La infraestructura cambia la forma en que operas.** Los almacenes preparan la carga, los intermediarios mejoran los contratos y las licencias desbloquean acceso premium.
- **Las finanzas son una palanca con consecuencias.** El crédito te permite avanzar más rápido. Si incumples, las puertas se cierran.
- **Cuatro caminos hacia la victoria.** Casa comercial legal, red clandestina, alcance oceánico o imperio comercial: el juego evalúa lo que realmente has construido.

Tres tipos de capitanes (Comerciante, Contrabandista, Navegante), 10 puertos, 8 productos comerciales, 17 rutas, 27 hitos y un sistema completo de seguros/crédito.

## Inicio rápido

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

O instálalo globalmente:

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## Cómo funciona

Este paquete descarga el binario precompilado de Portlight para tu plataforma desde GitHub Releases y lo almacena localmente. No se requiere instalación de Python.

| Preocupaciones | Detalles |
|---------|--------|
| **Network** | Solo HTTPS a la CDN de `github.com` |
| **Filesystem** | Escribe solo en la caché del usuario (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | Suma de verificación SHA256 en cada descarga |
| **Telemetry** | Ninguna. Sin seguimiento, sin análisis, sin comunicación con servidores externos. |
| **Platforms** | Windows (x64), macOS (x64/arm64), Linux (x64) |

## También disponible a través de pip

Si tienes Python instalado:

```bash
pip install portlight
```

## Seguridad

- Descarga binarios exclusivamente de `github.com` a través de HTTPS.
- Verificación de la suma de verificación SHA256 en cada descarga.
- Escribe solo en el directorio de caché específico del usuario; nunca modifica directorios del sistema.
- Sin telemetría, sin secretos, sin credenciales almacenadas.
- Sin acceso a la red más allá de la descarga inicial del binario.

Consulta [SECURITY.md](SECURITY.md) para obtener la política de seguridad completa.

## Licencia

MIT

Desarrollado por <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
