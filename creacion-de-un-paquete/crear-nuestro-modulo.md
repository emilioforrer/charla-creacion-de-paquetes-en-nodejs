## Crear nuestro módulo

Modificamos la propiedad `main` de nuestro `packaje.json` para que apunte al archivo compilado:

```
  "main": "dist/hjs-demo.js",
```

Creamos el archivo `src/hjs-demo.sass` y agregamos:

```
body
  background-color: red
```

Creamos el archivo `src/hjs-demo.js` y agregamos:

```
import css from "./hjs-demo.sass";

var HjsDemo = {

  word: "Hola Mundo!",

  say: function() {
    console.log(this.word);
  }
}


export default HjsDemo;
```



