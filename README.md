# Functions to work with github
```sh
…or create a new repository on the command line

echo "# gitcommands" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/edwinrepo/gitcommands.git
git push -u origin main

…or push an existing repository from the command line
git remote add origin https://github.com/edwinrepo/gitcommands.git
git branch -M main
git push -u origin main
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
```

## Comandos de git

Tomado de:
https://www.youtube.com/watch?v=AzfVDEBn9hw&t=243s

Se usa para iniciar la configuración del git
```sh
git init
```

Se crea una rama que se llama master, by default.

Para conocer el estado del repositorio
```sh
git status
```

Para agregar el archivo se le da
```sh
git add {new_file}
```

O se puede poner
```sh
git add .
```
Con el punto se adicionan todos los archivos

Para hacer los cambios se usa el comando 
```sh
git commit -m "Éste es mi comentario"
```

Para agregar el origin

```sh
git remote add origin https://github.com/edwinrepo/comandosGithub.git
```

Para quitar el origen

git remote remove origin

Luego para hacer el push

```sh
git push -u origin master
```
Para conocer todos los cambios se usa git log

Git clone es para obtener un nuevo repositorio


```sh
git clone {direccion_del_repositorio}
```

## Para recuperar archivos

### Para conocer los commit que se han realizado

git log --pretty=oneline

### Para devolverse a algun commit se usa el comando

git reset --soft 9d645d084d541c295a0e206c619594e3dc90b7ab # El número que está acá proviene del git log

### Para regresar es con

git revert 9d645d084d541c295a0e206c619594e3dc90b7ab

## Para crear una rama

Si se crea una nueva rama todos los archivos se crean como en una nueva sesión

git branch nueva_rama

### Para saber cuántas ramas hay
git branch -v

### Para cambiar de rama:
git checkout nueva_rama

### Para unir dos ramas
se cambia a la rama que se quiera hacer el merge
git checkout master
y luego se usa:
git merge nueva_rama

### Para borrar dos ramas
Se elimina una rama
git branch -D nueva_rama # Se borra local
git push origin --delete nueva_rama # se borra en github


