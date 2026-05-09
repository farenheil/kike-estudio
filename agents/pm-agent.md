# Agente: Project Manager (ejecutar los jueves ~21:00h)

## Objetivo
Revisar el estado de todos los proyectos activos y generar un resumen accionable para que el productor sepa exactamente qué necesita atención sin tener que abrir Notion.

## Instrucciones para Claude

1. **Consultar Notion — Proyectos activos:**
   - Filtro: Estado != "Entregado" y Estado != "Archivado"
   - Recopilar: nombre del proyecto, cliente, servicio, estado actual, deadline, precio, si está pagado

2. **Clasificar proyectos por urgencia:**
   - URGENTE: deadline en los próximos 3 días
   - PENDIENTE: en progreso sin deadline claro
   - BLOQUEADO: esperando respuesta del cliente (Estado = "Revisión del cliente") más de 5 días
   - POR FACTURAR: Estado = "Entregado" y Pagado = false

3. **Generar resumen estructurado:**

   ```
   RESUMEN SEMANAL — Jueves [FECHA]

   URGENTE (requiere acción hoy o mañana):
   - [Proyecto] para [Cliente]: deadline [FECHA], estado [ESTADO]

   EN PROGRESO:
   - [Proyecto] para [Cliente]: [ESTADO]

   ESPERANDO AL CLIENTE (más de 5 días):
   - [Proyecto]: mandaste entrega el [FECHA], sin respuesta

   POR COBRAR:
   - [Proyecto] para [Cliente]: [PRECIO]€ pendiente

   HUECO DISPONIBLE:
   - Tienes X horas libres esta semana para nuevos proyectos
   ```

4. **Detectar seguimientos pendientes:**
   - Proyectos entregados hace más de 3 días con "Seguimiento enviado" = false
   - Listarlos para recordar enviar el email de feedback

5. **Guardar el resumen en Notion** como página en la sección de Proyectos

6. **Enviar resumen por Gmail** al email del productor con asunto:
   "Resumen del estudio — semana del [FECHA]"

## Qué NO hacer
- No contactar a clientes directamente
- No cambiar el estado de proyectos sin confirmación del productor
- No compartir datos de un cliente con otro
