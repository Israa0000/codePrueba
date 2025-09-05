### Operadores de comparacion
1. NOT / !
2. AND / &&
3. OR / ||
este es el orden en el que la maquina lee los operadores de comparacion **SI NO HAY PARENTESIS**

Si aparece en una linea varios valores booleanos sin una complaracion siempre se leera como `= true` es decir`
`if (a && b)` se leera `if (a && b = true)`
`if (a || b)` se leera `if (a || b = true)`
`if (!a)` se leera `if (!a = true)`

### AND / && CONJUNCIÓN LÓGICA
Este operador solo devuelve verdadero si ambos valores de entrada son verdaderos 

#### Ejemplo
`A && B = true`  solo debuelve verdadero si:

A es verdadero `A = true` **Y** B es verdadero `B = true`

si uno de estos valores es falso nos devolvera falso **porque no se cumplen ambas condiciones**

`true && true = true`
`true && false = false`
`false && true = false`
`false && false = false`

### OR / || DISLUNCIÓN LÓGICA
Este operador devuelve verdadero si al menos uno de los valores es verdadero, solo sera falso cuando todos los valores son falsos

#### Ejemplo
`A || B = true` Es verdadero si `A = true` **O** si `B = true` o si los dos son verdaderos 
La unica forma de que devuelva `false` es cuando ambos o todos los valores son falsos

`true || true = true`
`true || false = true`
`false || true = true`
`false || false = false`

### NOT / ! NEGACIÓN LÓGICA
Invierte el valor logico que le des
Devuelve verdadero si la entrada es falsa y devuelve falso si la entrada es verdadera

#### Ejemplo
Si `A = true` significa que `!A = false`
Si `B = false` significa que `!B = true`

### Ejecicio y explicación
``! (true && false) || (false && !true) && true``

Empezamos por los parentesis:

1. `(true && false)`
como los dos valores no son verdaderos no dara `false`

2. `(false && !true)`
empezamos por la negacion a `!true` lo que revertiria su valor y nos daria:

`(false && false)` en esta ocasion ambos valores son `false` lo que nos dara `false`

Bien ahora si los parentesis tenemos 

`!false || false && true`

Segun las leyes de precedencia maquina leera los operadores de operacion tal que asi
1. ! 
2. &&
3. ||

Empezamos con `!false` lo que revertiria su valor = `true`

`true || false && true`

Seguiriamos por `false && true`, en esta ocasion los dos valores no son `true` a si que no daria `false`

`true || false`

Y por ultimo tenemos un true en esta comparación por lo que nos devolveria `true`


``! (true && false) || (false && !true) && true = true``
