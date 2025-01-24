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

   > Causó un conflicto que me pedía comparar los cambios y unificarlos, esto pasó porque modificaba un mismo archivo sobreescribiendo las líneas que estaban en 'styled', es decir lás líneas modificadas contenían un texto diferente.
   >
   > Se resolvió quedándonos con el contenido de la rama 'styled' y descartando los cambios que llegaban de 'htmlify'.

5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

   > No causó ningún conflicto porque los archivos no se modificaron en las mismas líneas es decir en una misma línea no existían diferencias entre ambos archivos.
   >
   > Fue un merge fast forward.

6. ¿Qué comando o comandos utilizaste en el paso 25?

   > Se utilizó el comando: `git log --graph --decorate --pretty=oneline`.
   >
   > También se puede simplificar configurando el comando de la siguiente manera:
   >
   > `git config alias.graph "log --graph --decorate --pretty=oneline`
   >
   > De esta forma bastaría con ejecutar git graph.

7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

   > Podría ser fast forward debido a que la rama title es hija directa de la rama main y puede ser absorbida.

8. ¿Qué comando o comandos utilizaste en el paso 27?
   > El comando para deshacer el merge y mantener el working copy fue:
   >
   > `git reset HEAD~1`
9. ¿Qué comando o comandos utilizaste en el paso 28?

   > Utilicé el comando `git reset --hard HEAD` para descartar los cambios del paso 28.

10. ¿Qué comando o comandos utilizaste en el paso 29?

    > El comando que utilicé fue: `git branch -D title`

11. ¿Qué comando o comandos utilizaste en el paso 30?

    > Utilicé el comando: `git reflog` para encontrar el identificador del merge y luego `git checkout cc61716` para rehacer el merge.

12. ¿Qué comando o comandos usaste en el paso 32?
    > Utilicé
13. ¿Qué comando o comandos usaste en el punto 33?
