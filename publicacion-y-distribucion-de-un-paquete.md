## Publicación y distribución  de un paquete

Ahora hacemos commit de nuestros cambios

```
git add -A; git commit -am "new release"
```

Finalizamos el release

```
git flow release finish v0.1.0
```

Hacemos push al `branch` **develop**

```
git push origin develop
```

Nos cambiamos al `branch` master y luego hacemos push junto con todos los tags creados a partir del release. Esto nos creará el tag en el repositorio remoto.

```
git checkout master
git push --tags origin master
```

Después de esto nos registramos en la página de [npm](https://www.npmjs.com/signup).

Una vez que ya hemos creado el usuario iniciamos sesión en la terminal, con el siguiente comando.

```
yarn login
```

E introducimos nuestro nombre de usuario y correo electrónico.

Luego de esto, hoy si ya podemos finalmente publicar nuestro paquete y que este disponible en los registros de npm, con el siguiente comando.

```
yarn publish
```

Y si tu usuario es organización y quieres que tu paquete este público, hay que correr el siguiente comando

```
yarn publish --access public
```

**Nota**: Cuando tu usuario de npm es una **organización**, el nombre del paquete en tu `package.json` debe ser `@nombre-de-la-organizacion/nombre-del-paquete`. Ejemplo:  `@horchatajs/hjs-multiselect`

