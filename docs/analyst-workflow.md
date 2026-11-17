# Flujo de trabajo: analista de requisitos y Codex

## Fuente compartida

El contenido versionado en GitHub es la referencia compartida para ambos roles:

- `AGENTS.md`: instrucciones para agentes que trabajan en el repositorio.
- `docs/requirements.md`: requisitos confirmados y preguntas abiertas.
- `docs/business-rules.md`: reglas de negocio verificables.
- `docs/decisions/README.md`: decisiones aprobadas.
- `docs/roadmap.md`: alcance y secuencia conocida.

Una conversación de ChatGPT o Codex por sí sola no cambia estos archivos.

## Trabajo del analista en ChatGPT

1. Consultar la versión más reciente de estos documentos en GitHub antes de responder sobre requisitos.
2. Usar las preguntas abiertas para entrevistar al cliente. Marcar claramente qué respuesta fue confirmada y qué sigue siendo una propuesta.
3. Preparar cambios concretos para los archivos afectados, manteniendo las preguntas no resueltas y sin inventar decisiones.
4. Proponer el cambio mediante una rama y pull request si la cuenta/conexión lo permite. Si no, entregar al cliente el texto o diff listo para incorporar.
5. Compartir con Codex el enlace al PR o los archivos actualizados para que implemente sobre la versión revisada.

## Trabajo de Codex

1. Leer la documentación más reciente de la rama objetivo antes de cambiar producto o código.
2. Implementar únicamente lo respaldado por requisitos aprobados. Ante una ambigüedad relevante, dejar una pregunta documentada o pedir aclaración; no elegir una política de negocio en silencio.
3. Cuando el usuario confirme requisitos nuevos, actualizar los documentos junto con el cambio correspondiente y presentarlos en un PR para revisión.
4. En la respuesta final, indicar el commit/PR usado como base, documentos cambiados y preguntas que siguen abiertas.

## Mantener ambos roles sincronizados

- GitHub conserva el historial y los cambios revisables; ambos roles deben volver a leer la versión más reciente antes de trabajar.
- Preferir PR para cambios de requisitos y código. Revisar y fusionar el PR es la acción que hace que su contenido pase a la rama compartida acordada.
- Si uno de los roles trabaja con una copia local o contexto anterior, puede quedar desactualizado. Indicar explícitamente la rama y el PR/commit de referencia al pasar trabajo.
- No asumir sincronización automática entre conversaciones, memoria, checkout local y GitHub. El acceso depende de las herramientas/conexiones disponibles en cada sesión.

## Handoff manual y límites

El cliente debe pasar el enlace del PR, commit o archivos entre conversaciones cuando los roles no comparten el mismo contexto. ChatGPT no recibe automáticamente los cambios locales de Codex y Codex no recibe automáticamente el historial completo de otra conversación. Un conector de GitHub puede permitir leer o proponer cambios directamente, pero no garantiza que cada conversación esté conectada, autorizada o consultando la última versión.

Para evitar divergencias, incluir en cada handoff: objetivo, enlace de PR/commit, estado de aprobación y preguntas pendientes. No copiar una regla de memoria conversacional como si ya estuviera aprobada en el repositorio.
