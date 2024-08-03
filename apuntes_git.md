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
Consideraciones:
- Git linea comandos instalado. 
- GitHub CLI instalado. [url](https://cli.github.com/).
- Tener en cuenta que la rama principal es *main*. 

```
cd ruta/al/directorio/new_repo
git init
git add . #añade todos los archivos existentes
git commit -m "Primer commit"
gh auth login
gh repo create nombre-del-repo --source=. --remote=origin --description "Descripcion del repo"
git push -u origin main

```
Solo nos queda verificar que los cambios se han realizado en la url de Github.
