# Sprint 1 - Backlog Scrum
## Autenticación: Creación de Cuentas e Inicio de Sesión

**Scrum Master:** Andrés Gil  
**Sprint:** 1  
**Duración:** 15 días  
**Equipo:** Ronald (Arquitecto), Santiago (Bases de Datos), Andrés (Scrum Master)

---

## 📊 Estado de las Historias - Sprint 1

| Historia Pendiente | Historia en Desarrollo | Historia Terminada |
|:---|:---|:---|
| HU-002 - Validación y Activación de Cuentas | **HU-001** - Creación de Cuentas de Usuario | |
| HU-004 - Recuperación de Contraseñas | **HU-003** - Inicio de Sesión | |
| HU-006 - Creación de Catálogo | | |
| HU-009 - Visualización de Catálogo | | |
| HU-010 - Consulta de Catálogo | | |
| HU-011 - Sistema de Filtrado | | |
| HU-012 - Realización de Pedidos | | |
| HU-014 - Consulta de Estado de Pedidos | | |
| HU-015 - Actualización de Estado de Producción | | |
| HU-016 - Gestión de Inventario | | |
| HU-022 - Asignación de Tareas de Producción | | |
| HU-024 - Reporte de Avances | | |
| HU-025 - Confirmación de Finalización de Tareas | | |
| HU-026 - Notificación al Jefe de Tareas Completadas | | |
| HU-029 - Módulo de Notificaciones | | |
| HU-030 - Alertas al Jefe | | |
| HU-031 - Reportes de Pedidos | | |
| HU-033 - Suma de Producción | | |

---

## 📋 Historias de Usuario - Sprint 1

### HU-001: Creación de Cuentas de Usuario
**Prioridad:** Alta | **Story Points:** 8

Como usuario nuevo, Quiero crear una cuenta en el sistema, Para poder acceder a las funciones de la plataforma.

**Criterios de Aceptación:**
- El usuario puede registrarse con email y contraseña
- El sistema valida que el email sea único
- El sistema valida que la contraseña sea fuerte (mín 8 caracteres, mayúscula, número, símbolo)
- La cuenta se crea activa
- Se muestra mensaje de error si los datos son inválidos

**Tareas:**
1. Backend: Crear endpoint POST /api/auth/register
2. Backend: Implementar validación de email único
3. Backend: Implementar validación de contraseña fuerte
4. Frontend: Crear componente RegisterForm
5. Frontend: Integrar cliente API de registro
6. Database: Crear tabla usuarios con campos necesarios
7. Testing: Pruebas unitarias de validaciones

---

### HU-003: Inicio de Sesión
**Prioridad:** Alta | **Story Points:** 5

Como usuario registrado, Quiero iniciar sesión con mi email y contraseña, Para acceder a mi cuenta.

**Criterios de Aceptación:**
- El usuario puede iniciar sesión con credenciales válidas
- El sistema genera token JWT tras login exitoso
- El usuario obtiene error si credenciales son incorrectas
- La sesión permanece activa 
- El usuario puede cerrar sesión (logout)

**Tareas:**
1. Backend: Crear endpoint POST /api/auth/login
2. Backend: Implementar autenticación JWT
3. Backend: Crear endpoint POST /api/auth/logout
4. Frontend: Crear componente LoginForm
5. Frontend: Implementar context de autenticación
6. Frontend: Guardar token en localStorage
7. Testing: Pruebas de flujo de autenticación

---

**Creado por:** Andrés Gil (Scrum Master)
