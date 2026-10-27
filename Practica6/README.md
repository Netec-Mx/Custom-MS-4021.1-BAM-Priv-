# Práctica 6. Prepara una reunión estratégica con Executive Briefing Agent

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Solicitar al agente un briefing para la Alta Dirección a partir de fuentes autorizadas.
- Contrastar referencias, cifras y supuestos con el dossier oficial del escenario.
- Refinar el briefing para identificar riesgos, preguntas y decisiones pendientes.

## Duración aproximada:

- 12 minutos.

## Tabla de ayuda:

| Elemento | Información para la práctica | Finalidad |
|---|---|---|
| Aplicación | Microsoft Copilot > Agentes > Executive Briefing Agent | Ejecutar el agente publicado para el curso. |
| Agente requerido | Instancia creada mediante la plantilla Executive Briefing Agent | Debe estar aprovisionado y compartido previamente. |
| Documento | [Dossier_comite_canal_digital.docx](../recursos/Dossier_comite_canal_digital.docx) | Fuente de cifras y alternativas. |
| Reunión | Comité Directivo del 4 de noviembre de 2026 | Contexto del encargo ejecutivo. |
| Acceso | Cuenta autorizada con permisos sobre agente y fuentes | No existen credenciales predefinidas dentro del material. |
| Alistamiento | [Validar el agente](../SETUP_GUIDE.html#comprobar-la-plantilla-executive-briefing-agent) | Comprobar funcionalidad y acceso al documento. |

## Instrucciones

### Escenario de práctica

Antes de presentar las alternativas de inversión al Comité Directivo de **Grupo Horizonte**, necesitas preparar un resumen que permita a los participantes comprender rápidamente la situación del Canal Digital. La información debe incluir antecedentes, riesgos, preguntas estratégicas y decisiones pendientes. Utilizarás Executive Briefing Agent para generar un briefing ejecutivo a partir de la información disponible, identificando los aspectos que requieren especial atención antes de la reunión.

### Tarea 1. Abrir el agente asignado (2 min)

Paso 1. Entrar a Microsoft Copilot > `Agentes` y abrir el agente publicado basado en la plantilla `Executive Briefing Agent`.

Paso 2. Identificar la reunión «Preparación estratégica — Grupo Horizonte» y el Comité Directivo del 4 de noviembre de 2026.

Paso 3. Comprobar los permisos del agente sobre OneDrive y el dossier; no atribuir al agente acceso automático a mensajes o documentos no compartidos.

### Tarea 2. Generar un briefing ejecutivo (6 min)

Paso 1. Enviar al agente la siguiente solicitud integrada:

```text
Prepara un briefing ejecutivo para el Comité Directivo de Grupo Horizonte
sobre la estabilización del Canal Digital del 4 de noviembre de 2026.
Usa el documento «Dossier_comite_canal_digital.docx» de OneDrive y,
si realmente están accesibles, la invitación y las comunicaciones
relacionadas. No uses información que no puedas recuperar.

Redacta un documento ejecutivo breve que incluya: propósito y contexto;
evidencia numérica con su fuente; antecedentes comprobables;
las alternativas A/B/C (8/18/31 millones UM); riesgos y lagunas;
preguntas que probablemente hará el Comité; mensajes clave;
y recomendación condicionada con decisiones que siguen pendientes.

No atribuyas aprobación de presupuesto ni inventes acuerdos previos.
Separa claramente hechos del material, hipótesis e iniciativas futuras.
```

Paso 2. Revisar el borrador estructurado o el documento Word que genere el agente, de acuerdo con sus capacidades habilitadas.

Paso 3. Identificar las afirmaciones sin referencia y cualquier aprobación de presupuesto que no conste en el escenario.

### Tarea 3. Contrastar fuentes y refinar el informe (3 min)

Paso 1. Revisar las fuentes indicadas por el agente y contrastar en el dossier los datos: SLA de 93,9 % frente a 79,2 %, incidentes de 10 frente a 36 y tres alternativas por 8/18/31 millones UM.

Paso 2. Enviar el siguiente prompt de refinamiento en un turno independiente:

```text
Revisa el briefing anterior. Señala brechas de información en vez
de completarlas con supuestos. Añade tres preguntas que un director
debería formular antes de decidir y una condición verificable para
autorizar un piloto. Mantén sin aprobar las tres alternativas.
```

Paso 3. Abrir el Word generado, si existe, y verificar la separación entre hechos respaldados, hipótesis y propuestas de acción.

### Tarea 4. Verificar el briefing resultante (1 min)

Paso 1. Confirmar que incluya objeto de la reunión, decisión pendiente, al menos dos cifras fundadas, las tres alternativas, riesgos y preguntas previsibles.

Paso 2. Identificar explícitamente las fuentes que el agente no haya podido consultar; no presentar como fundamentado un resultado que no recupere el dossier. Si el agente no está disponible, completar el [alistamiento](../SETUP_GUIDE.html#comprobar-la-plantilla-executive-briefing-agent) en lugar de sustituirlo por otro agente.

### Resultado esperado

El Executive Briefing Agent entrega un briefing con contexto del Comité, dos o más cifras respaldadas, alternativas, riesgos, preguntas y recomendaciones condicionadas. Cada ausencia de fuente queda identificada y ninguna inversión aparece aprobada.

---

[Anterior](../Practica5/README.md) · [Recorrido](../) · [Siguiente](../Practica7/README.md)
