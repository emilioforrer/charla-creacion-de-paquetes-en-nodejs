# Como crear, publicar y distribuir un paquete de Node js

###### Escrito por Emilio Forrer,  para la conferencia en HorcharaJS

---

## ¿Qué es un paquete y para nos sirve?

Un paquete es una forma encapsular y extraer de nuestro proyecto principal: librerias, componentes, funcionalidades, etc. Para que mediante un gestor de paquetes, las podamos instalar y reutilizar, en diferentes proyectos, siguiendo asi el principio DRY \(Do not repeat yourself\).

Lo cual no ofrece muchas ventajas como:

* Modularización.
* Instalación de subdependencias.
* Distribución mas fácil y efectiva, siguiendo el versionamiento de cada componentes, etc.

## ¿Qué es un gestor de paquetes?

Un gestor de paquetes es el que se encarga de distribuir, instalar, actualizar y controlar las dependiencias de los paquetes a través de un`descriptor.`

En la mayoria de lenguajes de programación modernos, existen gestores de paquetes y dependencias como:

* PHP: **Composer**
* Ruby: **Bundler**
* Nodejs: **npm** **y yarn **

Nota: si todavia ocupan **npm**, por favor comienzen a migrar a **yarn**. Yarn ofrece muchas más ventajas y ademas provee un archivo de bloqueo de versiones de las dependecias \(tipo: Gemfile.lock, composer.lock\) y ya no es necesario ocupar el comando **shrinkwrap** de npm el cual tenia ciertas dificultades.

## Descriptor

Es el archivo en el cual nosotros declaramos, las caracteristicas de nuestro poquete, como:

* El nombre
* La version
* Las dependencias, tando en ambiente de desarrollo como en ambiente  normal
* Archivos a incluir
* Información acerca del paquete, como:
  * Nombre del autor
  * Nombre de los contribuyentes
  * Dirección URL del paquete, etc
* Y muchas cosas más.





