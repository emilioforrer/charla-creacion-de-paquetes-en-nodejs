## Iniciar repositorio GIT

Inicializamos el repo con el siguiente comando:

```
git init
```

Para un mejor control del versionamiento de nuetro paquere vamos a utilizar [git-flow](https://danielkummer.github.io/git-flow-cheatsheet/). Inicializamos git flow en nuestro proyecto, con el siguiente comando.

```
git flow init
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
changelog.md
readme.md
```

Ahora hacemos commit de nuestros cambios

```
git add -A; git commit -am "Initial commit"
```

Y comenzamos  a crear nuestro primer release con `git-flow` el  cual será la versión 0.1.0.

```
git flow release start v0.1.0
```

Y el primer paso antes de crear nuestro módulo será, cambiar la versión en el `package.json` para que haga match con nuestro release.



```
  "version": "0.1.0",
```



