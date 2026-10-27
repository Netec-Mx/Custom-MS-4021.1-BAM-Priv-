# Setup Guide — Experiencia de inmersión en Copilot: Ejecutivos

[Volver al inicio](./)

Esta guía prepara el entorno común de las nueve actividades. Se realiza antes de iniciar los 100 minutos prácticos. No necesita máquinas virtuales, comandos de instalación, APIs, Power Automate ni acceso a sistemas productivos.

## 1. Descripción del entorno

Se utiliza una cuenta profesional o educativa de Microsoft 365 en un tenant habilitado para Microsoft Copilot, con Microsoft Teams, Outlook, OneDrive, Word y PowerPoint. El escenario usa archivos del laboratorio y una reunión de Teams creada por el participante. También utiliza los agentes Analista, Investigador, Facilitador y un agente basado en la plantilla Executive Briefing Agent.

Las funciones varían según la licencia, la habilitación administrativa, el despliegue por tenant y la versión de la aplicación. La existencia de «Copilot Chat» básico no garantiza acceso a todas las acciones de las prácticas.

## 2. Requisitos de hardware y conectividad

- Un ordenador compatible con Microsoft 365 y conexión estable a Internet. No se requiere GPU ni infraestructura local especial.
- Micrófono funcional para la práctica con Facilitador. Se recomienda usar auriculares.
- Navegador actualizado compatible con Microsoft 365 (por ejemplo, Edge o Chrome).
- Microsoft Teams en escritorio o web para reuniones; PowerPoint de Microsoft 365; Outlook nuevo para Windows específicamente si se van a importar los correos `.eml` mediante el método descrito a continuación.
- Espacio de OneDrive suficiente para un documento de Word y un libro Excel; no se requiere una máquina virtual.

## 3. Software y servicios

| Componente | Uso | Requisito funcional |
|---|---|---|
| Microsoft Copilot con acceso al trabajo | Análisis de agenda, prompts y recuperación de información | Acceso a la información corporativa permitida por Microsoft Graph |
| Microsoft Teams | Chat de Copilot, reunión programada y Facilitador | Licencia de Teams, agente permitido, opciones de Copilot activas |
| Outlook con Exchange Online | Calendario, correo y preparación de reuniones | Buzón corporativo con datos accesibles a Copilot |
| Nuevo Outlook para Windows | Importación masiva de `.eml` | Menú Configuración > Archivos > Importar; conexión a Internet |
| OneDrive para el trabajo | Almacenamiento compartido de los recursos | Archivos disponibles para la cuenta de laboratorio |
| Word / PowerPoint con Copilot | Documento de referencia y generación de presentación | Funciones de Copilot disponibles y habilitadas |
| Analista / Investigador | Análisis y búsqueda fundamentada | Agentes visibles y permitidos en Microsoft Copilot |
| Executive Briefing Agent | Briefing ejecutivo | Agente creado desde plantilla, publicado/compartido y accesible |

No se exige Copilot Studio, Microsoft Graph API, Claude de uso independiente ni ChatGPT. En la práctica de PowerPoint se utiliza el modo de creación/edición con Copilot que muestre la cuenta; si aparece un selector de modelo, se utiliza una opción habilitada por el tenant, sin presuponer disponibilidad universal de modelos específicos.

## 4. Licencias, cuentas y permisos

