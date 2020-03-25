# TP1-WEB

**El objetivo de este tp consiste en adquirir los conocimientos básicos sobre el marcado de una página web.

Con respecto a los ejercicios de la parte teorica se encuentra realizada en este mismo documento y en cuanto a la práctica, la resolución de los mismos se encuentran almacenado de la siguiente manera:

En la carpeta tp1/Capturas lujan.gob.ar se encuentra resuelto la primer parte el ejercicio 6 de la práctica que consiste en dibujar el Wireframe correspondiente a la página principal de lujan.gob.ar. La segunda parte de este punto se basa en desarrollar, en función al Wireframe realizado anteriormente, el código HTML5 correspondiente(el mismo se encuentra en tp1/TP_1-Practico6.html).

El siguiente ejercicio(Número 7) consiste en elaborar en HTML5 una página que contenga un currículum vítae, respetando la estructura dada en el trabajo, teniendo en cuenta que los elementos subrayados son enlaces a páginas web o a direcciones de correo electrónico y que la foto debe ser un enlace a la propia imagen. En la carpeta tp1/imagenes se encuentran las imagenes que forman parte del contenido del curriculum y el código correspondiente a este se encuentra en tp1/TP_1-Practico7.html).

El último ejercicio(Número 5), se basa en elaborar el código que represente a la tabla dada por los docentes. La resolución de este punto se localiza en la carpeta tp1/TP_1-Practico5.html.



# TEORIA
## 1. ¿Qué es un lenguaje de marcado? ¿Cuál es su utilidad? ¿Qué es un tag? ¿Qué es un atributo?
Un lenguaje de marcado, es un lenguaje que permite elaborar la estructura de un texto mediante el uso de etiquetas o tags. Este no debe confundirse con un lenguaje de programación ya que no son lo mismo. 
La utilidad de este lenguaje es que nos permite añadir un significado a cada parte de nuestro texto.
Un tag nos permite delimitar los elementos de nuestro documento por ejemplo encabezado, párrafos, etc. La mayoría de los tag constan de los símbolos `<>` utilizando dos tags, uno para el inicio de la etiqueta y otro para el final con el símbolo /, aunque algunos solo tienen marca inicial. (Por ejemplo `<head></head>`). Cada tag puede admitir atributos los cuales se incluyen a continuación del nombre de la etiqueta. Estos nos brindan información adicional sobre cada etiqueta.

## 2. ¿Cuál es la utilidad de HTML?  ¿Qué conjunto mínimo de tags debe contener un documento elaborado en este lenguaje? Describa brevemente su utilidad.
El HTML o Hypertext Markup Language es un tipo de lenguaje de marcado el cual nos permite elaborar páginas web utilizando etiquetas. 
La estructura global de HTML consta del siguiente conjunto mínimo de tags:
En primer lugar todo HTML debe iniciar con la etiqueta `<!DOCTYPE HTML>` el cual indica que nuestro documento es del tipo html5, la ultima versión.
Luego se utiliza las etiquetas `<html></html>` la cual va a envolver todo nuestro documento html.
La etiqueta `<head>` corresponde al encabezado de nuestro documento dentro del cual podemos especificar el título del documento con el encabezado `<title>`.
Y por último con los tags `<body></body>` definiremos todo el cuerpo del documento.
Un ejemplo de la estructura podría ser:

```html
<!DOCTYPE HTML>
<html>
	<head>
		<title>Mi pagina web</title>
	</head>
	<body>
		<p>Aquí escribo un párrafo</p>
	</body>
</html>
```

## 3. ¿Cuál es la utilidad e importancia de los enlaces o links entre páginas? ¿Qué significa hipertexto? ¿Un link solo puede apuntar a otra página? ¿Qué importancia tiene esto último?
Un hipertexto básicamente es un texto que contiene enlaces a otros textos. Por lo tanto, los enlaces o links son de vital importancia ya que nos dejan navegar entre las distintas páginas, creando así una interconexión entre las mismas. Los links no solo tienen que ser texto, sino que pueden ser también imágenes u otros elementos HTML. Cada link puede apuntar a un recurso como otra página, un archivo, etc., pero solo uno, lo cual nos permite no solo navegar entre páginas sino, por ejemplo, descargar contenidos como un archivo multimedia referenciado en el link.

## 4. ¿Cómo funcionan los tags audio y video?
Los tags audio y video funcionan de la siguiente manera: cuando queremos incluir en nuestro sitio un archivo multimedia como audio o video mediante estas etiquetas (Por ejemplo: `<audio></audio>`) tendremos que ingresar entre este conjunto de etiquetas de inicio y fin, otra etiqueta para indicar el origen de dichos archivos (`<source>`) especificando con los atributos ‘src’ la ubicación fisica y ‘type’ el tipo de audio o video. Un ejemplo concreto podría ser el siguiente:


```html
<audio controls>
 	<source src="audio.ogg" type="audio/ogg">
 	<source src="audio.mp3" type="audio/mpeg">
	El navegador no soporta el video.
</audio>
```

Como no todos los navegadores soportan el mismo tipo de archivo multimedia tanto de audio o de video, podemos incluir distintos archivos del mismo video, pero con varios formatos, como en el ejemplo anterior se incluye primero un audio formato ogg, luego el mismo en formato mp3 y por ultimo un aviso de que el navegador no soporta el audio. Asi el navegador recorrerá cada etiqueta ‘source’ desde arriba viendo si soporta el archivo, pasando al siguiente en caso de no poder o mostrando el último mensaje si no soporta ninguno de los tipos especificados.

## 5. ¿Qué es el Rendering Engine de un Browser? ¿Cuál es el que utiliza cada uno de los 5 browsers más conocidos (Chrome, Firefox, Safari, IE-Edge, Opera)? ¿Cuál es la importancia de conocer cada uno de ellos en la construcción de un sitio?
El motor de renderizado de un browser es un software que adquiere un contenido marcado(como por el HTML, XML) e información de formateo(como CSS), lo interpreta y lo representa de manera visual a los usuarios. Son utilizados por los navegadores para mostrar contenido web  
Los motores de renderizado utilizado por los diferentes navegadores son:
-Chrome => Blink
-Firefox => WebRender
-Safari => WebKit
-IE-Edge => Chromium
-Opera => Blink
La importancia de conocer a cada uno de ellos, es que a la hora de construir un sitio web podemos elegir el motor que contenga la mayor cantidad de funcionalidades que necesitamos, ya que poseen diferentes velocidades de carga y vistas de las páginas web, entre otras características.

