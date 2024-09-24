# <center>JavaScript Algorithms and Data Structures</center>

Podemos asignar valores utilizando el operador de asignación “=”.

`let hello = "Hello";`

Asignar un valor a una variable al momento de declararla es conocido como “initialization”.

Iniciar la variable *“character”* asignando el valor *“Hello”* durante su declaración.

JavaScript tiene **siete tipos** de información primitiva, “String” siendo uno de ellos.
En JavaScript, un string representa una secuencia de caracteres que pueden ser encapsulados con comillas simples (‘) o comillas dobles (“).

Cabe destacar que los string son *inmutables*, significa que al ser creados, no pueden ser cambiados. La variable puede ser reasignada a otro valor.

La consola nos permite imprimir y ver la salida o resultado de JavaScript. Podemos enviar información a la consola utilizando *“console.log()"*. Por ejemplo, el siguiente codigo imprimirá “Naomi” a la consola.

`let developer = "Naomi";`\
`console.log(developer);` 

El código de arriba accede a la variable developer con su nombre en el *console.log()*.
Notemos que el valor que está dentro del paréntesis es lo que se va a imprimir.

Cuando una variable es declarada con la palabra clave let, podemos reasignar ( o cambiar el valor de ) la variable más tarde. El valor de la variable *programmer* es cambiada de **“Naomi”** a **“CamperChan”**.

`let programmer = "Naomi";`\
`programmer = "CamperChan"`

<span style="color: lightgreen;">Resaltemos que cuando reasignamos la variable, no utilizamos nuevamente la palabra clave ***let***.</span>

En el siguiente paso, loggeemos la variable *character* a la consola. Deberíamos de ver el string **“Hello”** y luego el string **“World”**, en la consola.

Cuando el nombre de la variable tiene más de una palabra, hay reglas específicas en cómo las capitalizamos, ***en JavaScript*** la regla básica que se utiliza es el *CamelCase*.

*CamelCase* significa que la primera palabra del nombre está completamente en minúscula, pero para las próximas palabras, la primera letra empieza en *mayúscula*.

Declarar una nueva variable utilizando *CamelCasing*.

`let secondCharacter;`

<span style="color: red;">**Cuando declaramos una variable sin asignarle un valor está considerada no iniciada.**</span>

Actualmente nuestra variable *secondCharacter* no está inicializada.
Al hacer un *console.log()* de una variable no inicializada nos devuelve ***“undefined”***.
*Este es un tipo de dato que representa que un valor no tiene una definición todavía*.

Si se puede asignar un valor a una variable que no fue inicializada:

`let uninitialized;` \
`uninitialized = "assigned";`

También se puede asignar el valor de una variable a otra variable.

`let first = "One";`\
`let second = "Two";`\
`second = first;`

La variable *second* ahora va a tener el valor de *“One”*.

Para aclarar el funcionamiento de esto:

`let character = "Hello";`\
`console.log(character);`

Inicializamos una variable con nombre **character** con el *string “Hello”*, el *console.log(character)* imprimirá *“Hello”*.

`character = “World”;`

Se reasigna el valor de la variable *character* al string *“World"*

`let secondCharacter;`

Declaramos una variable sin iniciarla con el nombre *secondCharacter.*

`secondCharacter = character;`

Asignamos el valor de **character** a *secondCharacter*.

`console.log(secondCharacter);`

Imprimimos nuevamente el nuevo valor de *secondCharacter* qué es el valor de **character**.


`let character = 'Hello'; -> Variable inicializada`\
`console.log(character); -> Console log 1`\
`character = "World"; -> Reasignación de character`\
`let secondCharacter; -> Variable no iniciada`\
`secondCharacter = character; -> Asignación de valor`\
`console.log(secondCharacter); -> Console log 2`

Borrar los dos **console.logs()** y la reasignación de **character**.\
Borrar la variable **secondCharacter**, pero dejar la inicialización de **character**.

`let character = 'Hello'; -> Variable inicializada`

#

Antes de avanzar es mejor tomarse un momento para reforzar lo que vimos.

Utilizar la palabra clave *let* para declarar una variable llamada **profession** y otra **age**.
Inicializamos **profession** con el *string “teacher”*, pero no inicializamos **age**.

`let profession = "teacher";`\
`let age;`

Utilizamos *let* para declarar una variable llamada **count**, asignar el **valor númerico 8**.\
Cuando utilizamos un valor numérico no utilizamos comillas, por ejemplo:

