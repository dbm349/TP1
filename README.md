# TP1-WEB
# 1. ¿Qué es un lenguaje de marcado? ¿Cuál es su utilidad? ¿Qué es un tag? ¿Qué es un atributo?
Un lenguaje de marcado, es un lenguaje que permite elaborar la estructura de un texto mediante el uso de etiquetas o tags. Este no debe confundirse con un lenguaje de programación ya que no son lo mismo. 
La utilidad de este lenguaje es que nos permite añadir un significado a cada parte de nuestro texto.
Un tag nos permite delimitar los elementos de nuestro documento por ejemplo encabezado, párrafos, etc. La mayoría de los tag constan de los símbolos <> utilizando dos tags, uno para el inicio de la etiqueta y otro para el final con el símbolo /, aunque algunos solo tienen marca inicial. (Por ejemplo <head></head>). Cada tag puede admitir atributos los cuales se incluyen a continuación del nombre de la etiqueta. Estos nos brindan información adicional sobre cada etiqueta.

# 2. ¿Cuál es la utilidad de HTML?  ¿Qué conjunto mínimo de tags debe contener un documento elaborado en este lenguaje? Describa brevemente su utilidad.
El HTML o Hypertext Markup Language es un tipo de lenguaje de marcado el cual nos permite elaborar páginas web utilizando etiquetas. 
La estructura global de HTML consta del siguiente conjunto mínimo de tags:
En primer lugar todo HTML debe iniciar con la etiqueta <!DOCTYPE HTML> el cual indica que nuestro documento es del tipo html5, la ultima versión.
Luego se utiliza las etiquetas <html></html> la cual va a envolver todo nuestro documento html.
La etiqueta <head> corresponde al encabezado de nuestro documento dentro del cual podemos especificar el título del documento con el encabezado <title>.
Y por último con los tags <body></body> definiremos todo el cuerpo del documento.
Un ejemplo de la estructura podría ser:
	
<!DOCTYPE HTML>
<html>
	<head>
		<title>Mi pagina web</title>
	</head>
	<body>
		<p>Aquí escribo un párrafo</p>
	</body>
</html>

# 3. ¿Cuál es la utilidad e importancia de los enlaces o links entre páginas? ¿Qué significa hipertexto? ¿Un link solo puede apuntar a otra página? ¿Qué importancia tiene esto último?
Un hipertexto básicamente es un texto que contiene enlaces a otros textos. Por lo tanto, los enlaces o links son de vital importancia ya que nos dejan navegar entre las distintas páginas, creando así una interconexión entre las mismas. Los links no solo tienen que ser texto, sino que pueden ser también imágenes u otros elementos HTML. Cada link puede apuntar a un recurso como otra página, un archivo, etc., pero solo uno, lo cual nos permite no solo navegar entre páginas sino, por ejemplo, descargar contenidos como un archivo multimedia referenciado en el link.

# 4. ¿Cómo funcionan los tags audio y video?
Los tags audio y video funcionan de la siguiente manera: cuando queremos incluir en nuestro sitio un archivo multimedia como audio o video mediante estas etiquetas (Por ejemplo: <audio></audio>) tendremos que ingresar entre este conjunto de etiquetas de inicio y fin, otra etiqueta para indicar el origen de dichos archivos (<source>) especificando con los atributos ‘src’ la ubicación fisica y ‘type’ el tipo de audio o video. Un ejemplo concreto podría ser el siguiente:

<audio controls>
 	<source src="audio.ogg" type="audio/ogg">
 	<source src="audio.mp3" type="audio/mpeg">
	El navegador no soporta el video.
</audio>

Como no todos los navegadores soportan el mismo tipo de archivo multimedia tanto de audio o de video, podemos incluir distintos archivos del mismo video, pero con varios formatos, como en el ejemplo anterior se incluye primero un audio formato ogg, luego el mismo en formato mp3 y por ultimo un aviso de que el navegador no soporta el audio. Asi el navegador recorrerá cada etiqueta ‘source’ desde arriba viendo si soporta el archivo, pasando al siguiente en caso de no poder o mostrando el último mensaje si no soporta ninguno de los tipos especificados.

# 5. ¿Qué es el Rendering Engine de un Browser? ¿Cuál es el que utiliza cada uno de los 5 browsers más conocidos (Chrome, Firefox, Safari, IE-Edge, Opera)? ¿Cuál es la importancia de conocer cada uno de ellos en la construcción de un sitio? 


