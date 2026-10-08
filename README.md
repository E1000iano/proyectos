# Proyectos · Tecnología Localiza Argentina

Portfolio y documentación de los proyectos que armamos en el área de Tecnología de Localiza Argentina (rent a car). Para cada uno: qué es, cómo funciona el proceso, por qué es mejor que lo que había y en qué estado está.

Este repo tiene sólo documentación, sin código.

**Página del portfolio:** [`index.html`](index.html). Con GitHub Pages activado, se ve en https://e1000iano.github.io/proyectos/.

## Estado de un vistazo

| Proyecto | Estado | Próximo paso | Documentación |
|---|---|---|---|
| Portal de Clientes | ✅ Listo para usar | Que las sucursales carguen su contenido | [01-portal-clientes](docs/01-portal-clientes.md) |
| Facturación automática de multas | ✅ En producción | Automatizar los medios de cobro | [02-facturacion-multas](docs/02-facturacion-multas.md) |
| Intranet con nuevo diseño | ✅ Publicada | Llegar más rápido a la información | [03-intranet](docs/03-intranet.md) |
| Taller · Stock de repuestos | 🛠️ En construcción | Descuento automático desde franquicias, reparaciones y services | [04-taller-stock](docs/04-taller-stock.md) |
| Taller · Gastos Sucursales | 🛠️ Propuesta de mejora | Elegir el diseño simplificado | [05-taller-gastos-sucursales](docs/05-taller-gastos-sucursales.md) |
| Servidor de cámaras | 🛠️ En armado | Terminar el acceso por link | [06-servidor-camaras](docs/06-servidor-camaras.md) |
| Servidor propio de RustDesk | 🛠️ En instalación | Terminar la instalación y migrar equipos | [07-rustdesk](docs/07-rustdesk.md) |
| Portal de postulaciones | 🛠️ Hecho, sin publicar | Casilla de correo, dominio y requisitos reales | [08-portal-postulaciones](docs/08-portal-postulaciones.md) |

## Qué tienen en común

Casi todos los proyectos persiguen lo mismo: **menos trabajo manual y los datos en un solo lugar**.
- La facturación de multas dejó de cargarse a mano en el ERP.
- El stock del taller deja la planilla.
- Las postulaciones dejan de llegar por WhatsApp o en papel.
- El acceso remoto y las cámaras pasan a infraestructura propia.

## Stack

La mayoría de los proyectos viven dentro de la app interna de Localiza:
- Backend en Python (FastAPI).
- Frontend en Next.js (React).
- Integraciones con el ERP Tango, las APIs de contratos y de flota de Localiza, Google Workspace y Multabot.

El Portal de postulaciones es una web aparte. Cámaras y RustDesk son servidores propios.

## Estructura

```
.
├── README.md          ← este archivo
├── index.html         ← página del portfolio
└── docs/              ← un documento por proyecto, con el proceso completo
```
