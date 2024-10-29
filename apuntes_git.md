# Apuntes git.

## Teoria general

Tenemos tres areas de trabajo:

1. _Working Area:_ Área de trabajo: archivos del proyecto en el que estamos trabajando.
2. _Staging Area:_ Área de puesta en escena: zona temporal donde los archivos modificados que necesitamos agregar a nuestro control de versiones están esperando ser agregadas al repositorio.
3. _Repository:_ Repositorio: archivos y registros en el repositorio

Acciones:

1. _Staging:_ pasar los archivos del área de trabajo al área de _staging_.
2. _Commit:_ Desde el área de puesta en escena hasta el repositorio haremos _commit_.

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

_Falta contrastar información, no recuerdo su fuente_
En windows substituir “input” por “true” en el siguiente comando
`git config --global core.autocrlf input `

## Inicio rápido de un nuevo repositorio.


### Consideraciones:
- Git linea comandos instalado. 

- GitHub CLI instalado. [url](https://cli.github.com/).
- Tener en cuenta que la rama principal es _main_.

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
2. La segunda opción es hacer un _Fork_ del repositorio, esto creará una copia en nuestra cuenta de github, allí podremos hacer los cambios que queramos y luego se crea un Pull Request desde tu fork al repositorio original. La que se usa si no conocemos el propietario del repositorio o no hay una relación de confianza.

## Documentando mi repo

1. Creo una rama nueva develop y me cambio a ella en un paso:

```
git checkout -b develop
```

Aunque me gusta hacer lo mismo con dos comandos por separado para aprender y de paso lo subo al remoto:

```
git branch develop
git checkout develop
git push -u origin develop
```

2. A ver cuantas ramas tengo en mi repo?

```
git branch --list
git branch -l
```

3. A ver que commits se han creado? Ei , pero de forma simplificada que si no saca demasiadas lineas y me pierdo.

    ```
    git log --pretty=oneline
    ```
4. Creo rama apuntes-git_gabriel, que es en lo que me voy a centrar estos dias
    ```
    git checkout -b apuntes-git_gabriel
    ```

5. Ah y que quede constancia en github !
```
git push
```

