# Práctica 7. De los datos a la decisión: descubre insights con el agente Analista

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Analizar indicadores operativos a partir de un libro Excel utilizando Analista.
- Verificar el SLA ponderado, incidentes y tendencias entre periodos.
- Solicitar una recomendación ejecutiva basada en datos y sin aprobación de gastos.

## Duración aproximada:

- 15 minutos.

## Tabla de ayuda:

| Elemento | Información para la práctica | Finalidad |
|---|---|---|
| Aplicación | Microsoft Copilot > Agentes > Analista | Procesar el archivo y generar análisis. |
| Archivo | [Indicadores_operativos_2026.xlsx](../recursos/Indicadores_operativos_2026.xlsx) | Libro con 27 registros de enero a septiembre de 2026. |
| Hojas | `Base_Datos` y `Diccionario` | Datos y definiciones para cálculo. |
| Indicadores de contraste | SLA T1 ≈93,9 %; SLA T3 ≈79,2 %; incidentes T1=10 y T3=36 | Validar resultados del agente. |
| Meta interna | SLA de 92 % | Comparar cumplimiento. |
| Acceso | Agente Analista habilitado; cuenta de Microsoft 365 | Revisar [Setup Guide](../SETUP_GUIDE.html). |

## Instrucciones

### Escenario de práctica

La Dirección de Operaciones de **Grupo Horizonte** necesita comprobar con datos el deterioro del Canal Digital antes de evaluar una inversión. Para ello, dispones de un archivo Excel con indicadores de ingresos, costos, incidentes críticos y cumplimiento de tiempos de atención. Utilizarás el agente Analista para identificar tendencias, comparar resultados y detectar variaciones relevantes, convirtiendo los hallazgos en información que respalde las recomendaciones presentadas al Comité Directivo.

### Tarea 1. Abrir Analista y adjuntar los datos (2 min)

Paso 1. Abrir [Microsoft Copilot](https://copilot.cloud.microsoft/) > `Agentes` > `Analista`.

Paso 2. Seleccionar `Adjuntar contenido` y agregar [Indicadores_operativos_2026.xlsx](../recursos/Indicadores_operativos_2026.xlsx) desde OneDrive o el equipo.

Paso 3. Comprobar que el archivo aparezca en la solicitud y que el agente pueda acceder a su contenido.

### Tarea 2. Obtener el análisis de desempeño (7 min)

Paso 1. Enviar el siguiente prompt al agente:

```text
Analiza el archivo Excel adjunto «Indicadores_operativos_2026.xlsx».
Trabaja con la hoja Base_Datos, respeta las definiciones de Diccionario
y usa únicamente enero-septiembre de 2026.

Objetivos:
1. Identificar crecimiento o reducción de transacciones, ingresos
   y margen operativo por línea de negocio.
2. Calcular para Canal Digital el SLA ponderado del primer trimestre
   (enero-marzo) y del tercero (julio-septiembre), con
   SUMA(reclamos resueltos en 48 h) / SUMA(reclamos recibidos).
3. Comparar incidentes críticos en esos mismos periodos y detectar
   meses anómalos.
4. Señalar diferencias frente a la meta interna de SLA del 92 %.
5. Proponer dos líneas de acción con métricas de comprobación.

Muestra valores, periodos, método de cálculo y, si es posible, un gráfico.
No promedies porcentajes mensuales sin ponderación.
No pronostiques octubre-diciembre como si existieran datos observados.
```

Paso 2. Permitir el procesamiento del libro y revisar cualquier vista de cálculo, tabla o gráfico generado.

Paso 3. Identificar los métodos empleados y detectar promedios mensuales no ponderados, pronósticos presentados como hechos o conclusiones sin sustento.

### Tarea 3. Contrastar cálculos y solicitar una decisión sustentada (4 min)

Paso 1. Abrir el Excel y filtrar `Línea de negocio = Canal Digital`, comparando enero-marzo con julio-septiembre. Calcular el SLA agregado como SUMA(reclamos resueltos en 48 h) / SUMA(reclamos recibidos).

Paso 2. Comprobar como valores de control 10 y 36 incidentes críticos por trimestre, SLA ponderado de aproximadamente 93,9 % y 79,2 %, SLA agosto-septiembre de aproximadamente 75,1 % y 17 incidentes en agosto.

Paso 3. Enviar esta solicitud de interpretación ejecutiva:

```text
Con base en el análisis calculado, elabora una recomendación directiva
de máximo 180 palabras. Separa hechos numéricos, posibles causas NO
demostradas y medidas de mitigación. Relaciona la recomendación con
evaluar la alternativa B de 18 millones UM, sin tratarla como gasto
aprobado. Propón una métrica que se medirá antes y después del piloto.
```

### Tarea 4. Validar el análisis del agente (2 min)

Paso 1. Confirmar que el agente compare los dos trimestres, detecte el incumplimiento de la meta de SLA del 92 % en el tercer trimestre y presente al menos un hallazgo sobre incidentes críticos.

Paso 2. Solicitar corrección de un promedio incorrecto o de una columna calculada defectuosa, usando ingresos/costos y reclamos resueltos/recibidos; volver a adjuntar el libro si el agente no lo encuentra.

### Resultado esperado

Analista presenta el SLA ponderado de aproximadamente 93,9 % para enero-marzo y 79,2 % para julio-septiembre, incidentes de 10 y 36, el incumplimiento de la meta de 92 % y una recomendación que no confunde evaluación de la alternativa B con aprobación.

---

[Anterior](../Practica6/README.md) · [Recorrido](../) · [Siguiente](../Practica8/README.md)
