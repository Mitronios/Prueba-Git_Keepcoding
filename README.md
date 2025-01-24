# Git desde la terminal

## Preguntas sobre un flujo de trabajo de Git

1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?

   > Utilicé el comando: `git reset --hard~1`.

2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

   > Utilicé el comando: `git reflog` para obtener el identificador del último commit, luego `git reset --hard a9b2745` para moverme a ese commit.

3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

   > Cuando intentaba realizar el merge, me daba el mensaje de "Already up to date".
   >
   > Intente hacer el merge fast forward y no fast forward y tampoco funcionó.
   >
   > Averiguando encontré que las ramas locales estaban sincronizadas pero que las remotas podían diverger y la manera de solucionarlo fue hacer un commit en cada rama y luego hacer el merge para sincronizar las ramas locales y remotas.
   >
   > Fue un merge no fast forward.

4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

   > Causó un conflicto que me pedía comparar los cambios y unificarlos, porque modificaba un mismo archivo sobreescribiendo las líneas que estaban en 'styled', se resolvió quedándonos con el contenido de la rama 'styled' y descartando los cambios que llegaban de 'htmlify'.

5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
6. ¿Qué comando o comandos utilizaste en el paso 25?
7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
8. ¿Qué comando o comandos utilizaste en el paso 27?
9. ¿Qué comando o comandos utilizaste en el paso 28?
10. ¿Qué comando o comandos utilizaste en el paso 29?
11. ¿Qué comando o comandos utilizaste en el paso 30?
12. ¿Qué comando o comandos usaste en el paso 32?
13. ¿Qué comando o comandos usaste en el punto 33?
