# Functions to work with github
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

## Comandos de git

Se usa para iniciar la configuración del git
```git init```

Se crea una rama que se llama master, by default.

Para conocer el estado del repositorio
```git status```

Para agregar el archivo se le da
```git add {new_file}```
O se puede poner
```git add .```

Para hacer los cambios se usa el comando 
```git commit -m "Éste es mi comentario"```

Para agregar el origin

```git remote add origin https://github.com/edwinrepo/comandosGithub.git```
Luego para hacer el push

```git push -u origin master```
