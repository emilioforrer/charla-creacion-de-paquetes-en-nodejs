## Como crear un paquete

Ejecutamos el siguiente comando

```js
mkdir hjs-demo
cd hjs-demo
yarn init
```

Esto nos creara una carpeta con el archivo `package.json`

El cual posee muchas propiedas, como:

* **name**: Este es el nombre de nuestro paquete \(cuando es una organizacion lleva el prefijo de la organizacion precedido por una @ y separado por `/`\)

* **version**: Aqui se describe la versión del paquete, que debe sergui el [semver](http://semver.org/)

* **main**:  Indica el archivo de entra hacia nuestra app

* **dependencies**: Listado de pendencias del paquete

* **devDependencies**: Listado dependencias para el  desarrollo del paquete

* Podemos ver el listado completo [aquí](https://docs.npmjs.com/files/package.json)



