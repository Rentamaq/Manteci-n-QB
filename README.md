# Mantención QB

Panel público de equipos fuera de servicio (F/S) y operativos, alimentado con los reportes de los grupos de WhatsApp **Mecánicos QB** y **Supervisores TMF Rentamaq**.

- `index.html`: panel con 4 pestañas (Fuera de servicio, Equipos operativos, Dashboard KPI, Revisiones técnicas).
- `data.js`: datos de los equipos. Se actualiza a pedido con la búsqueda de las últimas 3 horas en los dos grupos (comando /actualiza-fsqb).
- `revtec.js`: alertas de revisión técnica de la semana, tomadas del correo "Rev. Tec. [Flota Teck QB]".

## Observaciones para mejorar el sistema (24-11-2026)

El panel funciona bien, pero la calidad de la información depende de cómo se reporta en WhatsApp. Hay dos problemas:

1. **Los usuarios no reportan de forma estandarizada.** Los avisos de falla en los grupos no siempre traen los datos necesarios: patente, n° interno, horómetro, ubicación, falla y hora de detención. Faltan datos, vienen en formatos distintos o solo con fotos, y eso impide registrar bien el equipo.
2. **Mantención no avisa cuándo el equipo queda operativo.** No hay una retroalimentación sistemática de que el equipo fue atendido y ya está operativo. Por eso muchos equipos siguen como F/S en el panel cuando en terreno ya están trabajando, y los tiempos de reparación quedan inflados.

Esto debe resolverse en una próxima mejora del sistema.
