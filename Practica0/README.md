# Práctica inicial - De un prompt a un resultado ejecutivo

## Objetivo de la práctica:
Transformar una consulta vaga en una solicitud con contexto, fuente, formato y criterios de decisión. Prepare la cuenta según la [Setup Guide](../SETUP_GUIDE.html) y cargue el [dossier del Comité](../recursos/Dossier_comite_canal_digital.docx) en OneDrive.

## Duración aproximada:
- 10 minutos.

## Instrucciones 

### Escenario de práctica

Formas parte del equipo ejecutivo de **Grupo Horizonte**, una entidad financiera que enfrenta un aumento de incidentes y una disminución en la calidad de atención de su Canal Digital. La dirección necesita evaluar alternativas para mejorar el servicio y preparar una reunión del Comité Directivo. Tu responsabilidad será utilizar Copilot para convertir la información disponible en un resumen claro y confiable, que permita comprender el problema, identificar los riesgos y orientar las decisiones.

### Fase 1. Probar un prompt vago — 2 min

1. En Teams > Chat > Copilot, o en [Microsoft Copilot](https://copilot.cloud.microsoft/), abra el chat de trabajo.
2. Escriba:

   ```text
   ¿Qué debería hacer la dirección con el canal digital?
   ```

3. Observe si su respuesta contiene recomendaciones genéricas sin fuente. No las considere hechos.

### Fase 2. Crear un prompt con criterio ejecutivo — 4 min

1. Adjunte o referencie `Dossier_comite_canal_digital.docx` desde OneDrive y compruebe que aparece como fuente.
2. Envíe:

   ```text
   Actúa como asesor del Comité Directivo de Grupo Horizonte.
   Utiliza SOLO el documento adjunto «Dossier_comite_canal_digital.docx».
   Debo preparar la decisión sobre la estabilización del Canal Digital.

   Entrega un resumen ejecutivo de máximo 220 palabras que incluya:
   1. Dos hechos numéricos y su periodo.
   2. Riesgo operativo principal.
   3. Alternativas A, B y C con inversión en millones UM.
   4. Recomendación condicionada y datos que faltan.
   5. Una pregunta de decisión para el Comité.

   Distingue HECHOS, HIPÓTESIS y RECOMENDACIONES.
   No afirmes que existe presupuesto aprobado ni inventes información.
   ```

3. Revise que Copilot no agregue fechas, autorizaciones o regulaciones inexistentes.

### Fase 3. Corregir el resultado — 3 min

1. Introduzca este segundo prompt:

   ```text
   Revisa tu respuesta. Sustituye por «pendiente de validar» las
   afirmaciones sin respaldo en el dossier. Destaca el cambio del SLA
   entre enero-marzo y julio-septiembre, el denominador del indicador
   y el incremento de incidentes críticos. Mantén tono directivo neutral.
   ```

2. Compare con el dossier: SLA ponderado de Canal Digital cercano a 93,9 % en enero-marzo y 79,2 % en julio-septiembre; incidentes críticos 10 y 36, respectivamente.

### Fase 4. Comprobar — 1 min

La respuesta debe indicar que 8, 18 y 31 millones UM son alternativas, no montos aprobados. Si muestra una decisión inexistente, corríjala en el mismo chat.

## Validación final

Es posible identificar en pantalla la fuente utilizada, una hipótesis diferenciada de un hecho y la acción requerida. No necesita crear un archivo de conclusiones.

[Volver al recorrido](../) · [Continuar](../Practica1/README.md)