1. Verifique una licencia base de Microsoft 365 elegible y la licencia de Microsoft Copilot asignada al participante. En el temario la denominación «Copilot Premium» se interpreta funcionalmente como acceso empresarial a las capacidades de Microsoft 365 Copilot, no como nombre de una licencia de empresa que deba adquirirse literalmente.
2. Verifique Microsoft Teams licenciado. Si el plan base es «sin Teams», se necesita una licencia válida de Teams separada.
3. La cuenta debe disponer de buzón Exchange Online, OneDrive y acceso a Word, PowerPoint y reuniones de Teams. No se requiere acceso de administrador para ejecutar las prácticas una vez habilitadas las funciones.
4. Verifique en Microsoft Copilot > Agentes que se muestran **Analista** e **Investigador**. La disponibilidad depende de la licencia y la política del tenant.
5. Verifique que **Facilitador** puede activarse en una reunión de Teams programada. Administración puede requerir habilitar la aplicación Facilitador, las experiencias de Loop en Teams y otras políticas correspondientes. La prueba debe permitir generación de notas; para consultarlas después de la reunión, active transcripción según la configuración de la organización.
6. Verifique acceso al agente **Executive Briefing Agent** ya creado por Agent Builder a partir de su plantilla. La plantilla no implica que el agente exista automáticamente en todas las cuentas. Si todavía no existe, un responsable con permisos para crear/publicar agentes debe aprovisionarlo y compartirlo, con acceso a los archivos necesarios. Si el tenant no ofrece la plantilla o su publicación, esta práctica queda bloqueada: no se considera equivalente consultar a un agente diferente.
7. Para las operaciones en Outlook y Teams con varias personas utilice cuentas de laboratorio autorizadas. No otorgue accesos generales a los documentos por comodidad; respete los permisos del entorno.

Documentación oficial para validar requisitos:

