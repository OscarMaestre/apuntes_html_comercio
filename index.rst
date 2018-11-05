.. Apuntes de HTML documentation master file, created by
   sphinx-quickstart on Mon Nov  5 09:41:25 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Apuntes de HTML's documentation!
===========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

Introducción
=======================

En este texto se da una introducción **muy básica** a la creación de páginas web. Para poder seguir estos apuntes basta con un ordenador que disponga de un editor de textos (puede bastar el "Bloc de Notas" de Windows). No es necesario disponer de conexión a Internet, ya que todos los ejemplos se almacenarán en el propio disco del equipo.

Se recomienda la creación de una carpeta (puede hacerse por ejemplo en el directorio "Mis documentos") a la que llamaremos "html". Dentro de ella iremos creando otras carpetas a las que iremos llamando "ejemplo_01", "ejemplo_02", etc... Como se verá más adelante, dentro de cada carpeta iremos poniendo muchos archivos que compondrán las diversas web de ejemplo que vayamos creando.

Los apuntes se han dividido en capítulos muy pequeños y lo más autocontenidos posible para intentar facilitar la asimilación de los conceptos en ellos presentados.

Los navegadores
===================

Cuando accedemos a Internet normalmente lo hacemos usando programas llamados "navegadores" (a veces también "browsers"). Hay muchos navegadores, algunos de los mas conocidos son:

* Firefox
* Chrome
* Internet Explorer (ahora conocido como Edge.)

Pregunta: navegadores
-----------------------

*¿Se puede acceder a cualquier web con cualquier navegador?*

Respuesta: **SÍ**. De hecho aquí está una de las fortalezas de la web.

.. IMPORTANT::
   Los navegadores descargan páginas escritas en un lenguaje llamado HTML que está **ESTANDARIZADO**. Gracias al estándar, cualquier persona o empresa puede crear un navegador o incluso un servidor de páginas web (e intentar venderlo si así lo desea).
   
El organismo que estandariza el lenguaje HTML es el World Wide Web Consortium o W3C y es un organismo sin ánimo de lucro que establece las reglas del lenguaje. Gracias a estos estándares libres, abiertos y gratuitos la Web ha podido avanzar muchísimo. A modo de ejemplo, las figuras siguientes muestran una página web mostrada en distintos navegadores.

.. figure:: imagenes/Captura_google.png
   :scale: 50%
   
   Captura de un buscador usando Mozilla Firefox.
   
   
.. figure:: imagenes/Captura_google_chrome.png
   :scale: 50%
   
   Captura de un buscador usando Google Chrome.
   
.. WARNING::
   En realidad, podría haber pequeñas diferencias pero este problema ocurre cada vez menos y se espera que con el tiempo haya cada vez menos diferencias.
   
En suma, lo importante es que el lenguaje es **abierto** y el W3C incluso publica los estándares del lenguaje para aquellos interesados en conocer los detalles más internos. Sin embargo, tales detalles quedan fuera del alcance de estos apuntes.

Primera página HTML
=====================

Antes de empezar vayamos al directorio "Mis documentos" y entremos dentro de la carpeta "html" que hicimos en su momento. Fabriquemos una nueva carpeta a la que llamaremos "ejemplo_01". Deberíamos ver algo como lo que muestra la figura.

.. figure:: imagenes/estructura_carpetas.png
   :scale: 50%
   
   Estructura de carpetas

Si ahora abrimos el "Bloc de notas" deberíamos ver algo como esto (este programa debería estar en el botón "Inicio" y dentro de él en "Accesorios").

.. figure:: imagenes/bloc_de_notas.png
   :scale: 25%
   
   Bloc de notas
   
   
Ahora podremos utilizar este programa para teclear nuestra primera página web.

Antes de empezar es importante conocer que HTML utiliza **marcas** para indicar como debe aparecer el texto en pantalla. Las marcas se escriben utilizando los símbolos "<" y ">". Dependiendo del teclado pueden estar en distintos sitios pero lo más común es que estén en la zona inferior izquierda del teclado y al lado de la tecla "z". Así una marca puede ser algo como "<h1>" o "<table>". Estas marcas **son la clave del lenguaje** ya que todo el lenguaje consta de marcas que nos permiten conseguir que la página se muestre como queremos. De hecho HTML significa HyperText Mark-up Language (algo así como "Lenguaje de marcas para hipertexto").

Además las marcas suelen tener una *apertura* y un *cierre*. Una marca de apertura podría ser "<h1>" y una de cierre "</h1>". El símbolo "/" suele estar en el teclado, en la tecla "7" y normalmente hay que pulsar la tecla "Mayúsculas" y "7" a la vez pero puede variar según el teclado.

Usemos ahora el Bloc de notas (a veces también llamado "editor") para escribir lo siguiente. En clase veremos que la estructura se puede modificar y por ejemplo se pueden escribir dos marcas seguidas o se puede dejar más de una línea en blanco, sin embargo las marcas sí deben escribirse exactamente igual.

.. code-block:: html

   <!DOCTYPE html>
   <html>
    <head>
        <title>
            Mi primera página web
        </title>
    </head>
    <body>
        <h1>Un ejemplo de página web</h1>
    </body>
   </html>
   
Una vez teclado, nos vamos al menú "Archivo" y dentro de él veremos una opción que pone "Guardar como". Guardaremos el archivo con el nombre "index.html" e indicaremos que **no vamos a guardar con la extensión .txt, sino que marcaremos la opción "Todos los archivos"**

.. figure:: imagenes/bloc_de_notas_guardando.png
   :scale: 30%
   
   Guardando el archivo.
   


Por desgracia el "Bloc de notas" intenta siempre guardar los archivos como "archivo.txt" y al crear páginas web nos interesa guardarlas como "loquesea.html", así que necesitaremos hacer esto.

Una vez hecho esto podemos ir a la carpeta "Mis documentos" y dentro de "html" deberíamos ver la carpeta "ejemplo_01" que debe contener el archivo "index.html" tal como muestra la figura siguiente:

.. figure:: imagenes/ejemplo_01_index.png
   :scale: 30%
   
   Nuestro archivo index.html
   
Si se hace doble click en dicho archivo deberíamos ver como el navegador de nuestro sistema muestra nuestra primera página web.



.. figure:: imagenes/primera_pagina.png
   :scale: 30%
   
   El navegador mostrando nuestra primera página web.
   
   
Si algo no funciona puede ser por alguno de estos motivos:

* Si al hacer doble click la página no se abre puede que tengamos que abrir primero el navegador y desde él usar el menú "Archivo" y luego "Abrir". Despues podremos ir a la carpeta "Mis documentos", "html", "ejemplo_01" y seleccionar el archivo "index.html"
* Si la página se abre pero no se muestra lo mismo que en la figura casi al 100% ha habido algún error al copiar las marcas. Vuelve al bloc de notas y repasa que todas las marcas sean exactamente iguales.

