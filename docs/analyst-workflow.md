# Flujo de trabajo: analista de requisitos y Codex

## Referencia compartida

- `AGENTS.md`: instrucciones para agentes.
- `docs/requirements.md`: contexto, hipótesis y requisitos que se aprueben.
- `docs/business-rules.md`: reglas aprobadas y comprobables.
- `docs/decisions/README.md`: registro de decisiones y rectificaciones.
- `docs/roadmap.md`: secuencia condicionada a validación.

El contenido versionado en la rama principal es la referencia oficial una vez revisado y fusionado; un PR abierto aún es un cambio propuesto.

## Cómo hacer el relevamiento

1. Leer la documentación más reciente antes de entrevistar a la dueña.
2. Explicar en lenguaje sencillo que existe «documentación de Santiago», pero que los detalles no fueron dados por aprobados.
3. Preguntar **una cuestión relevante por vez**. Empezar por la experiencia de la tablet y el destino de la comanda, no por parámetros técnicos.
4. Registrar claramente el origen de cada dato: carta aportada, relato de Santiago, respuesta directa de la dueña o propuesta del analista.
5. Clasificar **Propuesta / Aprobada / Implementada** sin elevar testimonios indirectos a aprobaciones funcionales.
6. Para cada requisito aprobado, definir comportamiento observable, excepciones y criterios de aceptación.
7. Preparar un PR de documentación en una rama; no fusionarlo automáticamente.

## Cómo trabajar con Codex

1. Consultar la rama `main` y los archivos anteriores, además del PR de relevamiento si todavía está pendiente.
2. Implementar **solo** comportamientos aprobados. La aprobación de un PR documental corrige el estado de la documentación, pero no aprueba propuestas comerciales listadas en ella.
3. No asumir precios, horarios, flujo de cobro, impresión, almacenamiento o integración de WhatsApp.
4. Al recibir una decisión aprobada, actualizar documentos afectados y preparar tareas específicas; informar rama/commit y evidencia de pruebas.
5. Marcar «Implementada» únicamente después de desarrollar y verificar.

## Sincronización y transferencia

La conversación no modifica el repositorio automáticamente. Indicar a Codex el PR o commit de referencia, el estado de aprobación y las preguntas pendientes. No copiar el relevamiento anterior como si estuviera confirmado. La dueña no necesita conocer GitHub: se le puede presentar como «la documentación de Santiago».
