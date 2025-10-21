Imagina esto:

Tienes una caja de 7 papeles, y cada papel tiene escrito un día de la semana:

String[] dias = {"Lunes", "Martes", "Miércoles", "Jueves", "Viernes", "Sábado", "Domingo"};


Ahora tú quieres sacar uno por uno los papeles para leer lo que dice cada uno.

Ahí es donde entra el for-each.

🤖 ¿Qué hace el for-each?
for (String dia : dias) {
    System.out.println(dia);
}


Esto significa:

“Dame uno de los papeles, guárdalo temporalmente en la variable dia, y haz algo con ese papel.
Luego, dame el siguiente papel, guárdalo en dia, y haz lo mismo.
Haz eso con todos los papeles, uno por uno.”

🧠 Palabras más claras para entender for-each

En lugar de decir "recorrer", piensa que el for-each sirve para:

Usar cada elemento de una lista/arreglo, uno a uno.

Aplicar una acción a cada elemento.

Revisar cada cosa dentro de una colección.

🧪 Veamos un ejemplo con frutas
String[] frutas = {"Manzana", "Banana", "Pera"};

for (String fruta : frutas) {
    System.out.println("Estoy comiendo una " + fruta);
}


Significa:

Toma el primer valor del arreglo ("Manzana"), guárdalo en fruta, y haz el println.

Luego toma el segundo ("Banana"), guárdalo en fruta, y haz lo mismo.

Luego el tercero ("Pera"), y listo.

🎮 Ejemplo paso a paso
String[] numeros = {"Uno", "Dos", "Tres"};

for (String numero : numeros) {
    System.out.println("Número actual: " + numero);
}


Aquí no estás pensando en posiciones ni en cuántos elementos hay.

Solo dices: “Dame el siguiente y úsalo”.

🛠 Comparación mental
Tipo	Forma de pensar
for clásico	"Quiero usar el elemento que está en la posición 0, luego 1, luego 2..."
for-each	"Solo quiero usar cada valor de la lista, uno por uno. No me importa la posición."
💬 Frase final para recordarlo

El for-each se usa cuando tú quieres hacer algo con cada cosa en una lista, sin preocuparte por dónde está o cómo se llama su lugar.