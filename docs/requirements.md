# Requisitos del producto

**Estado:** borrador inicial basado únicamente en requisitos confirmados.  
**Fuente de verdad:** este archivo y las reglas de negocio vinculadas. Las preguntas sin respuesta quedan abiertas.

## Alcance confirmado

1. **Armar un sándwich desde cero.** El cliente puede seleccionar ingredientes y el total se calcula sumando los precios de esos ingredientes.
2. **Personalizar un sándwich predefinido.** Si el cliente modifica un sándwich predefinido, se cobra únicamente el precio de los extras agregados. No se vuelve a cobrar el precio base del sándwich por esa modificación.
3. **Extras con precio individual.** Cada extra tiene un precio propio.
4. **Tamaños seleccionables.** La experiencia permite elegir tamaños. Los tamaños disponibles y su efecto en el precio están pendientes de definición.
5. **Mínimos y máximos configurables por etapa.** Cada etapa de selección puede tener límites mínimo y máximo configurables. La unidad, obligatoriedad y comportamiento exacto están pendientes.
6. **Pedidos por WhatsApp sujetos al horario del local.** La opción de realizar/enviar un pedido por WhatsApp está disponible solo cuando el local está abierto.
7. **Combos postergados.** Los combos quedan fuera del alcance inicial y se consideran para una etapa futura; el alcance futuro no está definido.

## Preguntas abiertas para el analista de requisitos

Resolver con el cliente y actualizar los documentos mediante un cambio revisable. No completar estas respuestas por inferencia.

### Catálogo y precios

- ¿Cuál es la lista de ingredientes y sus precios? ¿Quién puede editarlos y con qué frecuencia?
- ¿Qué significa exactamente “extra”: ingrediente añadido, reemplazo, porción adicional u otra opción?
- En un sándwich predefinido, ¿quitar ingredientes o reemplazar uno por otro tiene algún cargo o crédito?
- ¿Se permite agregar varias unidades del mismo ingrediente? ¿Cómo se calcula en ese caso?
- ¿Los precios incluyen impuestos? ¿Qué moneda y formato de precio se muestran?
- ¿Cómo se aplican los tamaños al sándwich armado desde cero y al predefinido? ¿Modifican ingredientes, cantidades o precios?

### Etapas y selección

- ¿Cuáles son las etapas de selección y en qué orden aparecen?
- ¿Qué elemento se cuenta para los mínimos y máximos de cada etapa?
- ¿Puede una etapa tener mínimo cero? ¿Qué ocurre si no se alcanza el mínimo?
- ¿Hay etapas o selecciones que dependan del tamaño, del tipo de sándwich o de otra elección?
- ¿Los límites se configuran por producto, etapa, tamaño o de manera global?

### Pedido y horario

- ¿Qué zona horaria y qué días/horas definen que el local está abierto?
- ¿Cómo se tratan feriados, cierres excepcionales y horarios que cruzan medianoche?
- ¿Qué debe ver el usuario cuando el local está cerrado? ¿Puede guardar o preparar un pedido para después?
- ¿“Solo cuando está abierto” se refiere a mostrar el botón, abrir WhatsApp o permitir completar el envío?
- ¿Qué número de WhatsApp se usa y qué datos/texto deben incluirse en el mensaje?
- ¿El pedido se considera confirmado al abrir WhatsApp, al enviarse el mensaje o tras otra confirmación?

### Alcance y operación

- ¿Qué otras páginas o funciones componen la primera versión?
- ¿Quién administra catálogo, precios, tamaños, límites y horarios, y desde qué herramienta?
- ¿Cómo se priorizarán y definirán los combos cuando se retomen?
- ¿Qué criterios de aceptación y escenarios de error debe cumplir cada flujo?

## Criterio de actualización

Al recibir una respuesta confirmada, convertirla en requisito verificable, reflejar la regla correspondiente en `business-rules.md`, actualizar una decisión en `decisions/README.md` cuando implique una elección aprobada y anotar el cambio en el roadmap si afecta el alcance o secuencia. Mantener aquí las preguntas que sigan sin respuesta.
