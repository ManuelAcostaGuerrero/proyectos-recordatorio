# Arquitectura Global — Sistema Inteligente de Recordatorios y Gestión Empresarial

## Arquitectura General

```txt
Frontend (React + Next.js)
        │
API REST + WebSocket
        │
Backend (Node.js + Express)
        │
Servicios Internos
│
├── Auth Service
├── User Service
├── Company Service
├── Task Service
├── Calendar Service
├── Notification Service
├── Audit Service
└── Report Service
        │
Base de Datos (PostgreSQL)
```

## Jerarquía Organizacional

SUPER ADMIN
→ ADMIN GENERAL
→ GERENTE
→ ADMINISTRADOR
→ CONTADOR
→ SUPERVISOR
→ OPERADOR / EMPLEADO

## Estados de Tarea

- Pendiente
- En proceso
- En revisión
- Observada
- Completada
- Vencida
- Reprogramada
- Cancelada

## Reglas Inteligentes

- Una tarea no puede cerrarse si existen subtareas pendientes.
- Las visualizaciones también se registran en auditoría.
- El calendario siempre muestra la prioridad más crítica del día.
- Las tareas completadas pueden reprogramarse generando historial.

## Base de Datos Principal

- users
- roles
- permissions
- companies
- branches
- departments
- tasks
- subtasks
- reminders
- notifications
- audit_logs
