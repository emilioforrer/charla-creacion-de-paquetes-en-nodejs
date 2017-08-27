# Como crear, publicar y distribuir un paquete de Node js

###### Escrito por Emilio Forrer,  para la conferencia en HorcharaJS

---

## Introducción

En la siguiente charla vamos a a dar a conocer un poco más acerca de Node js y su sistema de paquetes y dependencias

Nuestras metas a cumplir son:

* Crear, publicar y mantener paquetes para Node js.
* Buenas prácticas y recomendaciones a la hora de contruir tú propio paquete.
* Como distribuir tu paquete ya sea público o privado
  * local
  * github
  * gitlab
  * npm
  * Tu propio servidor privado

## ¿Qué es un paquete y para nos sirve?

Un paquete es una forma encapsular y extraer de nuestro proyecto principal: librerias, componentes, funcionalidades, etc. Para que mediante un gestor de paquetes, las podamos instalar y reutilizar, en diferentes proyectos, siguiendo asi el principio DRY \(Do not repeat yourself\).

Lo cual no ofrece muchas ventajas como:

* Modularización.
* Instalación de subdependencias.
* Distribución mas fácil y efectiva, siguiendo el versionamiento de cada componentes, etc.

## ¿Qué es un gestor de paquetes?

Un gestor de paquetes es el que se encarga de distribuir, instalar, actualizar y controlar las dependiencias de los paquetes a través de un `package descriptor` o `manifest`

En la mayoria de lenguajes de programación modernos, existen gestores de paquetes y dependencias como:

* PHP: [**Composer**](https://getcomposer.org/ "Composer")
* Ruby: [**Bundler**](http://bundler.io/)
* Nodejs: [**npm**](https://www.npmjs.com/) **y **[**yarn**](https://yarnpkg.com/en/)** **
* Javascript: [**bower**](https://bower.io/)
* Java: [**Maven**](https://search.maven.org/)

Nota: si todavia ocupan **npm**, por favor comienzen a migrar a **yarn**. Yarn ofrece muchas más ventajas y ademas provee un archivo de bloqueo de versiones de las dependecias \(tipo: Gemfile.lock, composer.lock\) y ya no es necesario ocupar el comando **shrinkwrap** de npm el cual tenia ciertas dificultades.

## Manifest / Package Descriptor 

Es el archivo en el cual nosotros declaramos, las características de nuestro paquete, como:

* El nombre
* La versión
* Las dependencias, tanto en ambiente de desarrollo como en ambiente  normal
* Archivos a incluir
* Información acerca del paquete, como:
  * Nombre del autor
  * Nombre de los contribuyentes
  * Dirección URL del paquete, etc
* Y muchas cosas más.

Ejemplos de package descriptors:

* Ruby: [**name\_of\_the\_gem.gemspec**](http://guides.rubygems.org/specification-reference/ "Gemspec")
* Node js: [**package.json**](https://docs.npmjs.com/files/package.json)
* Javascript: [**bower.json**](https://github.com/bower/spec/blob/master/json.md)
* Java:** **[**pom.xml**](https://maven.apache.org/pom.html "POM")
* PHP: [**composer.json**](https://getcomposer.org/doc/04-schema.md "Composer")



