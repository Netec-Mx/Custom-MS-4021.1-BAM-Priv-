# Práctica 2. Gestiona el correo ejecutivo en minutos

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Resumir conversaciones ejecutivas extensas utilizando Copilot en Outlook.
- Distinguir tareas urgentes de propuestas pendientes de autorización.
- Redactar una respuesta ejecutiva sin enviarla a destinatarios externos.

## Duración aproximada:

- 9 minutos.

## Tabla de ayuda:

| Elemento | Información para la práctica | Finalidad |
|---|---|---|
| Aplicación | Outlook con Microsoft 365 Copilot y buzón Exchange Online | Consultar mensajes y redactar el borrador. |
| Carpeta de trabajo | `LAB-Horizonte` | Ubicar los cuatro mensajes del escenario. |
| Asunto principal | `Decisión Q4 \| Canal Digital \| Comité Directivo` | Identificar los tres mensajes del hilo. |
| Plazos de referencia | 26 de octubre: restauración; 27 de octubre, 16:00: resumen ejecutivo | Priorizar solicitudes. |
| Archivos de entrada | [Cuatro correos EML](../SETUP_GUIDE.html#preparacion-del-correo-de-prueba) | Importar antes de comenzar. |
| Cuenta | Buzón de laboratorio autorizado | Iniciar sesión con las credenciales propias; no usar direcciones reales de clientes. |

## Instrucciones

### Escenario de práctica

Mientras preparas el Comité Directivo de **Grupo Horizonte**, recibes varios correos de las áreas de Operaciones, Tecnología y Riesgos con solicitudes urgentes, propuestas de inversión y asuntos pendientes. Revisar cada conversación manualmente consume tiempo y puede hacer que pases por alto información importante. Utilizarás Copilot en Outlook para resumir los mensajes, identificar compromisos prioritarios y preparar una respuesta ejecutiva, evitando presentar propuestas como decisiones ya aprobadas.

### Tarea 1. Localizar los correos del caso (1 min)

Paso 1. Importar los cuatro archivos EML conforme a la [Setup Guide](../SETUP_GUIDE.html#preparacion-del-correo-de-prueba) y abrir Outlook > `LAB-Horizonte`.

Paso 2. Buscar el asunto «Decisión Q4 | Canal Digital | Comité Directivo» y localizar los tres correos del 21, 22 y 23 de octubre de 2026; abrirlos por separado si Outlook no agrupa la conversación.

### Tarea 2. Generar y revisar un resumen (2 min)

Paso 1. Seleccionar en la conversación `Resumen por Copilot` o `Resumir` para sintetizar los mensajes disponibles.

Paso 2. Comprobar que el resumen distinga las alternativas por 8/18/31 millones UM, el piloto condicionado, la falta de aprobación y el plazo del 27 de octubre a las 16:00.

Paso 3. Introducir este prompt en el chat contextual de Outlook, cuando esté disponible:

```text
Resume esta conversación. Distingue decisiones aprobadas, propuestas
todavía abiertas, solicitudes, responsables y fechas límite.
Cita el mensaje de origen. No afirmes que se aprobó la opción B.
```

### Tarea 3. Priorizar solicitudes abiertas (3 min)

Paso 1. Abrir el cuarto correo «Acción necesaria | Continuidad del servicio y respaldo» y verificar el plazo del 26 de octubre para asignar la prueba de restauración.

Paso 2. Introducir el siguiente prompt en Copilot de Outlook con acceso a datos de trabajo:

```text
En la carpeta LAB-Horizonte busca los correos sobre Grupo Horizonte.
Ordena por urgencia las tareas abiertas: asunto, fecha límite, acción,
persona que solicita y tipo de decisión. Diferencia preparar una
propuesta de aprobar una inversión. Sustenta con cada mensaje.
```

Paso 3. Contrastar la prioridad de ambas solicitudes; si Copilot no permite buscar toda la carpeta, comparar manualmente los dos asuntos en vez de atribuirle una búsqueda que no realizó.

### Tarea 4. Redactar un correo ejecutivo sin enviarlo (2 min)

Paso 1. Abrir el último correo del hilo y seleccionar `Responder` > `Redactar con Copilot` o `Ayúdame a responder`, según la interfaz.

Paso 2. Introducir este prompt de redacción:

```text
Redacta una respuesta ejecutiva en español para Dirección de Operaciones.
Confirmamos que entregaremos antes del 27 de octubre a las 16:00 un
resumen de una página con SLA, incidentes, riesgos y responsables.
Los 18 millones UM son una alternativa PENDIENTE de aprobación.
Tono respetuoso y directo, máximo 120 palabras. No prometas gastar
ni iniciar un proyecto.
```

Paso 3. Revisar el borrador para comprobar su tono, extensión y ausencia de autorizaciones de gasto; dejarlo sin enviar a las direcciones de ejemplo del caso.

### Tarea 5. Verificar el borrador y los plazos (1 min)

Paso 1. Comprobar que el resumen refleje correctamente los plazos del 26 y 27 de octubre y que Outlook conserve visible el borrador.

Paso 2. Guardar o descartar el borrador. Si Copilot no encuentra los correos, comprobar que fueron importados al buzón Exchange y no solo abiertos en el equipo; considerar el tiempo de indexación.

### Resultado esperado

Outlook muestra un resumen de correo que distingue los plazos del 26 y 27 de octubre y un borrador de respuesta ejecutiva en español que no presupone aprobación de inversión ni se envía a direcciones del escenario.

---

[Anterior](../Practica1/README.md) · [Recorrido](../) · [Siguiente](../Practica3/README.md)