`let money = 100;`

Con el tipo de dato valor númerico, podemos realizar operaciones matemáticas, como suma, resta, entre otras.

**Intentemos imprimir *count + 1* a la consola.**

`let character = 'Hello';`\
`let count = 8;`

`console.log(count + 1);`\
`console.log(count / 2);`\
`console.log(count * 3);`\
`console.log(count - 4);`

#

En programación, usualmente voy a trabajar con mucha información. Hay muchos tipos de estructura que pueden ayudarte a organizar y manejar tu información.
Una de las estructuras de información más básicas es un *array*.

Los *array* es un tipo de información no primitivo. El tipo de información no primitiva en Java no están predefinidas. Son creados por el programador, estos también son llamados variables de referencia o referencias de objeto, ya que hacen referencia a un lugar en la memoria donde está guardada la información, non-primitive data se diferencia de primitive data ya que puede almacenar información más compleja, primitive data types como strings y numbers solamente puedan almacenar un valor al mismo tiempo.

Los arrays son denotados utilizando los corchetes **“[“** y **“]”**.

`let array = [];`

Declaro una variable llamada rows y le asigno un empty array.

`let rows = [];`

Cuando un *array* almacena valores o elementos, esos valores son separados con comas.

`let array = [“first”, “second”];`

Cambiar la declaración de la variable **rows** para que sea un *array* con ***strings “Naomi”, “Quincy”, y “CamperChan”***. El orden de los valores en un array es importante, entonces sigamos ese orden y recordando que en este caso, los strings son case-sensitive.

`let rows = [“Naomi”, “Quincy”, “CamperChan”];`

Podemos acceder a los valores dentro de un *array* utilizando el index **(posición)** de ese valor.
Un index es un número representando la posición del valor dentro del array, empezando en el 0 como el primer valor.

Podemos acceder al valor utilizando *bracket notation*, como por ejemplo **array[0]**.

Utilizar **console.log** y bracket notation para imprimir el primer valor de mi array llamado **rows**.

`let rows = ["Naomi", "Quincy", "CamperChan"];`
`console.log(rows[0]);`

Los *arrays* son especiales ya que **son considerados mutables**. Esto significa que *puedes* cambiar el valor de un index directamente.

Por ejemplo, el siguiente código va a asignar el *número 25* al **segundo elemento** en el *array*.

`let array = [1, 2, 3];`\
`array[1] = 25;`\
`console.log(array); // prints [1, 25, 3]`

Actualizar el **tercer elemento** en tu *array* llamado **rows** para que sea el **número 10**.
Luego imprimir el *array* **rows** a tu consola.

`rows[2] = 10;`\
`console.log(rows); // prints [“Naomi”, “Quincy”, 10]`

Esto es llamado **mutación**. Antes de avanzar esta es una buena oportunidad para aprender un uso normal del array. Actualmente, nuestro código accede al último elemento en el array con **rows[2]**. Pero también es *posible que no sepas cuántos elementos hay* en un array cuando queremos el último.

Podemos hacer uso de la propiedad `".length"` de un array, esto devuelve el numero de elementos en el array.
Para conseguir el ultimo elemento de cualquier array se puede utilizar esta sintaxis:

`array[array.length - 1]`

`array.length` devuelve el numero de elementos en un *array*.
Al sustraer 1 se consigue el index del ultimo elemento en el array.
Puedes aplicar el mismo concepto para el *array* llamado **rows**.

Actualicemos **rows[2]** para acceder dinamicamente la último elemento en el **array rows**.

`rows[rows.length - 1]; -> prints last element of the array`

#

Anteriormente aprendimos todo sobre como funcionan los *arrays*, vamos a tomarnos un momento para revisar lo que aprendimos.

Empecemos declarando una variable llamada **cities** e **iniciandola** con un *array* que contiene los *strings* **"London", "New York",** y **"Mumbai"**

Despues de **loggearlo**, cambiar el último elemento de **cities** al *string* **"Mexico City"**, y luego volver a loggear **cities**.

Al hacerlo correctamente deberíamos ver este resultado en la consola: 

`[ "London", "New York", "Mumbai" ]`\
`[ "London", "New York", "Mexico City" ]`

>`let cities = ["London", "New York", "Mumbai"];`\
`console.log(cities)`\
`cities = ["London", "New York", "Mexico City"]`\
`console.log(cities)`

