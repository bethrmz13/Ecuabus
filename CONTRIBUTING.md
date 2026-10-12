# Guía de Contribución - EcuaBus SCM

Bienvenido al repositorio de EcuaBus. Este documento define las políticas de Gobernanza SCM y el flujo de trabajo colaborativo que todos los integrantes deben seguir estrictamente.

## 1. Flujo de Trabajo (GitFlow)
Este proyecto utiliza el modelo GitFlow para la gestión de versiones.
* **`main`**: Rama de producción. Contiene únicamente código estable y versiones finales (releases).
* **`develop`**: Rama de integración. Todo el código nuevo se fusiona aquí antes de pasar a producción.
* **`feature/*`**: Ramas de desarrollo temporal. Cada integrante debe crear una rama con este prefijo para desarrollar su módulo (ej. `feature/temporizador-reserva`).
* **`hotfix/*`**: Ramas para corrección de errores urgentes en producción.

**REGLA DE ORO:** Está estrictamente prohibido hacer `git push` directamente a `main` o `develop`. Todo código debe integrarse a través de un Pull Request (PR)[cite: 2].

## 2. Convención de Commits (Conventional Commits)
El historial de Git será auditado. Todo commit debe explicar claramente qué se hizo usando los siguientes prefijos[cite: 2]:
* `feat:` - Nueva funcionalidad (ej. `feat(pagos): agrega validacion de comprobantes`).
* `fix:` - Corrección de un error (ej. `fix(auth): soluciona error de login`).
* `docs:` - Cambios en documentación.
* `chore:` - Mantenimiento, configuraciones, movimiento de carpetas o dependencias.

## 3. Reglas de Pull Requests y Revisión
1. El PR debe usar la plantilla oficial del repositorio (desglosando los commits).
2. Se requiere **al menos 1 aprobación** de un compañero distinto al autor del código.
3. Las líderes de revisión (Integrante 1 y Integrante 2) son responsables de verificar que el código cumpla con la arquitectura por capas antes de aprobar el Merge.
4. Si estamos en la Fase 2 del proyecto (ITIL), el PR debe mencionar el número del ticket que resuelve (ej. `Closes #5`).

## 4. Roles y Responsabilidades del Equipo
Para evitar cuellos de botella y conflictos de código, las tareas se dividen así:
* **Integrante 1 (Líder SCM):** Back-End Core, Seguridad JWT, Emailing SMTP, Admin Global y Dashboard de Auditoría ITIL.
* **Integrante 2 (Revisora Suprema):** Módulo Cooperativa, Gestión de Flota y Editor de Asientos.
* **Integrante 3:** Frecuencias ANT y Algoritmo de Hoja de Ruta.
* **Integrante 4:** Buscador, Filtros y Temporizador de Reserva.
* **Integrante 5:** Módulo Oficinista, Validación de Pagos, Generación PDF/QR y Wallet.
* **Integrante 6 (Fase 2):** Historial por Cédula y App Móvil Offline/QR para el Chofer.