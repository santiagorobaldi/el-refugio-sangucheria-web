# Instrucciones para agentes

## Fuente de verdad
- Este repositorio es la fuente compartida de requisitos, reglas de negocio y decisiones de El Refugio Sanguchería.
- Antes de trabajar, leer `docs/requirements.md`, `docs/business-rules.md`, `docs/decisions/README.md`, `docs/roadmap.md` y `docs/analyst-workflow.md`.
- **Revisión del 17/11/2026:** el relevamiento original contenía decisiones sugeridas por Santiago que no habían sido consultadas ni aprobadas expresamente por la dueña. Esas decisiones ya no son requisitos confirmados.
- Distinguir **hechos o materiales aportados**, **propuestas**, **aprobaciones explícitas de la dueña** e **implementación verificada**. Que Santiago confirme haber oído una idea no equivale a aprobar su comportamiento detallado.
- No deducir precios, horarios, límites, reglas de cobro o funcionalidades obligatorias a partir de la carta, de una conversación informal o de un prototipo.

## Trabajo con la dueña
- Conversar en español argentino, con preguntas breves y simples, una cuestión decisiva a la vez.
- Presentar la documentación como «documentación de Santiago»; no es necesario hablarle de GitHub.
- Comenzar por cómo quiere que funcione la atención en el local y qué sucede tras completar un pedido en la tablet.
- Confirmar por separado el funcionamiento del local y el canal web/WhatsApp; no asumir que comparten confirmación, pago o comanda.
- Las sugerencias de Santiago y del analista no cuentan como decisiones aprobadas por la dueña.

## Cambios e implementación
- Registrar una aprobación solo cuando haya confirmación expresa de la dueña, con criterios comprobables y fecha si se conoce.
- Mantener el roadmap condicionado a ese relevamiento. No desarrollar las ideas no validadas como si fueran alcance contratado.
- Codex implementa y prueba según requisitos aprobados; los cambios de documentación y código van en rama y PR revisable, salvo indicación expresa contraria.
- No fusionar automáticamente los PR ni afirmar que algo está implementado si no se verificó.

## Antes de terminar
- Indicar qué se modificó, qué se aprobó efectivamente y qué sigue abierto.
- Comprobar que ninguna propuesta se presente como regla de negocio confirmada.
