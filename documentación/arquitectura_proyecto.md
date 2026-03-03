# Arquitectura del Proyecto - Sistema de Gestión y Producción de Calzado - CALZADO J&R

**Arquitecto:** Ronald Guerrero

---

## Stack Tecnológico General

### Backend

| Tecnología | Descripción |
|-----------|-----------|
| **Python 3.12+** | Lenguaje de programación principal |
| **FastAPI** | Framework web API REST asincrónica |
| **SQLAlchemy 2.0** | ORM (Object-Relational Mapping) |
| **Alembic** | Migraciones de base de datos |
| **JWT** | Manejo de tokens para autenticación |

### Frontend

| Tecnología | Descripción |
|-----------|-----------|
| **React 18+** | Librería de interfaz de usuario |
| **Vite** | Herramienta de build moderna |
| **TypeScript** | Superset de JavaScript con tipado estático |
| **TailwindCSS 4+** | Framework CSS utilitario |

### Base de Datos

| Tecnología | Descripción |
|-----------|-----------|
| **PostgreSQL 17+** | Sistema de gestión de base de datos relacional |
| **Docker Compose** | Orquestación de contenedores |

### Testing

| Capa | Herramientas | Descripción |
|-----|-------------|-----------|
| **Backend** | pytest + httpx | Testing unitario e integración en Python |
| **Frontend** | Vitest + Testing Library | Testing unitario y de componentes en React |

---

## Estructura del Proyecto

```
entregas_metodologias_agiles/
├── README.md
├── documentación
│   ├──arquitectura_proyecto.md
│   ├──historias_de_usuario.md
│   ├──basededatos.drawio.svg
│   └──plan_de_trabajo.md
├── sprint_1
│   ├──be (backend)
│   ├──fe (frontend)
│   ├──db (bases de datos)
│   └──backlog_sprint_1.md
├── sprint_2
│   ├──be (backend)
│   ├──fe (frontend)
│   ├──db (bases de datos)
│   └──backlog_sprint_2.md
├── sprint_3
│   ├──be (backend)
│   ├──fe (frontend)
│   ├──db (bases de datos)
│   └──backlog_sprint_3.md
└── ... (hasta Sprint 10)

```

---
