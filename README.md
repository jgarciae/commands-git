# Git Commands

## 1. git init
```bash
echo "# commands-git" ]] README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:usuario/commands-git.git
git push -u origin main
```

## 2. Proyecto existente
```bash
git init
git remote add origin git@github.com:usuario/commands-git.git
git branch -M main
git push -u origin main
```

## 3. Configuracion

- Establece el nombre usuario en las transacciones de commit

```bash
$ git config --global user.name "[name]"
```

- Establece el e-mail en las transacciones de commit

```bash
$ git config --global user.email "[email]"
```

## 3. Ejecutar cambios

- Muestra el estado del repositorio, incluyendo archivos modificados, sin trackear, y cambios listos para commit.
```bash
$ git status
```

- Muestra las diferencias entre los archivos modificados que no han sido añadidos al área de preparación.
```bash
$ git diff
```

- Muestra las diferencias del archivo entre el área de espera y la última versión del archivo.
```bash
$ git diff --staged
```

- Añade el archivo especificado al área de preparación para ser incluido en el próximo commit.
```bash
$ git add [file]
```

- Remueve el archivo del área de preparación, pero mantiene los cambios en el directorio de trabajo.
```bash
$ git reset [file]
```

- Confirma los cambios añadidos al área de preparación con un mensaje de commit específico proporcionado entre comillas.

```bash
$ git reset [file]
```

## 4. Cambios grupales

- Enumera todas las ramas en el repositorio actual.

```bash
$ git branch
```

- Crear nueva rama.

```bash
$ git branch [branch-name] / git checkout -b [branch-name] 
```

- Cambiar de rama.

```bash
$ git checkout [branch-name] 
```

- Eliminar rama

```bash
$ git branch -d [branch-name]
```

## 5. Manejo de archivos

- Borra el archivo del directorio y lo pone en espera del archivo borrado.

```bash
$ git rm [file]
```

- Borra el archivo de controlador de versiones pero no lo elimina a nivel local.

```bash
$ git rm --cached [file]
```

- Cambia el nombre del archivo y lo prepara para el commit
```bash
$ git mv [file-original] [file-renamed]
```

## 6. Historial

- Enumera el historial de la versión para la rama actual.
```bash
$ git log
```

- Enumera el historial de versión para el archivo, incluidos los cambios de nombre.
```bash
$ git log --follow [file]
```

- Muestra las diferencias entre dos ramas.
```bash
$ git diff [first-branch]...[second-branch]
```

- Muestra información detallada sobre un commit específico.
```bash
$ git show [commit]
```

## 7. Sincronizar Cambios

- Descarga todo el historial del marcador del repositorio
```bash
$ git fetch
```

- Combina la rama del marcador con la rama local actual
```bash
$ git merge [branch]
```

- Carga todos los commits de la rama local al repositorio en el servidor
```bash
$ git push [branch]
```

- Descarga el historial del marcador
```bash
$ git pull
```
