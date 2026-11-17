# Requisitos del producto

**Estado:** relevamiento preliminar en reconstrucción (17/11/2026).  
**Criterio:** ninguna funcionalidad detallada del borrador anterior tiene aprobación expresa de la dueña. Esta documentación no autoriza implementar flujos comerciales sin nueva validación.

## Contexto conocido y evidencia

- El Refugio es una sanguchería. Santiago compartió una imagen de la carta del negocio como referencia del menú vigente que conoce; no se verificaron precios ni disponibilidad real de cada producto.
- Según Santiago, la dueña atiende sola y expresó interés en reducir la necesidad de una persona dedicada a tomar pedidos.
- Santiago relató que ella mencionó una **tablet en el local** para que el cliente elija productos y se genere una **comanda**; falta validar cómo llega a cocina, cómo se confirma y cómo se cobra.
- También relató interés en una **página web** para armar el pedido y continuar mediante un **mensaje de WhatsApp**; todavía no sabemos si es el flujo que ella quiere finalmente.
- Santiago mencionó que ella no quería pagos integrados ni cuentas de usuarios; su significado y alcance deben confirmarse directamente.
- La carta contiene sándwiches definidos. La idea de «armar un sándwich desde cero» fue mencionada, pero Santiago aclara que **no es una modalidad actualmente implementada en el negocio**.

## Carta recibida (referencia, no catálogo aprobado en sistema)

- **Panes:** focaccia (aceitunas, parmesano, tomates secos); ciabatta.
- **Sándwiches fríos:** Lácar, Lolog, Curruhué, Falkner, Tromen.
- **Sándwiches calientes:** Villarrica, Osorno, Lanín, Llaima.
- **Clásicos completos:** milanesa; lomo.
- **Al plato:** milanesa napolitana con papas.
- **Pizzetas:** muzzarella; mortadela y pistachos; jamón crudo y pesto de tomates secos.
- **Papas:** simples; bravas (picante y alioli).
- **Bebidas:** gaseosas 500 ml; gaseosas 1,5 L; cerveza lata.

La imagen recibida muestra espacios punteados donde irían precios, **sin valores legibles publicados**. No asignar precios, variantes, ingredientes opcionales ni stock por inferencia. Validar la transcripción y la carta actual con la dueña antes de cargar el catálogo.

## Necesidades y posibles funcionalidades (estado: propuesta por validar)

| ID | Tema | Hipótesis / necesidad preliminar | Estado |
|---|---|---|---|
| P-001 | Atención en local | El cliente usa una tablet para seleccionar productos de la carta y finalizar una solicitud. | Propuesta, sin flujo aprobado |
| P-002 | Comanda | Tras la selección se emite o muestra una comanda para preparación. Medio, destinatario y momento sin definir. | Propuesta |
| P-003 | Web | El cliente puede explorar la carta y preparar un pedido desde su dispositivo. | Propuesta |
| P-004 | WhatsApp | Desde la web se prepara un mensaje de pedido a WhatsApp; la dueña decidirá si el pedido requiere confirmación manual. | Propuesta |
| P-005 | Personalización | Posibilidad futura o inicial de armar sándwiches personalizados; todavía no es una modalidad operativa actual. | Idea por explorar |
| P-006 | Cobro y acceso | Posible ausencia de pagos online y registro de usuarios; no implica ausencia de cobro presencial ni de almacenamiento interno. | Por confirmar |

## Elementos del borrador anterior: no aprobados

Se conservan para contrastar con la dueña, **no como requisitos**:

- Armado desde cero con precio igual a suma de ingredientes.
- Personalización de predefinidos cobrando solo extras.
- Cada extra con precio individual.
- Tamaños seleccionables.
- Mínimos y máximos por etapa de elección.
- Habilitar WhatsApp solo durante horario abierto.
- Dejar combos fuera de la primera versión.

Ninguna de estas condiciones debe darse por aceptada o implementarse por el solo hecho de figurar en el borrador histórico.

## Preguntas prioritarias para la dueña

1. **Primera conversación:** cuando un cliente termina de elegir en la tablet, ¿qué querés que pase: ticket impreso, pantalla para cocina, aviso para atenderlo u otra cosa?
2. ¿Cómo se cobra el pedido dentro del local? ¿Antes o después de la preparación? ¿Quién confirma el pago?
3. ¿La tablet debe permitir los sándwiches de la carta tal cual están, cambios simples, o armar desde cero?
4. Para pedidos desde afuera, ¿querés solo generar el mensaje de WhatsApp o también registrar/confirmar el pedido dentro del sistema?
5. ¿Qué información mínima necesita la comanda y cómo distinguen pedidos en el local?
6. ¿Se permite pedir cuando el local está cerrado? ¿Quién mantiene actualizados menú, precios y disponibilidad?
7. ¿Qué quiere decir exactamente «sin pagos» y «sin usuarios»?
8. ¿Cuáles son las funcionalidades indispensables para abrir la primera versión?

No convertir esta lista en un cuestionario de una sola vez; priorizar una pregunta por conversación según las respuestas.

## Aprobación y criterios de aceptación

No hay aún requisitos funcionales detallados aprobados por la dueña ni criterios de aceptación finales. Al validar cada flujo, documentar actor, pasos, resultado, excepciones y condiciones comprobables; actualizar reglas, decisiones y roadmap en el mismo PR.
