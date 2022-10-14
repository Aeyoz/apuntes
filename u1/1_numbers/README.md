# Operaciones básicas con números en python 3.10.7

Las variables y las constantes se escriben en python de la siguiete manera:
```
variable:
x = 4
CONSTANTE:
PI = 3.14

Las constantes van en mayuscula ya que es un valor que no va a cambiar en ningun momento, en cambio la variable es posible que sí

```

### Operaciones posibles en python:

+ Suma (+)
+ Resta (-)
+ Exponenciación (Elevar un número a una potencia)(**): Ejemplo: 2 ** 3 == 8
+ División (/): Devuelve el cociente de la división, con decimales si los tuviera, por ejemplo: 3 / 2 == 1.5
+ División entera (//): Devuelve la parte entera del cociente de la división, por ejemplo: 3 / 2 == 1
+ Módulo (%): Devuelve el resto de una división, por ejemplo: 5 % 2 == 1
+ Absoluto de un número: Se usa la función abs(n) para que el número n sea devuelto como absoluto, por ejemplo el absoluto de -2 es 2

### Tipos de datos:

Por ahora los tipos de datos que hemos estudiado han sido booleanos, enteros, flotantes, complejos y strings.

|Nombre|Tipo|Ejemplo|
+----------+------+-------+
| Booleano | Bool | True, False|
| Entero | Int | 21, 34500, 34_500 (los 2 ultimos son el mismo número)|
| Flotante | Float | 3.14, 27.5e3|
| Complejo | Complex | 2j, 3 +5i |
| Cadena de texto | str | "TNF", "1", '''Tenerife - Islas Canarias''' |
| Tupla | Tuple | (1, 2, 3, 4, 5) |
| Lista | List | ["Chrome", "Firefox"] |
| Conjunto | set | set([2, 4, 6]) |
| Diccionario | dict | {"Chrome": "v89", "Firefox" : "v87"} |


### Normas de escritura del código de python:

+ No hace falta hacer un comentario de cada una de las acciones del código.
+ Intentar no pasar de 80 columnas en el código.
+ Usar la gramática, por ejemplo: 8, 9 (bien); 8 , 9(mal)
+ Los nombres de las variables deben de ir en inglés y en minúscula
+ Los nombres de las constantes deben de ir en mayúscula y en inglés.
+ Tanto las variables como las constantes deben de empezar por minúsculas y puden contener los siguientes caracteres:
    + Letras minúsculas.
    + Letras mayúsculas.
    + Dígitos.
    + Guiones bajos (_).ç
+ Las variables no pueden empezar ni por guiones bajos ni por numeros ni por caracteres especiales, tampoco pueden ser palabras reservadas por el lenguaje, por ejemplo: len = 7 no es posible debido a que len es una función que indica la longitud de un elemento, en cambio length = 7 si porque no es ninguna palabra reservada.


### Bases

Base binaria:
Lleva el prefijo 0b, por ejemplo:
0b1001 es el número 9 en binario
Base hexadecimal:
Lleva el prefijo 0x, por ejemplo:
0x7F2A es el número 32554 en hexadecimal
Base octal:
Lleva el prefijo 0c, por ejemplo:
0c6243 es el número 3235 en octal
Para convertir a un decimal se usa int de la misma manera que se muestra abajo.


Para convertir un número de decimal a cualquier tipo de las bases anteriores estan las funciones oct(), hex() y bin(), además, se puede convertir cualquier número siempre que se indique la base, por ejemplo:

bin(0x7F2A) daría 0b111111100101010.