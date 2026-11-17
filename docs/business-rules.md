# Reglas de negocio

Estas reglas reflejan solo lo confirmado por el cliente. Las condiciones aún no especificadas están listadas como preguntas abiertas; no se deben resolver mediante supuestos.

| ID | Regla confirmada | Detalle pendiente |
|---|---|---|
| BR-001 | En el armado desde cero, el total del sándwich es la suma de los precios de los ingredientes seleccionados. | Catálogo, moneda, impuestos, cantidades y redondeo. |
| BR-002 | Al modificar un sándwich predefinido, solo se cobran los extras agregados. | Definición de extra; cargos o créditos por quitar o reemplazar ingredientes. |
| BR-003 | Cada extra tiene un precio individual. | Quién define/actualiza los precios y si varían por tamaño o contexto. |
| BR-004 | El cliente puede seleccionar tamaños. | Lista de tamaños y su efecto sobre ingredientes y precio. |
| BR-005 | Se pueden configurar mínimos y máximos por etapa de selección. | Etapas, unidad contada, valores y tratamiento de incumplimientos. |
| BR-006 | El pedido por WhatsApp solo está disponible cuando el local está abierto. | Horarios, zona horaria, excepciones, definición exacta de “disponible” y comportamiento cerrado. |
| BR-007 | Los combos se postergan y no forman parte del alcance inicial. | Alcance y prioridad al retomarlos. |

## Reglas de cálculo conocidas

- Armado desde cero: total = suma de los precios de los ingredientes elegidos.
- Personalización de predefinido: cargo de personalización = suma de los precios de los extras agregados. No agregar un cargo base por modificarlo.

No se ha confirmado cómo interactúan tamaño, cantidades, descuentos, impuestos, envío, promociones o sustituciones con estos cálculos. No implementar esas interacciones hasta que se definan.
