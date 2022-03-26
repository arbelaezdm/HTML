JSDoc sirve para transformar las notas en HTML

# HTML

- Introduccion a HTML
- Etiquetas y atributos
- Elementos de línea y de bloque
- Etiquetas de texto
- Listas
- Rutas, hipervinculos e imagenes
- Indotruccion a semantica
- Estructura de un sitio web

# Creando la estructura de un sitio web

Con HTML podemos crear todos los elementos visuales de un sitio web, ya sean textos, imagenes, formularios e inclusto tros contenidos mas avanzados.

#HTML
##HTML
HTML es un lenguaje de marcado que permite, mediante etiquetas, generar contenido visible dentro de nuestro sitio web. Podemos crear desde elementos simples, como titulos, hasta elementos mas complejos, como formularios.

## Flow del sitio

Si un elemento ocupa toda la pantalla, el siguiente colapsará y caera el primer lugar que tenga disponible.

## Etiquetas

Las etiquetas estan conformadas por etiquetas de apertura <> y etiqueta de cierre</>
A las etiquetas se les agrega un contenido y da por resultado a un elemento HTML.

Etiquetas + Contenido = Elemento

## Atributos

Es una caracteristica de la etiqueta que queremos como modificas tales como: color de la fuente, tipo de fuente, tamaño de fuente, etc.
Los atributos esta conformados por:

- Nombre del atributo
- Un signo igual
- El valor del atributo entre comillas

**Ejemplo:**

<h1 align = "center"> Hola Mundo </h1>

Todo documento HTML debe tener una estructura basica que debe estar presente en todo contenido HTML.

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title></title>
</head>
<body>
</body>
</html>

Esta estructura le permite al navegador saber que va a recibir un documento con lenguaje HTML y que deberá visualizarlo de manera correcta.

## Etiqueta Doctype

Definir la version de HTML que se esta utilizando. Ahora se trabaja con la version 5

##Etiqueta html
Define que todo su contenido interno será HTML

## Etiqueta head

Guarda toda la informacion referente con el documento tales como la codificacion de caracteres, el titulo a mostrar en la pestaña del navegador, etc.

## Etiqueta meta

Es de uso multiple se usa particularmente para definir a partir de charset la codificacion del documento.

## Etiqueta title

Aca se escribe lo que se mostrará en la etiqueta del navegador

## Etiqueta body

Es donde va a contener todas las demas etiquetas que son las que van a generar contenido visual. Aca es donde va todo el contenido de la pagina en si.

## Nota

Algunas etiquetas pueden contener otran etiquetas dentro de ellas. A este concepto se le conoce como anidamiento de etiquetas que es super importante para escribir un documento de HTML

##Elemento de línea y de bloque

- Elementos en linea
- Elementos de bloque
- Elementos de semi-bloque
- Elementos ocultos

## Elementos de bloque

Es aquel que independiente de su contenido interno ocupara todo el espacio del que dispone a lo ancho sin permitir que otros elementos se posicione a sus costados laterales.

## Elementos de linea

Son todo lo contrario a los elementos de bloque, ocupan el espacio que les corresponde exclusivamente a su extension de contenido interno.

Al momento de diagramar un sitio web necesitamos disponer de etiquetas que corten el flujo de elementos que generen una suerte de saltos de linea. El objetivo es poder generar un esquema visual mucho mas organizado y funcional para la elegibilidad del visitante de la pagina.

# Propiedades

## display

Mediante la propiedad display de CSS podemos cambiar la disposicion del elemento que queramos. Los valores que recibe son block, inline, inline-block y none.

**Inline**
Define un elemento con comportamiento en linea. NO recibe algunas propiedades del modelo de caja.

**Block**
Define un elemento con comportamiento en bloque. Puede recibir propiedades del modelo de caja.

**Inline-block**
Define un elemento con comportamiento de semi-bloque. Puede recibir propiedades del modelo de caja, y tambien comparte propiedades de elementos de línea.

**None**
Oculta un elemento. No lo elimina de la estructura de HTML, solo desaparece de la vista

# Etiquetas de Texto

##header < h> - Elemento de bloque
Representan titulares o headers.
Van desde h1 hasta h6

Se usa para generar un bloque diferencial de texto respecto al contenido.
h1 no deberá ser utilizado mas de 1 vez dentro de un documento HTML dado a que este representa el titulo de mayor importancia

## paragraph < p> - Elemento de bloque

</p>
Sirve para generar bloques de texto . Se pueden usar las veces que lo requerimos. Esta es una de las etiquetas mas utilizadas dentro de un sitio web.

## cursiva < em> - Elemento de línea

Este sirve para colocar la letra en cursiva

##negrita < strong> - Elemento de linea
Sirve para colocar la letra en negrita.

## salto de linea < br>

De break line, esta etiqueta sirve para generar saltos de linea entre las distintas lineas de un parrafo

## Listas - Elementos de bloque

Sirven para generan un listado de elementos que podemos identificar facilmente.
Estas deberan estar dentro de la etiqueta <li>
Estas tienen dos variantes: listas ordenadas y listas desordenadas.

## Lista Ordenada <ol>

Es aquella que genera una viñeta numerica

