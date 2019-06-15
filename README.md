# Práctica del curso de git, gitHub y Sourcetree

Este repositorio, tiene las respuestas al *ejercicio1* la práctica del *curso de Git, Github y Sourcetree*.

## Ejercicio 1

1. ### ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Usé el comando ```$git checkout HEAD~1``` esto, porque es una forma mas elegante de usar ```$git reset --hard HEAD~1```, además que al hacer checkout, ya me modifica el staging area.
Con checkout me da un `detached HEAD`.
Con reset se mueve solo se mueve al commit anterior.


2. ### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Use el comando ```$git reflog``` para ver el id del commit, luego use ```$git checkout 1ad765f``` para moverme al commit que se deshizo.
También se probó el comando ```$git reset a438181``` esto nos mantiene el working copy.


3. ### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

Este no causó ningún conflicto, debido a que las 2 ramas estaban en el mismo `commit`.


4. ### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si causó un conflicto, esto debido a que se han modificado las mismas líneas del archivo `git-nuestro.md` en ambas ramas.

5. ### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

Este merge no causó conflictos, porque el archivo `git-nuestro.md` en la rama master no tenia ningún cambio, y lo que sucedió fue que los cambios o commits del archivo `git-nuestro.md` en la `rama styled`, fueron absorbidos y se trajeron esos cambios para que se apliquen en el archivo de la `rama master`.


6. ### ¿Qué comando o comandos utilizaste en el paso 25?

Usé el comando ```$git log --grapht --decorate``` ya que no tengo alias creados.


7. ### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

El `merge` del paso 26 sí podría ser fast-forward,porque hay un solo commit al que subir o alcanzar por parte de la `rama master` y que no tiene, simplemente el puntero `master` se ubica en el commit en el que se agrega un título en el archivo `git-nuestro` de la `rama title`.


8. ### ¿Qué comando o comandos utilizaste en el paso 27?

En el paso 27 se uso el comando ```$git reset HEAD~1```


9. ### ¿Qué comando o comandos utilizaste en el paso 28?

En este paso usea 2 comandos:
- Primero ```$ git diff HEAD``` para ver las  diferencias entre el working copy con el repo.

- Luego para descartar los cambios o dejar el archivo del working copy como esta en el repositorio usé:
```$ git checkout -- git-nuestro.md``` 
- Luego podemos ver con un ```$ git status``` que no hay ningún cambio en el archivo, así como dentro del archivo el título está como al inicio.

10. ### ¿Qué comando o comandos utilizaste en el paso 29?

Usé el comando  ```$git branch -D title```


11. ### ¿Qué comando o comandos utilizaste en el paso 30?

En el paso 30 usé lo siguientes comandos:
- ```$git reflog```
- ```$git reset --hard 0effff6``` usando el id del commit al que quiero moverme, podría usar también `git reset HEAD` para hacerlo.

12. ### ¿Qué comando o comandos usaste en el paso 32?

En el paso 32 usé los siguientes comandos:
- ```$git log```
- ```$git checkout 59052a19ab2010231af5598457e717eb12f6870d``` el hash del commit.

13. ### ¿Qué comando o comandos usaste en el punto 33?

Usé los siguientes comandos:
- ```$git reflog```
- ```$git reset --hard 0effff6``` usando la avrebiación del sha del commit.