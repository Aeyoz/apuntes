# Operaciones básicas con strings en python 3.10.7

### Funciones de los strings


cadena = "\t\t\t\taaa,aaaPassword: 1234,,,a,,,\n\n\n\n"

+ len(): Permite saber la longitud de la cadena (cuenta los caracteres de la cadena)

+ split(): Permite partir la cadena por el parametro pasado, es decir, si pasaramos cadena.split(",") la cadena sería troceada cada vez que hubiera una coma

+ strip(): Elimina por defecto los caracteres invisibles situados a los extremos de la cadena, por ejemplo \n (nueva linea) \t (tabulador), o si se le pasa

+ un parametro elimina SOLO ese parametro que aparezca en los extremos, si aparece otro antes que este no elimina nada por lo que habria que pasar este tambien, tipo, cadena.strip(",","\n", "\t", "a"), ahi elimina tanto los tabuladores, las comas, las a y las nuevas lineas que esten por los extremos de la cadena.

+ count(): Permite ver la cantidad de veces que aparece un caracter o una serie de caracteres en la cadena, si se hace cadena.count("a"), nos daría un total de 8, en cambio, si se hace cadena.count("Pa") da un total de 1.

+ index(): Encuentra la posición del caracter que se haya pasado, pasa la posición del primer caracter de este tipo en caso de que haya varios: cadena.index("a") da 7

+ find(): Funciona exactamente igual que index(): cadena.find("a") da 7

+ capitalize(): Pone la primera letra de la cadena en mayuscula 

+ title(): Pone la primera letra de cada palabra de la cadena en mayuscula

+ upper(): Convierte toda la cadena en mayuscula

+ lower(): Convierte toda la cadena en minúscula

+ swapcase(): Inverte el estado de cada uno de los elementos de la cadena, es decir, las mayus son minus y viceversa
+ replace(): Cambia el primer valor que se haya pasado por el segundo, se puede decidir la cantidad de veces que se desea realizar el cambio:

proverb = 'Quien mal anda mal acaba'

proverb.replace('mal', 'bien')
'Quien bien anda bien acaba'

proverb.replace('mal', 'bien', 1)  # sólo 1 reemplazo
'Quien bien anda mal acaba'

+ endswith() y startswith(): devuelven True o False, comprueba que la cadena empiece o termine con el parametro pasado.

La diferencia entre index y find reside en que find cuando no encuentra el valor que se ha pasado devuelve -1, mientras que index devuelve un error.

### Acceso a la cadena

cadena = "Hola mundo!"


cadena[1] == "o" Devuelve el caracter el la posición 1

cadena[::-1] == "!odnum aloH" Devuelve la cadena de texto invertida (a lo mejor lo pone en el examen si se pasa de pinche lanza)

cadena[1:7] == "ola mu" Devuelve los caracteres entre los indices 1 y 7 sin contar el 7.

cadena[1:7:2] == "oam" Devuelve la los caracteres entre los indices 1 y 7 en saltos de 2 caracteres

cadena[2:] == "a mundo!" Devuelve todos los caracteres a partir del segundo inclusive

cadena[:4] == "Hola" Devuelve todos los caracteres desde el indice 4 hacia atrás


### F-strings

Una f-string permite incorporar a una cadena de texto el valor de la variable sin tener que descontinuar la cadena misma, ejemplo:
world = "mundo"
f"Hola {world}!" Devuelve "Hola mundo!"

### Formateando valores

Mejor lean los apuntes del profe en este punto.
