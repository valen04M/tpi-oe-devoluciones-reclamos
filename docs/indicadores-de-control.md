# Indicadores de control y estándares de desempeño

Los indicadores I1 a I4 salen de las metas de la Entrega 2. Los indicadores I5 a I7 controlan el funcionamiento del proceso modelado en BPMN. Los estándares de I5, I6 e I7 son valores de planificación propuestos para este trabajo, no datos de Mercado Libre.

| ID | Indicador | Cómo se calcula | Estándar | Fuente / momento |
|---|---|---|---|---|
| I1 | Tiempo de consulta de un caso | Tiempo de respuesta medido en cada consulta de la prueba | ≤ 2 s en el 95 % de las consultas | Pruebas de rendimiento |
| I2 | Integración de datos | Casos de prueba que recuperan compra, pago y envío ÷ casos de prueba totales | ≥ 95 % | Pruebas de integración |
| I3 | Cobertura de pruebas | Escenarios ejecutados ÷ escenarios definidos (incluye G1 a G4) | ≥ 90 % | Matriz de casos de prueba |
| I4 | Cumplimiento del cronograma | Avance real comparado con el Gantt | 7 semanas | Revisión semanal |
| I5 | Tiempo medio de resolución | Suma de (`fecha_cierre` − `fecha_apertura`) ÷ casos cerrados | ≤ 5 días corridos | Casos cerrados de la prueba |
| I6 | Respuesta del vendedor en plazo | Reclamos con respuesta dentro de 48 h ÷ reclamos notificados | ≥ 80 % | Registro de la compuerta G2 |
| I7 | Errores en reintegros | Reintegros con monto distinto al esperado ÷ reintegros procesados | 0 % | Pruebas sobre montos y estados |

## Auditoría técnica

| Qué se audita | Evidencia | Criterio |
|---|---|---|
| Versionado | Ramas, historial de commits y Pull Requests | Trabajo en ramas secundarias, commits descriptivos y al menos un PR con revisión |
| Proceso | Diagrama BPMN y diccionario de datos | Cada paso del BPMN usa entidades y campos que existen en la Entrega 3 |
| Requisitos | Historias de usuario y tablero | Cada historia tiene criterios de aceptación y un estado actualizado |
| Calidad | Resultados de los indicadores I1 a I7 | Cada indicador se compara con su estándar y el desvío queda registrado |

## Ciclo de control

Se mide cada indicador, se compara con el estándar y, si hay desvío, se abre un issue de corrección en el tablero que se resuelve en una rama con su Pull Request.
