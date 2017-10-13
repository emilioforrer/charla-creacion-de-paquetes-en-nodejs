## Compilar nuestro paquete

Para compilar nuestro paquete corremos el comando `gulp`.



Y si queremos probar nuestro paquete, podemos crear un archivo `test.js`, agregarle  



```
HjsDemo = require("./dist/hjs-demo.js");

console.log(HjsDemo.say());

```



y ejecutarlos con `node test.js`



