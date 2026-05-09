# Setup: Workspace de Notion

## Bases de datos a crear

### 1. Clientes
Propiedades:
- Nombre (título)
- Instagram / Contacto (texto)
- Email (email)
- Teléfono (teléfono)
- Servicio habitual (select): Grabación | Mezcla | Master | Beat
- Primer contacto (fecha)
- Total sesiones (número)
- Notas (texto largo)

### 2. Proyectos
Propiedades:
- Nombre del proyecto (título)
- Cliente (relación → Clientes)
- Servicio (select): Grabación | Mezcla | Master | Beat License
- Estado (select): Pendiente | En progreso | Revisión del cliente | Entregado | Archivado
- Fecha de sesión (fecha)
- Deadline entrega (fecha)
- Precio acordado (número)
- Pagado (checkbox)
- Archivos (URL o texto)
- Notas del proyecto (texto largo)
- Seguimiento enviado (checkbox)

### 3. Beats
Propiedades:
- Nombre del beat (título)
- BPM (número)
- Key / Tonalidad (select): las 12 notas
- Mood (multi-select): Trap | Drill | R&B | Afro | Boom Bap | Latin | Dark | Chill | Energético
- Estado (select): En proceso | Listo | Publicado en BeatStars | Vendido
- Fecha de publicación (fecha)
- Precio exclusivo (número)
- Precio no exclusivo (número)
- Ventas (número)
- Link BeatStars (URL)
- Descripción generada (texto largo)

### 4. Contenido
Propiedades:
- Título / Idea (título)
- Semana (fecha)
- Tipo (select): Post | Story | Reel | BeatStars
- Estado (select): Idea | Redactado | Publicado
- Caption (texto largo)
- Hashtags (texto)
- Beat relacionado (relación → Beats)
- Proyecto relacionado (relación → Proyectos)

---

## Vistas recomendadas

- **Proyectos:** Kanban por Estado (ver de un vistazo qué está en cada fase)
- **Beats:** Galería con filtro Estado = "Listo" (beats listos para publicar)
- **Contenido:** Calendario semanal

---

## Primeros pasos manuales en Notion
1. Crear una página raíz llamada "Estudio Musical"
2. Dentro, crear las 4 bases de datos con las propiedades de arriba
3. Compartir el workspace con la integración de Claude (Settings → Connections)
