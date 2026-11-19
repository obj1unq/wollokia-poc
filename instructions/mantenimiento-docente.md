# Mantenimiento docente del proyecto

## Activación y alcance

Aplicar estas instrucciones en el rol docente, según [AGENTS.md](../AGENTS.md), antes de responder o actuar. El objetivo es mantener las instrucciones, los guardrails y la documentación del proyecto según los pedidos docentes.

Leer los archivos afectados antes de revisarlos o editarlos. Leer íntegramente [asistencia-estudiante.md](asistencia-estudiante.md) antes de revisar o editar sus reglas: es material de configuración, no el protocolo de esta conversación.

No aplicar a los turnos docentes los niveles de ayuda, la puerta de diseño, el registro en `interacciones-ia.md` ni los commits automáticos del protocolo estudiantil. No borrar ni reescribir el registro existente. El docente no ejecuta operaciones de Git: el usuario controla el repositorio.

## Cambios de guardrails

Para modificar las instrucciones o la documentación del proyecto:

1. Editar en el árbol de trabajo los archivos correspondientes: `AGENTS.md`, los archivos de `.opencode/agents/`, `opencode.json`, los archivos de `instructions/` u otros documentos de configuración.
2. No ejecutar ninguna operación de Git: ni `add`, `commit`, `push`, `checkout`, `switch`, `rebase`, `merge`, `stash`, ni consultas para decidir sobre ramas o historial. El usuario elige la rama de guardrails `poc/NN/main` y realiza todos los commits, rebases y pushes.
3. No agregar las interacciones de modo docente a `interacciones-ia.md`; el usuario decide cuándo y cómo versionar los cambios.
4. Dejar los cambios sin commitear, describirlos en la respuesta y avisar al usuario para que los revise y commitee. Si corresponde incorporarlos a la rama de resolución `poc/NN/resolution`, informarlo: el usuario decide si hace el rebase, sin que el docente modifique ramas ni historial.
5. Verificar que el registro no conserve turnos de modo docente y sugerir al usuario seleccionar el agente `estudiante` para continuar.

El rol docente no ejecuta Git ni autoriza por sí solo instalaciones, commits, pushes ni otras acciones externas; respetar las autorizaciones y restricciones comunes de `AGENTS.md`.
