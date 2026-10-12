# 🚌 EcuaBus - Plataforma de Transporte Interprovincial

Plataforma web centralizada para la gestión y venta de pasajes en Ecuador. Proyecto de Manejo y Configuración de Software.

## 👥 Equipo de Desarrollo (Roles SCM & ITIL)
* **Alisson Paredes:** Líder SCM, Revisor Supremo 1, Back-End Core, Auditoría & Emailing.
* **Katherine Moyolema:** Revisora Suprema 2, Módulo Cooperativa & Asientos.
* **Anahí Molina:** Módulo Frecuencias ANT & Hoja de Ruta.
* **Mateo Herrera:** Buscador, Pasajeros & Temporizador.
* **Julio Zurita:** Oficinista & Validación de Pagos.
* **Alina Ortiz:** Historial por Cédula & Módulo Chofer (Fase 2).

## 🚀 Arquitectura
* **Backend:** Java 17, Spring Boot 4.x
* **Base de Datos:** PostgreSQL / MySQL / H2
* **Seguridad:** Spring Security + JWT

## 🌿 Flujo de Trabajo (GitFlow)
* `main`: Código de producción. **Solo los Revisores Supremos aprueban PRs aquí.**
* `develop`: Rama de integración principal.
* `feature/*`: Ramas individuales para cada funcionalidad.

### Convención de Commits
Obligatorio usar [Conventional Commits]: `feat:`, `fix:`, `chore:`, `docs:`.
