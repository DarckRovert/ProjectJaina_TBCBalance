# 📋 Registro de Cambios — ProjectJaina_TBCBalance

Todos los cambios notables de este proyecto están documentados en este archivo siguiendo el estándar [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/).

---

## [1.0.2] — 2026-11-22
### Registro de Prefijo IPC, Persistencia de Aura `950040` y Soporte Multi-Reino (Hito #386)
- **Canal `INTITBC` y Persistencia (`ProjectJaina_TBCBalance.lua`):**
  - Registrado explícitamente el prefijo `INTITBC` mediante `RegisterAddonMessagePrefix` (con fallback 3.3.5a).
  - Eliminado el temporizador de auto-ocultado de `4s` para mantener visible el indicador mientras el aura `950040` permanezca activa hasta recibir `"0"` o cambiar de mundo.
  - Ampliado filtro de reinos soportados a `inti|jaina|wanitos|forja` e implementado `SyncTbcScaleAura` + `.tbcscale` en servidor (`85_ContentProgressionGate.lua`).
- **Higiene de Código:** Eliminado archivo duplicado obsoleto `IntiTBCBalance.lua`.

---

## [1.0.1] — 2026-10-10
### Estabilización de Ecosistema y Gobernanza Oficial (Project Jaina)
- **Normalización de UI y Gráficos:** Compatibilidad con la compuerta de progresión temporal autoritativa y verificación de coeficientes de escalado para fases Vanilla (60) y TBC (70).
- **Homologación Documental:** Incorporación y actualización formal de `GOVERNANCE.md`, `LICENSE`, `NOTICE.md` y `SECURITY.md`.
- **Licencia Canónica:** Consolidación de licencia MIT 2026 bajo titularidad de DarckRovert & Project Jaina Team.
- **Validación de Runtime:** Verificado al 100% con compilador sintáctico `lua52_compiler.exe -p` con 0 errores y 0 warnings.

---

## [1.0.0] — 2026-10-04
### Lanzamiento Inicial — Ecosistema Project Jaina WotLK 3.3.5a
- Implementación de la arquitectura base para Project Jaina TBC Balance.
- Registro de comandos slash: `/tbcbal`.
- Persistencia de configuración en `TBCBalanceDB`.
- Compatibilidad certificada con cliente WotLK 3.3.5a (Build 12340) y directiva `Interface: 30300`.
