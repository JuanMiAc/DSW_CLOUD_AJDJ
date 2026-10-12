# Plataforma de Simulación de Infraestructura Cloud con Asistente de IA

¡Bienvenidos al repositorio oficial del proyecto! Esta plataforma web permite a los usuarios diseñar, presupuestar y simular el despliegue de arquitecturas Cloud (AWS, Azure, etc.) de forma guiada, contando con el soporte de un asistente virtual basado en Inteligencia Artificial.

Este proyecto se desarrolla dentro del marco del módulo de Desarrollo de Aplicaciones Web (**2º DAW / DSW**).

##  Estado Actual (Final de la UT1)
Actualmente, el proyecto ha finalizado su **Fase de Planificación, Arquitectura y Diseño Conceptual**. El repositorio contiene los modelos de datos, diagramas de clases y la documentación técnica necesaria. La fase de codificación e implementación comenzará de forma oficial en la **UT2**.

---

##  Stack Tecnológico Previsto
*   **Backend:** Laravel 11+ (PHP 8.2+)
*   **Base de Datos:** MySQL / PostgreSQL
*   **Arquitectura:** Service Pattern (Desacoplamiento de lógica de negocio)
*   **Integración de IA:** API de Modelos de Lenguaje (LLM) con rol consultivo
*   **Control de Versiones:** Git & GitHub

---

##  Estructura Modular del Sistema
La aplicación está diseñada de forma modular bajo una arquitectura limpia, dividida en 12 bloques funcionales:
1. **Usuarios:** Registro y control de accesos por roles (RBAC).
2. **Catálogo:** Servicios Cloud simulados y tarifas base.
3. **Proveedores / Regiones:** Zonas geográficas y latencias ficticias.
4. **Proyectos:** Entornos de trabajo de los clientes.
5. **Requerimientos:** Validación de necesidades previas al diseño.
6. **Arquitecturas:** Planos lógicos y topologías Cloud.
7. **Carrito:** Preselección temporal de recursos.
8. **Presupuestos:** Congelación de tarifas comerciales inmutables.
9. **Pedidos:** Formalización de la intención de compra.
10. **Pagos:** Simulación de transacciones financieras y rollback.
11. **Despliegues:** Simulación asíncrona del aprovisionamiento técnico.
12. **Auditoría / IA:** Registro inmutable (Append-Only) y analíticas de seguridad.

---

##  Política de Contribución (Git & Commits)
Para mantener el repositorio limpio y organizado, el equipo sigue la norma **Conventional Commits**:
*   `feat(...)`: Nuevas funcionalidades.
*   `fix(...)`: Corrección de errores.
*   `docs(...)`: Cambios en la documentación.
*   `refactor(...)`: Optimización de código sin cambiar su función.

*Nota:* Está estrictamente prohibido subir el archivo `.env` al repositorio. Las variables de entorno de ejemplo se gestionan en `.env.example`.

---

## 👥 Equipo de Trabajo
*   **[Tu Nombre/Apodo]** - Desarrollo Backend / Integración de IA
*   **Damián Pérez Alemán** - Diseño de Base de Datos / Lógica de Negocio
*   **Juan Francisco Millet Acedo** - Arquitectura de Software / Frontend
