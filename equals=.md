Lo que hace == es comparar el objeto no el contenido para comparar el contenido tenemos que utilizar es `equals`

Ejemplos:
var a = "Hello World";
var b = "Hello World";
var c = new String("Hello World")

si hago una comparacion en la que imprimo a comparando a == b y a == c 
me daria true y false incluso teniendo el mismo contenido. 
Para comparar el contenido de un objeto tenemos que utilizar equals
a.equals(c)
esto nos devuelve true 

Mas tipos de equals