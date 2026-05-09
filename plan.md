# Plan: Ecosistema de Agentes para Estudio Musical

## Contexto

Productor musical con servicios de grabación, beat making, mezcla y mastering. Trabaja 8h diarias en otro empleo, lo que limita severamente el tiempo para gestionar el estudio. Situación actual: caos generalizado — clientes por WhatsApp/Instagram, Notion sin estructura, 7 beats en BeatStars sin constancia, Instagram activo pero sin calendario editorial. El objetivo es construir un equipo de agentes que cubra los procesos de negocio con mínima intervención manual.

---

## Los 4 Agentes

### Agente 1: La Recepcionista
Captar clientes, gestionar reservas y comunicación inicial.
- Cliente llega por Instagram → enlace en bio → Google Calendar Appointment Schedule
- Confirmación automática por Gmail
- Recordatorio 24h antes de la sesión

### Agente 2: El Project Manager
Llevar el estado de cada proyecto activo (mezcla, master, grabación).
- Al confirmar sesión → entrada en Notion con plantilla
- Jueves noche → revisión de proyectos activos + resumen
- 3 días post-entrega → Gmail pidiendo reseña

### Agente 3: El Asistente de Contenido
Mantener presencia en Instagram y BeatStars sin pensar qué publicar.
- Lunes → plan de contenido semanal (captions + hashtags listos para copiar-pegar)
- Genera descripciones para BeatStars de cada beat nuevo
- Guarda todo en Notion para revisión

### Agente 4: El Analista
Informe semanal de negocio.
- Domingo noche → recopila sesiones, proyectos, ingresos de Notion
- Genera informe + recomendación accionable

---

## Stack (coste 0€)

| Herramienta | Rol |
|---|---|
| Google Calendar | Reservas automáticas |
| Gmail | Comunicación automatizada |
| Notion | Hub de proyectos y contenido |
| Claude Code | Agentes programados (contenido, PM, analista) |

---

## Estado

- ✅ Gmail MCP autenticado
- ✅ Google Calendar MCP autenticado
- ✅ Notion MCP autenticado
- ✅ Estructura de proyecto creada

## Fases

### Fase 1 — Fundación
- [ ] Crear workspace Notion (bases de datos: Clientes, Proyectos, Beats, Contenido)
- [ ] Crear Google Calendar Appointment Schedule → enlace para bio

### Fase 2 — Automatización de clientes
- [ ] Email: confirmación de sesión
- [ ] Email: recordatorio 24h
- [ ] Email: seguimiento post-entrega

### Fase 3 — Agentes programados
- [ ] Agente lunes: plan de contenido
- [ ] Agente jueves: revisión de proyectos
- [ ] Agente domingo: informe semanal

### Fase 4 — Expansión (Mes 2+)
- [ ] Make.com: formulario → Notion automático
- [ ] Instagram API (publicación directa)
- [ ] BeatStars API cuando disponible
