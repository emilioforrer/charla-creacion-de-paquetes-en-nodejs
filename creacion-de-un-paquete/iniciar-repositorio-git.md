## Iniciar repositorio GIT

Inicializamos el repo con el siguiente comando:

```
git init
```

Para un mejor control del versionamiento de nuetro paquere vamos a utilizar [git-flow](https://danielkummer.github.io/git-flow-cheatsheet/). Inicializamos git flow en nuestro proyecto, con el siguiente comando.

```
git-flow init
```

Creamos nuestro archivo .gitignore \(`nano .gitignore`\) y agregamos:

```
node_modules/
bower_components/
```

Creamos nuestro archivo .npmignore \(`nano .`npmignore\) y agregamos:

```
src/
test/
bower_components/
```

Como buena práctica es bueno crear los siguientes archivos:

```
CHANGELOG.md
README.md
```


