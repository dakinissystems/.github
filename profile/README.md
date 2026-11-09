<p align="center">
  <img src="./banner.png" alt="Dakinis Systems Banner" width="100%">
</p>

<p align="center">
  <img src="./assets/akoenet.png" alt="AkoeNet" width="70">
  &nbsp;&nbsp;&nbsp;
  <img src="./assets/streamautomator.png" alt="StreamAutomator" width="70">
  &nbsp;&nbsp;&nbsp;
  <img src="./assets/core.png" alt="Dakinis One" width="70">
</p>

<div align="center">

# Dakinis Systems

### Software para operar el negocio, coordinar comunidades y programar contenido — sobre una plataforma compartida.

[![Organization](https://img.shields.io/badge/GitHub-dakinissystems-181717?logo=github)](https://github.com/dakinissystems)
![Status](https://img.shields.io/badge/Status-Active-success)
![Site](https://img.shields.io/badge/Web-dakinissystems.com-0A7A5A)

**Sitio:** [dakinissystems.com](https://dakinissystems.com) · **Estado del ecosistema:** [docs/STATUS](https://github.com/dakinissystems/dakinis-systems/blob/main/docs/STATUS.md)

</div>

---

## Qué resolvemos

Dakinis Systems construye un **ecosistema SaaS** con tres capas:

| Capa | Para quién | Productos |
|------|------------|-----------|
| **Negocio** | Operaciones, hospitality, finanzas | [Dakinis One](https://core.dakinissystems.com) · [LifeFlow](https://finance.dakinissystems.com) · [Hub](https://hub.dakinissystems.com) |
| **Creadores y comunidades** | Streamers y grupos online | [StreamAutomator](https://streamautomator.com) · [AkoeNet](https://akoenet.dakinissystems.com) |
| **Plataforma** | Todos los productos anteriores | Auth, Billing, AI, Search, Notifications, Knowledge, DES (UX compartida) |

No son apps aisladas con la misma marca: comparten identidad, facturación, búsqueda y experiencia de usuario cuando aplica.

---

## Productos

| Producto | Qué es | Abrir |
|----------|--------|-------|
| **Dakinis One** (código: Core) | Sistema de gestión empresarial modular — clientes, operaciones, hospitality | [core.dakinissystems.com](https://core.dakinissystems.com) |
| **LifeFlow** | Radar de flujo de caja (proyección, no solo histórico) | [finance.dakinissystems.com](https://finance.dakinissystems.com) |
| **Hub** | “Mi día primero” — atención y entrada al ecosistema | [hub.dakinissystems.com](https://hub.dakinissystems.com) |
| **StreamAutomator** | Programación y gestión de contenido para streamers | [streamautomator.com](https://streamautomator.com) |
| **AkoeNet** | Comunidades: chat, voz, DMs, Twitch / StreamAutomator | [akoenet.dakinissystems.com](https://akoenet.dakinissystems.com) · [Descargas](https://akoenet.dakinissystems.com/download) |

Madurez real por producto: [STATUS.md](https://github.com/dakinissystems/dakinis-systems/blob/main/docs/STATUS.md) (🟢 producción · 🟡 beta · 🟠 MVP · ⬜ roadmap).

---

## Arquitectura (vista)

```text
                    Cloudflare → Gateway (api.dakinissystems.com)
                                      │
              ┌───────────────────────┼───────────────────────┐
              ▼                       ▼                       ▼
           Auth IdP                  Hub                  Productos
              │                       │              One · LifeFlow · SA · AkoeNet
              └───────────────────────┴──────────┬────────────┘
                                                 ▼
                    Platform: Billing · Internal · AI · Search · Notifications · Knowledge
                                                 │
                                          DES / dakinis-shared (paquetes, no un servicio)
```

Detalle: [SYSTEMS.md](https://github.com/dakinissystems/dakinis-systems/blob/main/docs/SYSTEMS.md) · [ARCHITECTURE.md](https://github.com/dakinissystems/dakinis-systems/blob/main/docs/ARCHITECTURE.md)

---

## Repositorios públicos

| Repo | Rol |
|------|-----|
| [`dakinis-systems`](https://github.com/dakinissystems/dakinis-systems) | Orquestación: gateway, contratos, Docker, docs, scaffolds |
| [`dakinis-core`](https://github.com/dakinissystems/dakinis-core) | Dakinis One (web + API) |
| [`dakinis-streamautomator`](https://github.com/dakinissystems/dakinis-streamautomator) | StreamAutomator |
| [`akoenet-client`](https://github.com/dakinissystems/akoenet-client) | Cliente de AkoeNet. El API no tiene repositorio público |
| [`dakinis-landing`](https://github.com/dakinissystems/dakinis-landing) | Sitio dakinissystems.com |

Auth, Hub, los paquetes DES y las APIs de Billing, Search, Notifications, Internal, Knowledge y AI no están en la organización pública. Contratos y scaffolds: [`dakinis-systems`](https://github.com/dakinissystems/dakinis-systems).

Estándar de README: [DOC-STANDARDS.md](https://github.com/dakinissystems/dakinis-systems/blob/main/docs/DOC-STANDARDS.md)

---

## Stack (resumen)

Node.js · React · PostgreSQL · Redis · Railway · Cloudflare · Stripe · Sentry

---

## Contacto

- Web: [dakinissystems.com](https://dakinissystems.com)
- Organización: [github.com/dakinissystems](https://github.com/dakinissystems)

<div align="center">

**Hecho por Dakinis Systems**

</div>
