# Práctica 8. Delega la investigación: obtén una visión estratégica con el agente Investigador

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Realizar una investigación ejecutiva multifuente con el agente Investigador.
- Distinguir marcos de gestión, normas y controles técnicos con referencias verificables.
- Elaborar criterios y controles para una decisión de adopción de IA.

## Duración aproximada:

- 15 minutos.

## Tabla de ayuda:

| Elemento | Información para la práctica | Finalidad |
|---|---|---|
| Aplicación | Microsoft Copilot > Agentes > Investigador (Researcher) | Realizar la investigación. |
| Fuentes oficiales | [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework); ISO/IEC 42001; [Microsoft Copilot](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-copilot-requirements) | Contrastar las referencias resultantes. |
| Escenario | Adopción responsable de IA generativa en servicios financieros | Delimitar el encargo, sin información confidencial. |
| Horizonte de propuesta | Piloto de 90 días | Diseñar recomendaciones con indicadores. |
| Permisos | Agente Investigador y acceso web autorizado | Verificar en [Setup Guide](../SETUP_GUIDE.html). |

## Instrucciones

### Escenario de práctica

Después de conocer las posibilidades de Copilot, la Alta Dirección de **Grupo Horizonte** considera implementar un piloto de inteligencia artificial generativa de 90 días para mejorar la productividad de sus equipos. Antes de avanzar, necesita comprender las buenas prácticas de adopción, seguridad y gobierno de IA. Utilizarás el agente Investigador para consultar fuentes confiables, comparar recomendaciones y preparar una síntesis estratégica que facilite la evaluación de esta nueva iniciativa.

### Tarea 1. Abrir Investigador y delimitar fuentes (2 min)

Paso 1. Abrir [Microsoft Copilot](https://copilot.cloud.microsoft/) > `Agentes` > `Investigador (Researcher)`.

Paso 2. Habilitar las fuentes web oficiales cuando exista esa opción y verificar que el agente esté autorizado a consultarlas, sin añadir documentos privados innecesarios.

### Tarea 2. Encargar una investigación estratégica (7 min)

Paso 1. Enviar al agente la siguiente solicitud completa:

```text
Actúa como asesor de estrategia y gobierno de IA para Grupo Horizonte,
una organización de servicios financieros. Debemos evaluar cómo adoptar
asistentes y agentes de IA generativa para productividad de directivos,
sin automatizar aprobación de créditos ni utilizar datos personales reales.

Investiga fuentes OFICIALES y recientes (indica fecha o versión) sobre:
- NIST AI Risk Management Framework (AI RMF) y controles de gobierno.
- ISO/IEC 42001 como sistema de gestión, diferenciando norma de certificación.
- Controles de permisos, privacidad y datos para Microsoft Copilot empresarial.

Entrega un informe ejecutivo con: hallazgos con enlaces, qué exige cada
referencia y qué recomienda (sin inventar obligaciones jurídicas);
una comparación de tres marcos/enfoques; cinco riesgos operativos o de
gobierno; tres recomendaciones priorizadas para un piloto de 90 días;
y cuatro preguntas de decisión para Alta Dirección.

Distingue requisitos legales locales que necesitarían verificación por
la asesoría jurídica. No uses blogs comerciales como prueba principal.
Si una fuente no es accesible, reconócelo y no le atribuyas citas.
```

Paso 2. Revisar las fuentes y resultados conforme se generen, reconociendo que una investigación multifuente puede superar el tiempo operativo previsto si el servicio está lento.

Paso 3. Identificar las recomendaciones respaldadas y separar cualquier supuesto sobre legislación local que requiera revisión jurídica.

### Tarea 3. Validar fuentes y profundizar (4 min)

Paso 1. Abrir al menos dos citas de la respuesta y contrastarlas con páginas oficiales, como [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework) y [requisitos de Microsoft Copilot](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-copilot-requirements).

Paso 2. Diferenciar el marco de riesgos NIST AI RMF, el sistema de gestión ISO/IEC 42001 y los controles técnicos de Microsoft; no tratarlos como referencias equivalentes ni universalmente obligatorias.

Paso 3. Solicitar este refinamiento para el Comité:

```text
Reduce el informe a una recomendación para el Comité de una página.
Incluye tres controles de acceso/datos, dos controles de revisión humana
y tres indicadores verificables para un piloto de 90 días.
Para cada recomendación, cita la referencia que la sustenta y marca
qué aspectos requieren validación jurídica local.
```

### Tarea 4. Comprobar la recomendación final (2 min)

Paso 1. Revisar que el resultado incluya fuentes accesibles, al menos tres riesgos con medidas de mitigación y recomendaciones accionables para un piloto de 90 días.

Paso 2. Solicitar la eliminación o corrección de citas que no sustenten las afirmaciones, manteniendo diferenciadas las buenas prácticas y las obligaciones jurídicas sujetas a jurisdicción.

### Resultado esperado

Investigador entrega una síntesis estratégica con citas oficiales verificables, tres o más riesgos con mitigaciones, controles e indicadores para un piloto de 90 días, y una distinción clara entre orientaciones técnicas y requisitos jurídicos que deben validarse.

---

[Anterior](../Practica7/README.md) · [Recorrido](../) · [Setup Guide](../SETUP_GUIDE.html)