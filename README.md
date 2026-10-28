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

Seguimiento de las historias de usuario en GitHub Projects: https://github.com/users/valen04M/projects/1/views/1

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

**Propósito específico:** Se utilizó la IA como herramienta de apoyo conceptual y de consulta para:
- Guiar la estructuración de la entrega y el flujo de trabajo con Git y GitHub (manejo de ramas, commits y pull requests).
- Aportar ideas para la definición inicial del trabajo, la redacción de las historias de usuario y el diseño general de los procesos y documentos..

**Prompt principal y justificación.** Se consultó sobre cómo organizar las ideas de las entregas previas para definir las historias de usuario y estructurar la documentación del proyecto de forma clara. Ademas se pidio ayuda para hacer todo lo relacionado con git y github simplemente como guia.


**Límites del asistente que se tuvieron en cuenta:**

- - La IA solo actuó como guía y borrador inicial de ideas; no interactuó con la plataforma de GitHub ni ejecutó comandos del repositorio.
- Todas las decisiones finales, validaciones de los diagramas, métricas e integración en el repositorio fueron realizadas por el autor.

**Correcciones humanas efectuadas sobre los resultados de la IA:**

- Se revisaron, corrigieron y adaptaron los borradores de las historias de usuario al contexto real del trabajo.
- Se ajustaron los flujos del diagrama BPMN y los indicadores de control según los criterios propios del proyecto.


