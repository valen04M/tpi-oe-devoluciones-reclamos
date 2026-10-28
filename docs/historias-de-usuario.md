# Historias de usuario

Formato: **Como** [usuario], **quiero** [funcionalidad], **para** [beneficio]. Cada historia corresponde a un actor del [diagrama BPMN](bpmn/proceso-devoluciones-reclamos.png).

## HU-01 — Registrar un reclamo o devolución

**Como** comprador, **quiero** registrar un reclamo o solicitar una devolución desde mi cuenta y que el sistema recupere solo los datos de la compra, **para** no cargarlos a mano y que el caso quede asociado a la operación original.

Criterios de aceptación:
- Se puede iniciar el reclamo desde una compra propia indicando el motivo.
- El sistema recupera compra, pago y envío sin que el comprador los cargue.
- El reclamo queda en estado «abierto» y el comprador puede consultar su estado.

Vínculo: Pool *Comprador* y tarea «Recuperar datos de la compra, el pago y el envío». Entidades `Reclamo` y `Compra`.

## HU-02 — Responder un reclamo como vendedor

**Como** vendedor, **quiero** ver el reclamo recibido y responder aceptándolo o aportando evidencia dentro del plazo, **para** defender mi postura antes de que se resuelva el caso.

Criterios de aceptación:
- El vendedor recibe el aviso con los datos de la compra.
- Puede aceptar o disputar adjuntando evidencia dentro de las 48 h.
- Si el plazo vence sin respuesta, el caso continúa y el vencimiento queda registrado.

Vínculo: Pool *Vendedor* y compuerta G2. Entidad `Reclamo` (campo `estado`).

## HU-03 — Resolver un caso en disputa

**Como** analista de reclamos, **quiero** revisar la evidencia de ambas partes y registrar la resolución, **para** cerrar los casos en disputa con un criterio documentado y activar la devolución o el reintegro que corresponda.

Criterios de aceptación:
- Ve en una sola pantalla el reclamo, la evidencia y el estado del pago y del envío.
- Registra la resolución (a favor del comprador o sin reintegro) con su justificación.
- La resolución activa a Mercado Envíos y Mercado Pago y registra la fecha de cierre.

Vínculo: Lane *Analista de reclamos* y compuertas G3 y G4. Entidades `Reintegro` y `Envío`.

## Estados en el tablero

| Estado | Cuándo una historia está en este estado |
|---|---|
| Por hacer | El issue está creado con criterios de aceptación, pero todavía no hay rama de trabajo. |
| En progreso | Existe una rama `docs/…` abierta con commits y, si corresponde, un Pull Request en revisión. |
| Listo | Se hizo el merge del Pull Request a `main` y se verificaron los criterios de aceptación. |
