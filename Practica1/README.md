# Práctica 1. Optimiza tu agenda ejecutiva con Copilot

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Identificar conflictos entre compromisos de una agenda ejecutiva utilizando Copilot.
- Priorizar reuniones conforme a su importancia estratégica.
- Reprogramar un evento de prueba y reservar un bloque de preparación en Outlook.

## Duración aproximada:
- 9 minutos.

## Tabla de ayuda:

| Elemento | Información para la práctica | Finalidad |
|---|---|---|
| Aplicaciones | Microsoft Teams (Copilot con datos de trabajo) y Calendario de Outlook | Analizar eventos y aplicar ajustes. |
| Archivo de agenda | [Agenda_ejecutiva_noviembre_2026.ics](../recursos/Agenda_ejecutiva_noviembre_2026.ics) | Importar los eventos al calendario del participante. |
| Periodo del escenario | 2 al 6 de noviembre de 2026 | Intervalo a consultar; adaptar en caso de reprogramación. |
| Reunión prioritaria | Comité Directivo, 4 de noviembre, 09:00–10:00 | Preservar este compromiso. |
| Cuenta de acceso | Buzón Exchange Online y licencia Copilot habilitada | Usar la cuenta de laboratorio del participante; no se entrega contraseña. |
| Preparación | [Setup Guide](../SETUP_GUIDE.html#5-preparacion-del-entorno-y-de-los-recursos) | Completar la importación y revisar conflictos. |

## Instrucciones


### Escenario de práctica

Como integrante de la Alta Dirección de **Grupo Horizonte**, tienes una agenda cargada de reuniones, algunas con horarios superpuestos, justo antes del Comité Directivo del 4 de noviembre de 2026. Necesitas priorizar los compromisos estratégicos, resolver conflictos de horario y reservar tiempo para preparar la reunión. Utilizarás Copilot para analizar tu calendario y organizar una agenda que te permita concentrarte en las actividades de mayor impacto.

### Tarea 1. Consultar la agenda del escenario (2 min)

Paso 1. Importar previamente el [archivo de agenda](../recursos/Agenda_ejecutiva_noviembre_2026.ics) según la [Setup Guide](../SETUP_GUIDE.md#5-preparacion-del-entorno-y-de-los-recursos) y abrir Outlook > Calendario.

Paso 2. Comprobar los eventos del 2 al 6 de noviembre de 2026 y revisar las prioridades indicadas en sus descripciones.

Paso 3. Abrir Microsoft Teams > Chat > Copilot con datos de trabajo; utilizar Teams como superficie de consulta y el calendario de Exchange Online como origen de los compromisos.

### Tarea 2. Detectar solapamientos con Copilot (3 min)

Paso 1. Enviar el siguiente prompt al chat de Copilot:

```text
Examina mi calendario del lunes 2 al viernes 6 de noviembre de 2026,
solo con los eventos a los que realmente tengo acceso. Identifica
solapamientos, reuniones críticas o altas y actividades delegables.
Indica fecha, horario, eventos en conflicto, prioridad y tu propuesta.
No modifiques nada. Si no puedes leer un evento, decláralo.
```

Paso 2. Contrastar las coincidencias con Outlook: martes 3 y miércoles 4 de noviembre, de 09:30 a 10:00.

Paso 3. Identificar las reuniones de prioridad alta y excluir de la decisión cualquier evento que Copilot no haya recuperado realmente.

### Tarea 3. Priorizar y reorganizar eventos de prueba (3 min)

Paso 1. Introducir este prompt sin autorizar cambios automáticos:

```text
Prioriza el Comité Directivo del 4 de noviembre de 09:00 a 10:00
y la validación de controles del 3 de noviembre de 09:00 a 10:00.
Propón mover reuniones de menor prioridad a horarios libres.
Identifica además un espacio de 45 minutos para preparar el Comité.
Propón antes de actuar; no envies invitaciones ni cambies reuniones.
```

Paso 2. Revisar en Outlook la disponibilidad del horario sugerido y modificar manualmente un evento de laboratorio de baja prioridad, sin cambiar compromisos de otras personas.

Paso 3. Crear un bloque privado de 45 minutos denominado «Preparar decisión Canal Digital» antes del Comité y conservar los eventos estratégicos.

### Tarea 4. Verificar los cambios en el calendario (1 min)

Paso 1. Actualizar la vista del calendario y comprobar que el evento reprogramado ya no se solapa con el prioritario.

Paso 2. Confirmar la presencia del bloque de preparación. En caso de no encontrar los eventos, revisar el calendario importado, los permisos de Copilot y el periodo seleccionado, adaptando fechas si se reubicó la agenda.

### Resultado esperado

El calendario de Outlook muestra el evento de baja prioridad reprogramado sin conflicto con la reunión prioritaria y un bloque privado de 45 minutos para preparar la decisión. Los cambios deben comprobarse en Outlook, no solo como sugerencias de Copilot.

---

[Anterior](../Practica0/README.md) · [Recorrido](../) · [Siguiente](../Practica2/README.md)
