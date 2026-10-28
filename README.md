# Módulo de gestión de devoluciones y reclamos — Mercado Libre

Trabajo Práctico Integrador y Progresivo (TPI) de **Organización Empresarial**
Tecnicatura Universitaria en Programación a Distancia — Universidad Tecnológica Nacional (UTN)

## Descripción del sistema

Este repositorio aloja la documentación técnica de un módulo de software que centraliza y automatiza la gestión de **devoluciones y reclamos** de las compras en Mercado Libre (caso de estudio del TPI).

El comprador registra un reclamo desde su cuenta y el sistema recupera automáticamente los datos de la compra, el pago y el envío. Según el caso, el módulo notifica al vendedor, coordina con Mercado Envíos si el producto debe volver, solicita el reintegro a Mercado Pago y cierra el caso dejando información para medir tiempos y detectar problemas repetitivos.

> El módulo, la estructura del área de sistemas y los valores numéricos son propuestas académicas. No corresponden a datos ni a la estructura real de Mercado Libre.

## Integrantes

| Integrante | Rol en el trabajo |
|---|---|
| Valentino Mangini | Autor del trabajo (análisis, modelado y documentación) |

**Docentes:** Prof. Gabriela Martínez (titular); Prof. Carolina Bruno, Prof. Mario Raúl López y Prof. Andrea Ramos (adjuntos).

## Tablero de gestión

Seguimiento de las historias de usuario en GitHub Projects: **[PEGAR AQUÍ EL ENLACE AL TABLERO]**

## Contenido de la documentación

| Documento | Ubicación |
|---|---|
| Diagrama BPMN del proceso (editable, abre en [bpmn.io](https://demo.bpmn.io)) | [`docs/bpmn/proceso-devoluciones-reclamos.bpmn`](docs/bpmn/proceso-devoluciones-reclamos.bpmn) |
| Diagrama BPMN (imagen) | [`docs/bpmn/proceso-devoluciones-reclamos.png`](docs/bpmn/proceso-devoluciones-reclamos.png) |
| Historias de usuario | [`docs/historias-de-usuario.md`](docs/historias-de-usuario.md) |
| Indicadores de control y estándares | [`docs/indicadores-de-control.md`](docs/indicadores-de-control.md) |
| Entregas 1, 2 y 3 del TPI | [`docs/entregas/`](docs/entregas/) |

## Cómo se trabaja en este repositorio

- La rama `main` contiene solo documentación terminada.
- Cada documento se trabaja en una rama secundaria `docs/<tema>` y se integra a `main` mediante un Pull Request con revisión.
- Los mensajes de commit siguen el formato `tipo: descripción` (por ejemplo, `docs: agrega el diagrama BPMN del proceso`).
- Cada historia de usuario es un *issue* vinculado al tablero.

## Declaración de uso de IA

**Herramienta:** asistente de Inteligencia Artificial Generativa (Claude, de Anthropic).

**Propósito específico:** organizar la información de las Entregas 1, 2 y 3 dentro de la Entrega 4, proponer la estructura del diagrama BPMN y de los indicadores, redactar borradores de tablas y de este README, y dar formato visual a los documentos.

**Prompt principal y justificación.** Se cargó el enunciado de la Entrega 4 junto con las Entregas 1, 2 y 3 y se pidió resolver la Entrega 4 basándose en ellas, de forma prolija y ordenada. Se hizo así para mantener el mismo caso, los mismos nombres de entidades y las mismas metas ya definidas, en lugar de partir de cero.

**Límites del asistente que se tuvieron en cuenta:**

- Las entregas anteriores no tenían definidas las historias de usuario, por lo que el asistente las propuso a partir del flujo del proceso. Se revisó que cada una corresponda a un actor del BPMN.
- Los valores numéricos nuevos (plazo de 48 h, 5 días de resolución, 80 % de respuesta en plazo) son supuestos de diseño y no datos de Mercado Libre.
- El asistente no puede crear el repositorio, el tablero, los commits ni el Pull Request: eso se realizó directamente en GitHub.

**Correcciones humanas efectuadas sobre los resultados de la IA:**

> [COMPLETAR: describir con tus palabras las correcciones concretas que hiciste (qué cambiaste en el BPMN, qué indicador ajustaste o descartaste, qué historia reescribiste y por qué). Borrar este recuadro al terminar.]

El autor asume la responsabilidad por la veracidad y la coherencia conceptual del trabajo.
