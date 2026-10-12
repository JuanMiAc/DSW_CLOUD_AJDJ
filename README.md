# Plataforma de Simulación de Infraestructura Cloud con Asistente de IA

Esta plataforma web permite a los usuarios diseñar, presupuestar y simular el despliegue de arquitecturas Cloud de forma guiada, contando con el soporte de un asistente virtual basado en Inteligencia Artificial.

Este proyecto se desarrolla dentro del marco del módulo de Desarrollo de Aplicaciones Web (**2º DAW / DSW**).

---

## Estado Actual (Final de la UT1)
Actualmente, el proyecto ha finalizado su **Fase de Planificación, Arquitectura y Diseño Conceptual**. El repositorio contiene los modelos de datos, diagramas de clases, la verificación del entorno correcto y la documentación técnica necesaria. La fase de codificación, creación de la base de datos e implementación comenzará de forma oficial en la **UT2**.

---

## 🛠️ Stack Tecnológico Utilizado
*   **Backend:** Laravel 13.33.0 (PHP 8.5.4)
*   **Base de Datos:** MariaDB 11.8.6
*   **Gestor de Dependencias:** Composer 2.9.5 / npm 11.19.0
*   **Compilador Frontend:** Vite (Node.js v24.12.0)
*   **Arquitectura del Servidor:** Service Pattern (Desacoplamiento de lógica de negocio)
*   **Integración de IA:** API de Modelos de Lenguaje (LLM) con rol puramente consultivo
*   **Control de Versiones:** Git & GitHub

---

## Estructura Modular del Sistema
La aplicación está diseñada de forma modular bajo una arquitectura limpia, dividida en 12 bloques funcionales:
1. **Usuarios:** Registro y control de accesos por roles (RBAC).
2. **Catálogo:** Servicios Cloud simulados y tarifas base.
3. **Proveedores / Regiones:** Zonas geográficas y latencias ficticias.
4. **Proyectos:** Entornos de trabajo de los clientes.
5. **Requerimientos:** Validación de necesidades previas al diseño.
6. **Arquitecturas:** Planos lógicos y topologías Cloud.
7. **Carrito:** Preselección temporal de recursos antes de la compra.
8. **Presupuestos:** Congelación de tarifas comerciales inmutables.
9. **Pedidos:** Formalización de la intención de compra basada en presupuestos aprobados.
10. **Pagos:** Simulación de transacciones financieras y rollback inmediato ante fallos.
11. **Despliegues:** Simulación asíncrona del aprovisionamiento técnico.
12. **Auditoría / IA:** Registro inmutable (Append-Only) y analíticas de seguridad.

---

## Requisitos, Instalación y Ejecución

### Requisitos Mínimos del Sistema
*   Servidor Ubuntu con PHP 8.5 o superior instalado.
*   Gestor de bases de datos MariaDB/MySQL activo.
*   Composer y Node.js configurados en el entorno global.

### Pasos para Poner el Proyecto en Funcionamiento
1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com
   cd proyecto-laravel
   ```
2. **Instalar dependencias del backend:**
   ```bash
   composer install
   ```
3. **Instalar dependencias del frontend:**
   ```bash
   npm install
   ```
4. **Configuración del Entorno Local:**
   Duplicar la plantilla de variables de entorno para crear el archivo de configuración local:
   ```bash
   cp .env.example .env
   ```
   *(Nota: Editar el nuevo archivo `.env` configurando los accesos locales de tu servidor MariaDB en las variables `DB_DATABASE`, `DB_USERNAME` y `DB_PASSWORD`).*

5. **Levantar el Servidor de Desarrollo:**
   ```bash
   php artisan serve
   ```
   La aplicación pasará a estar disponible en tu navegador a través de la URL de comprobación: `http://127.0.0`

---

##  Política de Contribución (Git & Commits)
Para mantener el repositorio limpio y organizado, el equipo sigue de forma estricta la norma **Conventional Commits** para el historial de versiones:
*   `feat(...)`: Nuevas funcionalidades del sistema.
*   `fix(...)`: Corrección de errores o bugs de código.
*   `docs(...)`: Cambios exclusivos en los archivos de documentación.
*   `refactor(...)`: Optimización de código fuente sin alterar su comportamiento.

*Nota de seguridad:* Está estrictamente prohibido subir el archivo `.env` al repositorio público o privado. Todos los secretos se manejan de forma local.

---

## Equipo de Trabajo y Roles
*   **Ángel:** Desarrollo Backend / Configuración y control del flujo de peticiones.
*   **Damián:** Arquitectura de Software / Planificación de Clases de Servicio y reglas de negocio.
*   **Juan Francisco:** Modelado de Base de Datos / Diseño conceptual de esquemas y relaciones de datos.
*   **Yoel:** Desarrollo Frontend / Diseño de interfaz de usuario y maquetación de vistas conceptuales.