## Lista desordenada <ul>

Es aquella que genera una viñeta de bullet o punto

## Rutas - Hipervinculos e Imagenes

## Ruta

Una ruta en HTML es un trayecto que un documento debe atravesar hasta llegar a una ubicacion de un determinado recurso.
Existen dos clases de rutas:

- Relativas: son aquellas que contienen solamente la informacion necesaria para que el documento HTML llegue a la ubicacion del recurso determinado. Es como cuando queremos saber la ruta donde se encuentra una foto en nuestro pc. c:/Documents/imagenes/yo.png. En sintexis estas rutas contienen las coordenadas parciales de una determinada ubiacion mas alla de la cual sea la ruta asignada para nuestros documentos HTML. NO pueden hacer referencia a una carpeta dentro del disco de nuestro PC. Deben ser facilmente identificables por el documento dentro del cual las estamos gestionando.
  **Ruta Relativa:** ../imagenes/yo.png

- Absolutas: son aquellas que contienen toda la informacion de la ubicacion de un recurso determinado. un ejemplo es la URL de un sitio web. Generalmente este tipos de rutas hacen relacion a una ubicacion dentro de internet. Son coordenadas exactas para su ubicacion determinada.
  **Ruta Absoluta:** https//www.google.com

## Imagenes <img>

No requiere etiqueta de cierre pero si de los siguientes atributos:

- src="" => ruta de la imagen a mostrar. Puede ser una ruta relativa o una ruta absoluta.
  En la ruta absoluta no es necesario que la imagen este en nuestro PC, esta esta siendo llamada desde una ubicacion en internet.
  En la ruta relativa si se requiere que el archivo de imagen este en alguna carpeta de nuestro proyecto, la cual será realativa a la ubiacion del archivo HTML
- alt="" => texto alternativo o descriptivo de la imagen

## Enlaces o Hipervinculos <a>

Son etiquetas de HTML que nos permite vincular distintos archivos entre si o distintas ubicaciones en internet.
Esta etiqueta necesita de una referencia o atributo href="" donde se escribirá la ruta del recurso que deseamos vincular.
Existen enlaces externos o enlaces locales.

## Enlaces Externos

Son los que nos llevan a un recurso externo, es decir, otro sitio web.

## Enlaces Locales

Son los que nos permiten enlazar nuestros recursos presentes en la misma carpeta del archivo de nuestro proyecto

## Semantica

Cuando realizamos nuestro codigo es muy importante que desde las etiquetas empecemos a poner un orden semántico. El objetivo es que a través de las mismas, y a simple vista, podamos identificar un encabezado, la seccion principal del sitio, distintas secciones, articulos, cual es el pie pagina o una barra de navegación.

Ademas es importante que los usuario entren al mismo y lo conozcan, ya sea a traves de una busqueda o publicidad.

Con base en esto debemos tratar de darle orden al codigo como por ejemplo:

## Etiqueta header - etiqueta de bloque

Nos sirve para generar la cabecera del documento, o incluso tambien para generar la cabecera de una seccion de contenido

<header>
   Logotipo
   Barra de navegación
   Barra de busqueda
   Enlaces a redes sociales
</header>

## Etiqueta nav - etiqueta de bloque

Dentro de esta etiqueta se suele implementar la navegacion al rededor de listas desordenadas, elementos de listas y enlaces o hipervinculos

<nav>
   <ul>
      <li><a href="#" >Inicio</a> </li>
      <li><a href="#" >Quiénes somos</a> </li>
      <li><a href="#" >Servicios</a> </li>
      <li><a href="#" >Contacto</a> </li>
   </ul>
</nav>

## Etiqueta footer - etiqueta de bloque

Servirá para generar el pie de pagina principal del documento o el pie de pagina de una sección de contenido

<footer>
   <p>Todos los derechos reservados</p>

   <nav>
      <ul><a href="#">Terminos y condiciones</a></ul>
      <ul><a href="#">Mapa del sitio</a></ul>
      <ul><a href="#">Informacion legal</a></ul>
   </nav>
</footer>

## Etiqueta section - etiqueta de bloque

Servira para definir una sección de contenido o monotematica. Dentro de esta se puede utilizar un footer o un header si fuese necesario.
Esta podrá tener contenido que podría funcionar por si solo sin necesidad de todo lo que lo rodea: un producto, un servicio, una noticia, etc.

<section>
   <header>
      <h2>Productos destacados</h2>
   </header>

Descripcion del producto: Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit perspiciatis nihil provident fugit ipsa, facere laboriosam ab nam reprehenderit dolore temporibus sed, enim vel corrupti reiciendis maxime voluptates vitae repellat?

   <footer>
      <a href="#">Continuar leyendo</a>
   </footer>

</section>

## Etiqueta article - etiqueta de bloque

Servirá para definir una porcion de contenido dentro de una seccion.
Sirve para generar distintos apartados de texto o contenido de una misma tematica.
No necesariamente debe ir dentro de un section

<section>
   <header>
      <h2>Producto destacado</h2>
   </header>

<article>
   Descripcion del producto - Lorem ipsum dolor sit amet consectetur adipisicing elit.
</article>

</section>
