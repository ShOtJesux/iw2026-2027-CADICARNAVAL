# Plan de Proyecto

## 1. Asignación de Roles
* **Product Owner + Desarrollo Backend:** Encargado del dominio del negocio (Carnaval de Cádiz) y definición de historias de usuario.
* **Scrum Master + Desarrollo Backend:** Encargado de la gestión de la metodología ágil y la coordinación del equipo.
* **Desarrollo Backend (Mayor carga):** Dedicación principal a la implementación técnica y lógica de negocio pesada.

---

## 2. Eventos de Scrum
* **Planificación del Sprint (Sprint Planning):** Al inicio de cada sprint (~1 hora). Sesión presencial o por videollamada para seleccionar las historias del *Product Backlog* que pasan al *Sprint Backlog*.
* **Reunión Diaria (Daily Scrum):** 2 a 3 veces por semana (o diaria de 15 min vía mensajería/presencial) respondiendo: qué hizo, qué hará y bloqueos.
* **Revisión y Retrospectiva (Sprint Review & Retrospective):** Al finalizar cada sprint (~45-60 min). Se comprueba el incremento entregable, se actualiza la documentación en `docs/` y se analizan mejoras del equipo.

---

## 3. Modelo de Trabajo
* **Flujo de ramas (GitFlow simplificado):**
  * `main` / `master`: Código estable de versiones entregadas (*releases*).
  * `develop`: Rama de integración para el sprint en curso.
  * `feature/nombre-historia`: Ramas individuales para el desarrollo de tareas de forma aislada.
* **Revisiones de código (Pull Requests):** Es obligatorio que al menos otro integrante revise y apruebe las *Pull Requests* antes de fusionar en `develop`.
* **Convenciones de commits:** Commits semánticos (ej. `feat: añadir módulo de sorteos`, `fix: corregir validación de autoría`).

---

## 4. Definición de "Done" (Terminado)
Una tarea o historia de usuario se considera completada únicamente si cumple:
1. El código compila correctamente mediante Apache Maven sin errores ni advertencias críticas.
2. Incluye pruebas automáticas asociadas (unitarias o de integración) que pasan con éxito.
3. Está integrado en `develop` tras una *Pull Request* revisada y aprobada por otro miembro.
4. La documentación correspondiente en `docs/` o comentarios técnicos han sido actualizados.
5. Se declaran y validan las partes asistidas por IA (en cumplimiento de `AGENTS.md`).

---

## 5. Acuerdos del Equipo
* **Comunicación:** Canal de mensajería instantánea para el día a día y correo electrónico para asuntos formales.
* **Resolución de conflictos:** Decisiones técnicas por consenso. En caso de bloqueo, decide el Product Owner o se consulta en tutorías.
* **Uso de IA:** Permitido como asistente de desarrollo. Todo código generado debe ser asumido, comprendido y revisado por quien firma el commit, registrando las herramientas en el repositorio.

---

## 6. Roadmap del Proyecto
1. **Hito 0 (Inicio):** Redacción conjunta del plan de proyecto (`docs/plan-proyecto.md`) y configuración inicial de la forja (GitHub, Maven y estructura base).
2. **Sprint 1 (Análisis y Núcleo):** Requisitos iniciales, configuración de la base de datos, gestión de usuarios/permisos y modelo de datos base (Ediciones y Agrupaciones).
3. **Sprint 2 (Funcionalidades principales - Back-office y Front-office):** Inscripciones, sorteos, programación de sesiones y calendario público.
4. **Sprint 3 (Evaluación, Archivo histórico y Despliegue final):** Sistema de evaluación/jurado, archivo histórico y despliegue definitivo del sistema.