#

Ahora estamos listos para avanzar a la próxima lección de arrays.

Un método en JavaScript es una función que está asociada con ciertos valores u objetos. Un ejemplo que ya nos encontramos es el método `.log`, que es parte del objeto `console`.

Los arrays tienen sus propios métodos, y el primero que vamos a explorar es el método `.push()`, que este nos deja "empujar" un valor al final del array.
Este es un ejemplo de **agregar** `.push()`, `empujar`, el número 12 al **final del array**.

`array.push(12);`

Utilicemos el método `.push()` para agregar el *string* *"freeCodeCamp"* al final de mi array **rows**.

Agregamos este código antes del `console.log` para que podamos ver los cambios que se le hacen al array.

`let rows = ["Naomi", "Quincy", "CamperChan"];`\
`rows.push("freeCodeCamp");`\
`console.log(rows);`

Otro método escencial para este proyecto es el método `.pop()`, que remueve el último elemento de un *array* y devuelve ese elemento.

Cuando un método devuelve un valor, podemos pensarlo básicamente que nos devuelven el valor, haciendo posible su uso en otra parte del código.

Crear una variable llamada **"popped"** y asignar el valor de `rows.pop()`, luego loggear **"popped"** a la consola.

`let popped = rows.pop();`

Deberías de haber visto "freeCodeCamp" impreso en la consola. Esto se debe a que el método `.pop()` devuelve el valor que fue removido del array y anteriormente habiamos `pusheado` **"freeCodeCamp"** al final del array.

Pero, ¿qué es lo que devuelve `.push()`? 
Asignemos el valor de `rows.push()` a una nueva **variable** y hagamosle un `console.log(pushed)`.

¿Estabas esperando ver un 4 en la consola? `.push()` devuelve el nuevo valor del array, despues de agregar el valor que le das.

Es importante estar alerta de que valores devuelve un método. Tomate un tiempo para experimentar con `.push()` y `.pop()`.
Cuando estés listo remueve todos los `.push()` y `.pop()` y tu método `console.log()`.

Cambiemos la declaración de **rows** para asignarle un array vacio.

Tambien, cambiemos el *string* 'Hello' para hacer que utilice doble comillas otra vez.
Generalmente la elección de comillas no importa, pero es preferible que seas consistente en tu elección durante tu proyecto.

`let character = "Hello";`\
`let count = 8;`\
`let rows = [];`

Declarar una variable con la palabra clave *let* nos habilita a poder reasignarla.
Esto significa que podemos cambiar la variable **character** más tarde a otro valor.

Para este proyecto, no queremos cambiar los valores de esas variables. Entonces, en lugar de utilizar *let*, deberiamos utiliar *const* para declararlas. Las variables *const* son especiales.

<span style="color: red;">Primero, una variable **const** no puede ser reasignada como una variable **let**. Esto podría arrojar un error:</span>

`const firstName = "Naomi";`\
`firstName = "Jessica";`

<span style="color: red;">Una variable **const** tampoco puede estar **no inicializada**, este código arrojará error.</span>

`const firstName;`

#

Ahora estamos listos para empezar a crear nuestro generador de piramides. La variable **character** va a servir como el bloque de la piramide.

*"Hello"* no va a funcionar bien para eso, cambiemos el valor de **character** para que sea el carácter hash **"#"**.

`const character = "#";`\
`const count = 8;`\
`const rows = [];`

Para generar una piramide, vas a necesitar crear muchas líneas.
Cuando necesitamos realizar una tarea repetidamente hasta que una condición es cumplida, vamos a usar un *loop*.

Hay varias maneras de escribir un *loop*.

Vamos a iniciar un *for loop* básico, *for loops* utiliza el siguiente sintaxis:

`for (iterator; condition; iteration) {`\
`logic;`\
`}`

En los próximos pasos, vamos a explorar cada componente de un loop en detalle.
Por ahora vamos a construir un *for loop* que incluye los terminos **"iterator", "condition" e "iteration"** para los tres componentes. Mantengamos el *loop body*, la sección con {}, vacío.

`for (iterator; condition ; iteration) {`

`}`

Nuestro loop va a necesitar un iterador correcto. El iterador es una variable que podemos declarar especificamente en nuestro *for loop* para controlar como el loop itera o atraviesa la logica.