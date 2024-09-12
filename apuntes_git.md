# Apuntes git.

## Teoria general

Tenemos tres areas de trabajo:

1. *Working Area:* Área de trabajo: archivos del proyecto en el que estamos trabajando.
2. *Staging Area:* Área de puesta en escena: zona temporal donde los archivos modificados que necesitamos agregar a nuestro control de versiones están esperando ser agregadas al repositorio.
3. *Repository:* Repositorio: archivos y registros en el repositorio

Acciones:
1. *Staging:*  pasar los archivos del área de trabajo al área de *staging*.
2. *Commit:* Desde el área de puesta en escena hasta el repositorio haremos *commit*.

## Configuración bàsica GIT

```
git config --global user.name minombre
git config --global user.email email@dominio.com
```

Configuramos git para que la rama principal sea siempre "main". [Fuente](https://help.dreamhost.com/hc/es/articles/4466702078740-Configurar-git-para-usar-main-como-rama-principal)
```
git config --global init.defaultBranch main
```

Para editar la configuración en achivo de texto:
```
git config --global -e
```

*Falta contrastar información, no recuerdo su fuente* 
En windows substituir “input” por “true” en el siguiente comando
`
git config --global core.autocrlf input 
`

## Inicio rápido de un nuevo repositorio.

### Consideraciones:
- Git linea comandos instalado. 
- GitHub CLI instalado. [url](https://cli.github.com/).
- Tener en cuenta que la rama principal es *main*. 

```
cd ruta/al/directorio/new_repo
git init
```
Añadir ficheros del proyecto, asegurarse que el archivo  *__.gitignore__* es correcto.
```
git add . #atentos a archivos que deberian esta en .gitignore
git commit -m "Primer commit"
gh auth login
gh repo create nombre-del-repo --source=. --remote=origin --description "Descripcion del repo"
git push -u origin main

```
Solo nos queda verificar que los cambios se han realizado en la url de Github.

## Autenticarse con github CLI 
```
gh auth login
```

## Colaboración mediate Github

Parece que hay dos maneras principales de colaborar en github sobre un repositorio dado:

1. La primera opción es que el propietario del repositorio nos añada como colaborador, en los ajustes debe haber menú de colaboradores.
2. La segunda opción es hacer un *Fork* del repositorio, esto creará una copia en nuestra cuenta de github, allí podremos hacer los cambios que queramos y luego se crea un Pull Request desde tu fork al repositorio original. La que se usa si no conocemos el propietario del repositorio o no hay una relación de confianza.

## Documentando mi repo

1. Creo una rama nueva develop y me cambio a ella en un paso:
```
git checkout -b develop
```
Aunque me gusta hacer lo mismo con dos comandos por separado:
```
git branch develop
git checkout develop
```
2. A ver cuantas ramas tengo en mi repo?
``` 
git branch --list
git branch -l
```
3. Hacer cambios ... añadirlos y  *comitear*
    ```
    git status
    git add .
    git commit -m "Añadidos los cambios X"
    ```
4. Subir rama al repositorio remoto
    ```
    git push origin nueva-rama
    ```

5. 

## Liandola con github
No se me ha ocurrido retocar este fichero en local de la rama apuntes-md sin antes hacer un Pull de la rama ... tengo la sensación es que estoy liandola :-)

```
git push origin apuntes-md
git checkout main
   Your branch is behind 'origin/main' by 5 commits, and can be fast-forwarded.
   (use "git pull" to update your local branch)
git pull
   Updating 8eefb4b..a8d8c3c
   Fast-forward
    apuntes_git.md | 71    ++++++++++++++++++---------
    1 file changed, 45 insertions(+), 26 deletions(-)
```
No me dejaba guardar los cambios porque no coincidian los ficheros , he de cambiarme a `apuntes-md` otra vez.

Seguiremos con merge :-P