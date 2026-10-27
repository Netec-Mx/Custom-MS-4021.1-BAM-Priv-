# Práctica 5. Genera presentaciones ejecutivas para el Comité Directivo

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Crear una presentación ejecutiva a partir de un documento Word utilizando Copilot.
- Editar una diapositiva de alternativas para conservar cifras y estado de aprobación.
- Validar y guardar la presentación como producto de la actividad.

## Duración aproximada:

- 12 minutos.

## Tabla de ayuda:

| Elemento | Información para la práctica | Finalidad |
|---|---|---|
| Aplicación | PowerPoint para Microsoft 365 con Copilot habilitado | Crear y editar diapositivas. |
| Archivo fuente | [Dossier_comite_canal_digital.docx](../recursos/Dossier_comite_canal_digital.docx) | Usar como única fuente del contenido. |
| Alternativas | A: 8; B: 18; C: 31 millones UM | Mostrar importes sin aprobación presupuestaria. |
| Presentación de salida | `Comite_Grupo_Horizonte.pptx` | Guardar en OneDrive al terminar. |
| Cuenta | Microsoft 365 con función de generación desde archivo disponible | Usar el usuario y contraseña personales de laboratorio, no proporcionados en la guía. |
| Alistamiento | [Setup Guide](../SETUP_GUIDE.html) | Verificar permiso a Word, PowerPoint y OneDrive. |

## Instrucciones

### Escenario de práctica

El Comité Directivo de **Grupo Horizonte** necesita conocer la situación del Canal Digital y comparar tres alternativas de inversión: 8, 18 y 31 millones UM. Aunque dispones de un documento con los antecedentes e indicadores, debes transformar esa información en una presentación breve y fácil de comprender. Utilizarás Copilot en PowerPoint para elaborar una presentación ejecutiva que destaque los principales hallazgos, riesgos y alternativas, facilitando su evaluación por parte de los directivos.

### Tarea 1. Preparar PowerPoint y la fuente (2 min)

Paso 1. Abrir PowerPoint para Microsoft 365 e iniciar una presentación nueva.

Paso 2. Abrir Copilot desde la cinta o la interfaz disponible y seleccionar la función de creación con archivo de referencia o el modo edición.

Paso 3. Seleccionar `Referenciar archivo` o escribir `/` para localizar en OneDrive `Dossier_comite_canal_digital.docx`, comprobando el nombre del archivo elegido.

### Tarea 2. Generar la propuesta de presentación (7 min)

Paso 1. Introducir el siguiente prompt para construir el borrador a partir exclusivamente del dossier:

```text
Crea una presentación para el Comité Directivo de Grupo Horizonte a partir
EXCLUSIVAMENTE de «Dossier_comite_canal_digital.docx».
Audiencia: directores con 5 minutos para revisar alternativas.
Quiero 6 diapositivas como máximo:
1. Decisión que se solicita.
2. Evidencia: SLA e incidentes del Canal Digital, con los periodos precisos.
3. Alternativas A/B/C: inversiones 8/18/31 millones UM.
4. Comparación de riesgos, requisitos y brechas de información.
5. Recomendación CONDICIONADA con criterios de salida.
6. Decisión pendiente y próximos pasos.

Usa títulos que expresen conclusiones, no títulos genéricos.
Máximo 3 ideas por diapositiva; prioriza cifras verificables.
No atribuyas causalidad a un proveedor ni presentes presupuesto aprobado.
Agrega notas breves de exposición cuando la función lo permita.
```

Paso 2. Revisar el esquema propuesto por Copilot y confirmar su generación cuando corresponda, respetando las opciones que presente la versión habilitada en el tenant.

Paso 3. Verificar que las diapositivas no incluyan causas, cifras o autorizaciones ajenas al dossier.

### Tarea 3. Ajustar la diapositiva de alternativas (2 min)

Paso 1. Abrir la diapositiva que compara las alternativas A, B y C e introducir este prompt:

```text
Ajusta esta diapositiva para mostrar en columnas A: 8 millones UM,
B: 18 millones UM y C: 31 millones UM. Añade una línea visible:
«Escenarios de inversión sin aprobación presupuestaria».
```

Paso 2. Comprobar que las cifras y la advertencia sean legibles en PowerPoint; realizar manualmente el ajuste si la función de edición no puede aplicarlo.

### Tarea 4. Validar y guardar la presentación (1 min)

Paso 1. Revisar que la primera diapositiva explique la decisión solicitada y la última precise las condiciones pendientes.

Paso 2. Guardar en OneDrive `Comite_Grupo_Horizonte.pptx`. Tratarlo como producto de la práctica, no como un archivo preconstruido que deba figurar en el ZIP.

### Resultado esperado

El archivo `Comite_Grupo_Horizonte.pptx` contiene una presentación ejecutiva a partir del dossier, con alternativas A/B/C por 8/18/31 millones UM, cifras verificadas y una decisión explícitamente pendiente. El archivo queda guardado en OneDrive.

---

[Anterior](../Practica4/README.md) · [Recorrido](../) · [Siguiente](../Practica6/README.md)
