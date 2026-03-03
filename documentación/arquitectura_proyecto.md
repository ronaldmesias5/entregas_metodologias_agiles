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
│
├── 📚 documentación/                 # Documentación
│   ├── plan_de_trabajo.md            # Plan de sprints
│   ├── historias-usuario.md          # Historias de usuario
│   ├── arquitectura_proyecto.md      # Tecnologías y estructura
│   ├── bsededatos.drawio.svg         # MER
│   └── Sprints/                      # Backlogs sprints
│       └── backlog_sprint_1.md       # Backlog
│
├── 🚀 backend/                       # API y Lógica de Negocio
│   ├── src/
│   │   ├── controllers/              # Controladores
│   │   ├── services/                 # Lógica de negocio
│   │   ├── models/                   # Esquemas
│   │   ├── routes/                   # Rutas
│   │   ├── middleware/               # Autenticación, validación
│   │   ├── utils/                    # Funciones auxiliares
│   │   └── config/                   # Configuración
│   ├── tests/                        # Tests unitarios e integración
│   ├── .env                          # Variables de entorno
│   ├── package.json                  # Dependencias
│   └── server.js                     # Punto de entrada
│
├── 💻 frontend/                      # Interfaz de Usuario
│   ├── src/
│   │   ├── components/               # Componentes React
│   │   ├── pages/                    # Páginas
│   │   ├── services/                 # Llamadas a API
│   │   ├── styles/                   # CSS/Tailwind
│   │   ├── utils/                    # Funciones auxiliares
│   │   └── App.js                    # Componente raíz
│   ├── public/                       # Archivos estáticos
│   ├── package.json                  # Dependencias
│   └── .env                          # Variables de entorno
│
├── 🗄️ database/                      # Base de Datos
│   ├── migrations/                   # Migrations de esquema
│   ├── seeds/                        # Datos iniciales
│   └── schema.sql                    # Esquema completo
│
├── .gitignore                        # Archivos ignorados
├── docker-compose.yml                # Orquestación de contenedores
├── README.MD                         # Introducción proyecto
└── package.json                      # Root dependencies
```

---
