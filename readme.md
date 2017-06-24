#Practica 1. 

##¿Qué comando utilizaste en el paso 11? ¿Por qué?
Para perder los cambios en el working copy es necesario usar *git reset --hard HEAD~1* (de esta forma se modifica el working copy y se vacia el staging area)

##¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Primeramente necesitas utilizar el comando *git reflog* para listar todas las acciones realizadas (reflog lista los commit)
A continuacion se realizara un *git reset --hard* **identificador corto del puntero donde quieres ir**

##El merge del paso 13, ¿Causó algún conﬂicto? ¿Por qué?
No, pero realmnente no pasa nada, ya que según el merge la rama style ya esta update
 El merge del paso 19, ¿Causó algún conﬂicto? ¿Por qué?
Sim causo conflicto
Auto-merging git-nuestro.md
CONFLICT (content): Merge conflict in git-nuestro.md
Automatic merge failed; fix conflicts and then commit the result.

Es debido a que cada rama tiene un git-nuesrto con distinto contenido

##El merge del paso 21, ¿Causó algún conﬂicto? ¿Por qué?
No hay ningun conflicto, se trata de merge fast forward

##¿Qué comando o comandos utilizaste en el paso 25?
git log --graph --decorate --pretty=oneline

##El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si, ya que unicamente seria avanzar el puntero

##¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1 el cual no borra el working copy (si quieres borrar el working copy usar el modificador --hard)

##¿Qué comando o comandos utilizaste en el paso 28?
git checkout -- git-nuestro.md

##¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title

##¿Qué comando o comandos utilizaste en el paso 30?
git reflog para buscar el merge
git checkout **identificador del merge**
git branch title + git checkout title o git checkout -b title

##¿Qué comando o comandos usaste en el paso 32?
git reflog para sacar el identificador corto del commit
git checkout **identificador del commit**
git checkout -b inicial
git checkout master
git merge inicial
git branch -D inicial

##¿Qué comando o comandos usaste en el punto 33?
git reflog para localizar el identificador corto del titulo
git checkout **identificador del commit**
git checkout -b final
git checkout master
git merge final
git branch -D final
