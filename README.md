# Sistema de Help Desk Automatizado (UMG)

Este proyecto es una solución Full Stack de automatización para la gestión de tickets de soporte, desarrollado como Proyecto Final para el curso de Análisis de Sistemas II. Se utilizó una arquitectura de microservicios locales integrando **n8n**, **PostgreSQL** y un frontend interactivo en **HTML/JS**.

## 🚀 Arquitectura y Tecnologías
* **Motor de Automatización:** n8n (Workflows).
* **Base de Datos:** PostgreSQL (Persistencia local).
* **Frontend:** Interfaz web con KPIs dinámicos, ciclo CRUD y búsqueda en tiempo real.
* **Infraestructura:** Docker & Docker Compose.

## ⚙️ Instalación y Ejecución

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/geohengs/HelpDesk_UMG.git]

## Levantar los servicios:
Asegurarse de tener Docker instalado y ejecutar esto en la terminal:

docker-compose up -d

## Importar Workflows:
Accede a http://localhost:5678, ve a Workflows > Import from File y carga los archivos .json ubicados en la carpeta /workflows.

## Uso del Sistema:
Abrir el archivo index.html en tu navegador para ingresar tickets nuevos, o admin.html para visualizar y gestionar el panel de control.

## Ciberseguridad y Manejo de Errores
Seguridad: Las credenciales de la base de datos están protegidas estrictamente mediante variables de entorno configuradas vía .env e ignoradas en Git, evitando su exposición.

## Manejo de Errores:
Los flujos implementan estructuras robustas que previenen la caída del sistema ante peticiones de red malformadas o datos inválidos.