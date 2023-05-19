# Git Cheatsheet

## Configuración básica
- `git config --global user.name <nombre>`: Establece el nombre de usuario.
- `git config --global user.email <email>`: Establece la dirección de correo electrónico.
- `git config --global core.editor <editor>`: Configura el editor de texto predeterminado para los mensajes de commit.

## Crear y clonar repositorios
- `git init`: Inicializa un nuevo repositorio local.
- `git clone <url>`: Clona un repositorio remoto existente.

## Realizar cambios
- `git status`: Muestra el estado actual del repositorio.
- `git add <archivo>`: Agrega un archivo específico al área de preparación.
- `git add .`: Agrega todos los archivos modificados al área de preparación.
- `git commit -m "<mensaje>"`: Crea un nuevo commit con los archivos en el área de preparación.
- `git diff`: Muestra las diferencias entre los archivos modificados y el último commit.

## Ramas (Branches)
- `git branch`: Muestra todas las ramas locales.
- `git branch <nombre_rama>`: Crea una nueva rama.
- `git checkout <nombre_rama>`: Cambia a la rama especificada.
- `git merge <nombre_rama>`: Fusiona la rama especificada con la rama actual.
- `git branch -d <nombre_rama>`: Elimina la rama especificada.

## Sincronización remota
- `git remote add origin <url>`: Agrega un repositorio remoto con el nombre "origin".
- `git push -u origin <rama>`: Sube la rama actual al repositorio remoto.
- `git pull origin <rama>`: Descarga los cambios más recientes desde el repositorio remoto.
- `git fetch`: Obtiene los cambios remotos sin fusionarlos automáticamente.

## Historial y deshacer cambios
- `git log`: Muestra el historial de commits.
- `git log --oneline`: Muestra el historial de commits en una sola línea.
- `git reset <commit>`: Deshace los cambios realizados después del commit especificado.
- `git revert <commit>`: Revierte el commit especificado creando un nuevo commit.

## Consejos útiles
- Utiliza `.gitignore` para especificar los archivos y directorios que no deben ser rastreados por Git.
- Realiza commits atómicos y descriptivos para mantener un historial claro y comprensible.
- Utiliza ramas para desarrollar nuevas características o solucionar problemas sin afectar la rama principal.
- Antes de fusionar ramas, utiliza `git merge --no-ff` para preservar el historial de desarrollo.
- Utiliza `git stash` para guardar temporalmente los cambios no terminados y pasar a otra tarea.