- [Microsoft Copilot: requisitos](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-copilot-requirements)
- [Licencias elegibles de Microsoft Copilot](https://learn.microsoft.com/en-us/microsoft-365/copilot/copilot-license-options)
- [Preparar Facilitador en Teams](https://learn.microsoft.com/en-us/microsoftteams/facilitator-teams)
- [Plantilla Executive Briefing Agent](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-template-executive-briefing)

## 5. Preparación del entorno y de los recursos

### Crear el espacio de archivos en OneDrive

1. Inicie sesión en [Microsoft Copilot](https://copilot.cloud.microsoft/) y en [OneDrive](https://www.microsoft365.com/launch/onedrive) con la misma cuenta corporativa.
2. En OneDrive cree una carpeta `Laboratorio-Grupo-Horizonte`.
3. Descargue y cargue en esa carpeta:
   - [Dossier_comite_canal_digital.docx](./recursos/Dossier_comite_canal_digital.docx).
   - [Indicadores_operativos_2026.xlsx](./recursos/Indicadores_operativos_2026.xlsx).
4. Abra ambos archivos en Word/Excel. Compruebe que el documento muestra las opciones A = 8, B = 18 y C = 31 millones UM y que el libro tiene las hojas `Base_Datos` y `Diccionario`.
5. Si Excel muestra un aviso de recálculo, permita que se actualicen las fórmulas y guarde el archivo. Las columnas Margen y SLA deben mostrar números, no errores o celdas vacías.
6. Si otra persona va a colaborar en Teams, comparta únicamente la carpeta/documento concreto con ese participante mediante los permisos previstos para el laboratorio. No lo configure como acceso público.

### Importar la agenda para Copilot en Teams

1. Descargue [Agenda_ejecutiva_noviembre_2026.ics](./recursos/Agenda_ejecutiva_noviembre_2026.ics).
2. Abra Outlook en la Web o nuevo Outlook; vaya a Calendario > Agregar calendario > Cargar desde archivo. Seleccione el `.ics` y el calendario de trabajo de la cuenta de laboratorio; importe los eventos. Si desea que Microsoft Copilot pueda encontrarlos mediante los permisos habituales de su cuenta, no dependa de que los eventos de un calendario externo compartido estén indexados.
3. Compruebe los eventos del 2 al 6 de noviembre de 2026. En especial, el 3 de noviembre entre 09:30 y 10:00 existen dos compromisos simultáneos y el 4 de noviembre entre 09:30 y 10:00 hay otro conflicto.
4. El archivo usa horas locales flotantes: Outlook aplica el huso horario configurado en el calendario del participante. El escenario tiene fechas de referencia fijas. Si se ejecuta después de esa semana, reubique los eventos a una semana futura conservando nombres, prioridades y solapamientos y ajuste en los prompts el intervalo de fechas.
5. No debe convertir automáticamente los eventos importados en invitaciones a otras personas. Son elementos de demostración; su modificación solo se efectúa en el calendario de laboratorio.

Documentación de Microsoft: [Importar un calendario ICS en Outlook](https://support.microsoft.com/en-us/outlook/import-or-subscribe-to-a-calendar-in-outlook-com-or-outlook-on-the-web).

### Preparación del correo de prueba

Esta actividad necesita mensajes reales en el buzón de prueba para que Copilot en Outlook pueda resumir un hilo. Los `.eml` se proporcionan para importarse, no solo para leerse en el navegador.

1. Descargue los cuatro archivos y guárdelos en una misma carpeta local `Correos-Horizonte` (sin subcarpetas):
   - [01_Hilo_comite.eml](./recursos/Correos/01_Hilo_comite.eml)
   - [02_Hilo_comite.eml](./recursos/Correos/02_Hilo_comite.eml)
   - [03_Hilo_comite.eml](./recursos/Correos/03_Hilo_comite.eml)
   - [04_Accion_continuidad.eml](./recursos/Correos/04_Accion_continuidad.eml)
2. En nuevo Outlook para Windows, abra Configuración > Archivos > Importar > Iniciar importación (algunas versiones muestran Configuración > General > Importar). Seleccione la carpeta `Correos-Horizonte`, la cuenta de laboratorio y una carpeta de correo creada para el ejercicio, por ejemplo `LAB-Horizonte`.
3. Verifique que aparecen tres mensajes con el asunto «Decisión Q4 | Canal Digital | Comité Directivo» y un cuarto con asunto «Acción necesaria | Continuidad del servicio y respaldo». Si el cliente no los agrupa en un solo hilo, consulte primero cada mensaje; la agrupación depende de los metadatos y ajustes de Outlook.
4. Para probar el resumen de conversación, confirme que Outlook con Copilot puede acceder a los mensajes importados. La indexación de Exchange puede requerir tiempo. Si no se muestran o Copilot no los recupera, el tenant debe ofrecer un buzón de laboratorio con un hilo equivalente enviado y recibido normalmente; un archivo `.eml` abierto localmente no reemplaza mensajes indexados en el buzón.
5. No envíe respuestas reales a las direcciones de ejemplo contenidas en los correos. Mantenga cualquier borrador sin enviar o utilice una cuenta de pruebas de la organización expresamente autorizada.

Documentación de Microsoft: [Importar archivos EML en nuevo Outlook para Windows](https://support.microsoft.com/en-us/outlook/bulk-import-eml-files-in-new-outlook).

### Programar una reunión real de prueba para las prácticas 3 y 4

La importación de eventos `.ics` no crea una reunión de Teams con transcripción ni habilita Facilitador automáticamente. Prepare por separado una reunión de Teams:

1. En Calendario de Teams seleccione Nueva reunión y programe «Preparación estratégica — Grupo Horizonte» para el momento de ejecución de las prácticas 3 y 4. Agregue una cuenta de prueba colaboradora, si está disponible, y active la opción de reunión de Teams.
2. Pegue en la descripción:

   ```text
   Objetivo: preparar el Comité Directivo sobre estabilización del Canal Digital.
   Agenda: (1) hallazgos sobre SLA e incidentes; (2) comparación A/B/C;
   (3) riesgo de invertir sin causa raíz; (4) propuesta de decisión y responsables.
   No existe todavía una alternativa autorizada por el Comité.
   ```

3. Abra el `Dossier_comite_canal_digital.docx` desde OneDrive, copie su enlace interno de uso autorizado e inclúyalo en la invitación o chat de la reunión. No cree un enlace público.
4. Abra el chat asociado a la reunión programada y publique un mensaje de preparación breve usando esta información: «Se contrastarán tres inversiones posibles: 8, 18 y 31 millones UM. El equipo aún no tiene aprobación final. Revisaremos riesgos, responsables y criterios de salida del piloto». Así existirá contexto real de reunión al que Copilot pueda tener acceso.
5. En Opciones de reunión > Copilot y otras IA, habilite Copilot y Facilitador según permisos del tenant. La funcionalidad Facilitador solo está diseñada para reuniones programadas; no la pruebe en «Reunirse ahora», llamadas 1:1 ni reuniones de canal.
6. Para poder consultar contenido después, configure la transcripción con consentimiento de los participantes y conforme a la política del tenant. Si no hay autorización para transcribir, puede realizar la parte de toma de notas en vivo si está habilitada, pero no dé por disponible el resumen posterior.

Para probar los diálogos de la práctica 4 se puede realizar la reunión entre dos participantes o usar una sesión de prueba autorizada en la que se expresen verbalmente las cuatro decisiones indicadas en la guía. El valor principal de la práctica es comprobar que Facilitador convierte una conversación efectivamente realizada en notas accionables.

Documentación de Microsoft: [Facilitador en reuniones de Teams](https://support.microsoft.com/es-es/teams/copilot/facilitator-in-microsoft-teams-meetings) y [Preparación de reuniones con Copilot](https://support.microsoft.com/es-es/outlook/prepare-for-your-meeting-with-copilot).

### Comprobar la plantilla Executive Briefing Agent

1. En Microsoft Copilot > Agentes, localice el agente publicado para el curso y compruebe que está basado en la plantilla `Executive Briefing Agent`.
2. Abra el agente y pregunte «¿Qué tipo de briefing ejecutivo puedes preparar?». Compruebe que contesta y que puede utilizar las fuentes habilitadas.
3. Asegure que el dossier Word y, si corresponde, el chat de reunión se encuentran dentro de su alcance de permisos y fuentes de conocimiento. Si el agente no recupera el dossier, el responsable debe corregir el acceso o permitir adjuntar el archivo directamente en la interacción; no atribuya datos que el agente no haya recuperado.
4. No cargue datos sensibles ni comunicaciones internas reales para improvisar el escenario del laboratorio.

## 6. Verificación del alistamiento

La preparación se considera suficiente cuando se comprueban funcionalmente estos puntos, sin completar una bitácora:

- Microsoft Copilot puede abrir un chat con datos de trabajo desde la cuenta del participante y encuentra el dossier si se selecciona como referencia.
- En el calendario aparecen los dos conflictos intencionales de noviembre de 2026.
- Outlook muestra tres mensajes del hilo y un correo independiente; el botón de Resumen por Copilot aparece sobre un mensaje o hilo compatible.
- La reunión de Teams programada existe, contiene la agenda y muestra las opciones esperadas de Copilot/Facilitador.
- PowerPoint abre el documento de Word como referencia o permite elegirlo para crear una presentación.
- Los agentes Analista, Investigador y Executive Briefing Agent se abren y aceptan solicitudes con el alcance adecuado.
- El Excel abre las hojas, presenta los valores calculados y tiene 27 registros mensuales (3 líneas × 9 meses).

## 7. Consideraciones, costos, seguridad y limpieza

- Se requieren licencias organizacionales; el ZIP no incluye licencias ni aprovisionamiento de servicios. No presuponga que un trial o Copilot Chat sin licencia cubre Facilitador, Analista, Investigador y la generación de presentaciones.
- La configuración del tenant puede bloquear datos del trabajo, adjuntos, agentes, transcripción, web o modelos. No eluda las políticas del administrador.
- Revise antes de enviar: Copilot no aprueba presupuestos ni sustituye el juicio ejecutivo. No envíe mensajes o invitaciones externas ni autorice gastos desde el laboratorio.
- El archivo `.ics` usa la semana del 2 al 6 de noviembre de 2026. Si se usa con posterioridad, adapte los eventos como se indicó.
- Al finalizar, elimine del calendario los eventos importados del escenario, archive o borre la carpeta `LAB-Horizonte`, la reunión de prueba y los archivos de OneDrive cuando ya no se necesiten. Conserve solo presentaciones/briefings que vaya a utilizar como productos del ejercicio.
- No se han verificado estas interfaces con un tenant autenticado en este paquete. Las rutas se contrastaron con documentación oficial de Microsoft y deben comprobarse en el tenant donde se imparta el curso.

[Volver al índice del curso](./)
