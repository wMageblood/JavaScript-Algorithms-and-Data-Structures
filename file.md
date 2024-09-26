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
```
const character = "#";
const count = 8;
const rows = [];
```
Para generar una piramide, vas a necesitar crear muchas líneas.
Cuando necesitamos realizar una tarea repetidamente hasta que una condición es cumplida, vamos a usar un *loop*.

Hay varias maneras de escribir un *loop*.

Vamos a iniciar un *for loop* básico, *for loops* utiliza el siguiente sintaxis:
```
for (iterator; condition; iteration) {
    logic;
}
```
En los próximos pasos, vamos a explorar cada componente de un loop en detalle.
Por ahora vamos a construir un *for loop* que incluye los terminos **"iterator", "condition" e "iteration"** para los tres componentes. Mantengamos el *loop body*, la sección con {}, vacío.
```
for ("iterator"; "condition" ; "iteration") {

}
```
Nuesto loop va a necesitar un iterador adecuado. El *iterador* es una variable que puedes declarar especificamente en tu *for loop* para controlar como el *loop* itera o atraviesa tu lógica.

Es una convencion común utilizar "i" como la variable iteradora en un loop.

Esto se puede declarar dentro de los parentesis de un *for loop*. Por ejemplo, este es un *for loop* declarado con una variable **index** y le asigna el valor 100.
```
for (let index = 100; "second"; "third") {

}
```
Reemplazar el *string* "iterator" con una declaración *let* para la variable "i", asignarle un valor de 0 para empezar. Esto le va a dar un valor de 0 a la variable "i" la primera vez que tu código corra.
```
for (let i = 0; "condition"; "iteration") {

}
```
La condición de un *"for loop"* le dice al *loop* cuantas veces va a iterar, cuando la **condición** se convierte en falsa, el loop para.

En JavaScript, un **boolean** puede ser **verdadero** o **falso**.
Estos **no son strings**, vamos a aprender mas sobre ellos, luego.

Por ahora, vamos a utilizar el operador ***less than* / *menor (<)***.

Esto nos dejará evaluar si el **valor de la izquierda es menor que le valor de la derecha**. Por ejemplo, `count < 3` se evaluaría `true` si `count` es `2` y `false` si `count` es `4`.

Remplazar nuestra string `"condition"` dentro del `for loop` para evaluar si `i` es menor que `count`.
```
for (let i = 0; i < count; "iteration") {

}
```
La declaración de la iteración le va a decir a tu loop que hacer con el iterador en cada vuelta.

Cuando *reasignamos una variable*, podemos **usar la variable para referenciar el valor anterior** antes de que sea reasignado.
Esto te deja hacer cosas como agregar tres a un numero existente.

Por ejemplo, `bees = bees + 3;` incrementaría el valor de `bees` por tres.

Utilizar esa sintaxis para reemplazar el string `"iteration"` con una declaración de reasignación que incrementa el valor de `i` por uno.

```
const character = "#";
const count = 8;
const rows = [];

for (let i = 0; i < count; i + 1) {

}
```

El loop va a correr 8 veces. Dentro del cuerpo del loop, imprimamos el valor del iterador `i` para ver que es lo que sucede.

`for (let i = 0; i < count; i = i + 1) {`\
    `console.log(i);`\
`}`

Vamos a ver el número de 0 a 7 impreso en la consola, uno por linea.
Esto va a servir para la fundación de la pirámide.

Remplacemos el `console.log(i)` para `.push(i)` a nuestro **rows** array.

Desafortunadamente no podemos ver que es lo que está haciendo el loop ahora.

Utilicemos *let* para declarar una variable `result` y asignemosle un *string* vacío.
Un *string* vacío es representado con comillas sin nada entre ellas, como por ejemplo `""`.

Ahora, agregamos un `console.log` imprimiendo el valor de `result`. Dependiendo en qué consola utilices, puede ser que no veas nada.

`console.log(result);`

Para manipular el string `result`, vamos a necesitar usar un tipo de *loop* distinto.

Especialmente un ***for...of*** loop, que itera sobre cada objeto en un objeto iterable y temporalmente lo asigna a una variable.

El sintaxis de un ***for...of*** loop se ve asi:

```
for (const value of iterable) {

}
```

Notemos que si se puede utilizar **const** porque la variable solamente existe por una sola iteración, no durante todo el loop.

Creemos un `for...of loop` para iterar a través de tu array **rows**, asignando el valor a una variable llamada **row**.

Recordemos que en el anterior loop utilizamos el operador de suma `"+"` para incrementar el valor de `i` por `1`.

Podemos hacer algo similar con un *string* añadiendo un nuevo string a un string existente. Por ejemplo, `hello = hello + " World";` agregaría el string " World" al string guardado dentro de la variable `hello`, esto se llama *concanetación*

En nuestro `for...of loop`, utiliza el operador de suma para concatenar el valor de `row` al valor de `result`.

```
let result = ""

for (const row of rows) {
  result = result + row;
}
```
Ahora, todos los números están apareciendo en la misma línea. Pero esto no va a funcionar para crear una pirámide.

Vamos a tener que agregar bajar una línea nueva a cada fila.
Aunque al apretar `enter` en nuestro teclado va a crear una línea nueva, esto en JavaScript va a resultar en un error.

En este caso vamos a tener que usar un tipo especial de `escape sequence` `\n`, que es interpretada como una nueva linea cuando el `string` es loggeado. Por ejemplo:

`lineOne = lineOne + "\n" + lineTwo;`

Utilicemos un segundo operador de suma para concatenar una nueva línea entre el `result` existente y el valor de `row` agregado.
```
for (const row of rows) {
  result = result + "\n" + row;
}
```

Imprimir numeros no va a resultar en una pirámide linda, ahora que nos está devolviendo el contenido de nuestro array **rows** formateado, es tiempo de actualizar nuestro loop original.

En lugar de empujar `i` al array, empujemos el valor de nuestra variable `character`.

```
for (let i = 0; i < count; i = i + 1) {
  rows.push(character);
}
```

Ahora que tenemos una serie de caracteres `#`, pero todavía falta la ofrma de nuestra pirámide. Afortunadamente la variable `i` representa el número de nuestra `row` actual. Esto nos habilita a usarla para crear nuesta estructura piramidal.

Para lograr esto, vamos a tener que usar el método `.repeat()` el cual está disponible para `strings`. Este método acepta un número como argumento, especificando el numero de veces para repetir el `string` que quermeos.
Por ejemplo, utilicemos `.repeat()` para generar el string `"Code! Code! Code!"`
```
const activity = "Code! ";
activity.repeat(3);
```

En este punto estamos encontrando lo que es conocido como *off-by-one-error*, un problema frecuente que se encuentran en lenguajes que contienen ***zero-based indexing*** como JavaScript.

El primer index de nuestro array `rows` es `0`, por lo que es mejor empezar nuestro `for loop` con `i = 0`. Pero repetir nuestro loop cero veces resulta en nada que imprimir.

Para arreglar esto, agregamos `1` al valor de `i` en nuestro método `.repeat()`, tal cual como hicimos en nuestras condiciones de loop.

La logica para para formatear la piramide probablemente se ponga complicada, esto significa que es un buen momento para extraer ese codigo a una funcion.
```
function name(parameter) {

}
```

La palabra clave `function` le dice a JavaScript que la variable `name` va a ser una función. `parameter` es una variable que representa el valor que es pasado a la función cuando es utilizada.

La funcion puede tener muchos o pocos `parameters` como gustes. Como por ejemplo en un `for loop`, el espacio entre los *curly braces* es el cuerpo de la función.

Declaremos una función llamada `padRow`, no le agreguemos ningún parametro todavía, el cuerpo de la funcion debe de estar vacío, recordemos también la convención *CamelCase*.

Para que sea una función, necesitamos llamarla.
Un llamado a la función le dice a tu aplicacion que corra el código de la función donde tu quieras llamarla.

La sintaxis de una llamada de función es el nombre de la función seguida de parentésis, por ejemplo, el siguiente código define y llama a la función `test`.
```
function test() {

}
test();
```
Ahora, llamemos nuestra funcion `padRow`.
```
function padRow() {

}
padRow();
```

Estamos llamando nuestra función `padRow`, pero no estamos haciendo nada con ella. Todas las funciones en JavaScript *devuelven* un valor, esto significa que ellas proveen un resultado predefinido cuando las llamas para utilizarlas en cualquier otro lado.

Para ver el resultado de nuestro *calleo* a la función `padRow`, declaremos una variable llamada `call` y asignemos la llamada existente de `padRow` a esa variable.
```
const call = padRow();
padRow(call);
```

Ahora agreguemos un `console.log` para imprimir el valor de nuestra variable `call`.
```
function padRow() {

}
const call = padRow();
console.log(call);
```
Nuestra variable `call` tiene un valor `undefined`, incluso habiendola definido. Esto se debe a que nuestra función `padRow` actualmente no devuelve ningun valor. Por predefinido, las funciones devuelven `undefined` como su valor.

Para devolver otra cosa, vas a necesitar utilizar la palabra clave `return`, aca hay un ejemplo de una funcion que devuelve el `string`: `"Functions are cool!"`
```
function demo() {
  return "Functions are cool!";
}
```

Utilicemos la palabra clave `return` para que tu función devuelva el `string` `"Hello!"`.
```
function padRow() {
    return "Hello!;
}
```

Cuando tenemos un valor que esta explicitamente escrito en tu código, como el `string` `"Hello!"` en tu función, es considerado que está *hard-codeada*.

*Hard-Codear* un valor dentro de tu función puede hacer que no sea tan reutilizable como nos gustaría.

En su lugar, podemos definir parametros para la función. Parametros son variables especiales que se les da un valor cuando llamas a la función, y pueden ser utilizados en tu función para dinámicamente cambiar el resultado de la código de la función.

Para agregar parametros a tu funcion, necesitas agregar el nombre de una variable dentro de los parentesis, por ejemplo: la función `demo` tiene un parametro llamado `name`:
```
function demo(name) {

}
```

`name` suena a un parametro útil, entonces vamos a agregarlo a nuestra función `padRow`.
```
function padRow(name) {
  return "Hello!";
}
```

Una función no tiene que devolver un valor que esté hard-codeado, puede devolver un valor que esté guardado en una variable. Los parametros son variables especiales para una función, que también pueden ser `returned`.

Cambiemos nuestra funcion `padRow` para que haga `return` de directamente el parametro `name`.
```
function padRow(name) {
  return name;
}
```

Si abrimos la consola otra vez, vamos a ver que nuestra funcion `padRow` está devolviendo `undefined`, incluso habiendo puesto una variable de `return`, esto se debe a que los parametros necesitan recibir un valor cuando llamas a la función.

Cuando pasamos el valor a un calleo de funcion, el valor es referido como un `argument`, este es un ejemplo de llamar a la funcion `demo` y pasarle `"Naomi"` como el argumento para el parametro `name`.
```
function demo(name) {
  return name;
}
demo("Naomi");
```

Ahora, pasemos mi nombre como el argumento del parametro `name` en la call de `padRow`, recuerda que tu nombre es un `string`, asique vas a necesitar utilizar comillas.

`const call = padRow("Enzo");`

#

Antes de seguir adelante, vamos a tomarnos un momento para ver como se comportan las funciones.

Declaremos una funcion llamada `addTwoNumbers`, esta funcion debe de tomar dos argumentos y `return` la `sum` de esos dos argumentos.

Tu función no debe de tener valores hard-codeados, un ejemplo de valores hard-codeados es este:
```
function sayName(firstName, lastName) {
  return "John Doe";
}

sayName("Camper", "Cat");
```

Esta función va a devolver el valor "John Doe" independientemente de los argumentos pasados a los parametros `firstName` y `lastName`, entonces `"John Doe"` es considerado un valor hard-codeado.

Declaremos la variable `sum` y asignemosle el valor de llamar la funcion `addTwoNumbers` con `5` y `10` como los argumentos.
Posteriormente `console.log(sum)` al finalizar.
```
function addTwoNumbers(firstValue, secondValue) {
    return firstValue + secondValue;
}

const sum = addTwoNumbers(5, 10);
console.log(sum);
```

Las variables en JavaScript tienen un *alcance especifico*, en otras palabras, cuando una variable es declarada, determina en qué parte de tu código se puede utilizar.

El primer tipo de *scope* es el global, variables que son declaradas fuera de cualquier "bloque" como en una función o un for loop, estan en el *global scope*.

Nuestras variables `character`, `count` y `rows` estan todas en el ***global scope***.

Cuando una variable está en el ***global scope***, una función puede acceder a ella.

Este es un ejemplo de una función que utiliza una variable global llamada `title`.
```
const title = "Professor ";
function demo(name) {
  return title + name;
}
demo("Naomi")
```

Este ejemplo devolverá el valor `"Professor Naomi"`, actualicemos nuestra funcion `padRow` para que devuelva el valor de la concanetacion de la variable `character` al principio del parametro `name`.

```
function padRow(name) {
  return character + name;
}
```

Las variables tambien pueden ser declaradas dentro de una funcion. Estas variables estan consideradas entro de un ***local scope*** o un ***block scope***.

Una variable declarada dentro de una funcion solamente puede ser utilizada en esa funcion. Si tratamos de acceder a ella desde fuera de la funcion, vamos a tener un error de referencia.

Para ver esto en accion, utilicemos `const` para declarar una variable `test` en tu funcion `padRow`. Inicieemosla con el valor `"Testing"`

Luego, debajo de tu funcion, trata de `console.log(test)`, vas a ver un error porque no esta definida fuera del scope local.

Los valores devueltos por una funcion se utilizan llamando a la funcion. Se puede utilizar la llamada a la funcion directamente como el valor que devuelve o capturar el valor devuelto en una variable. De esta manera puede utilizar el valor asignado a una variable de ambito local, fuera de la funcion en la que se creo.
```
function getName() {
  const name = "Camper cat";
  return name;
}

console.log(getName()); // "Camper cat"

const capturedReturnValue = getName();
console.log(capturedReturnValue); // "Camper cat"

console.log(name); // reference error
```

Para utilizar nuestro valor `"Testing"`, y devolverlo a nuestra funcion `padRow` tenemos que updatear nuestra declaracion `return` para que solamente nos devuelva la variable `test`.
```
function padRow(name) {
  const test = "Testing";  
  return test;
}
```

Debajo de la declaracion `return`, `console.log("This Works!")`.

Despues de hacer eso, no vas a ver el string `"This Works!"`, en la consola, y el `console.log("This works!")` esta con color gris.

Copiemos el `console.log()` y peguemoslo en la parte de arriba del `return`, ahora el string `"This Works!"` deberia de aparecer en la consola.

Una cosa importante para saber sobre la palabra clave `return` es que no solamente define un valor que puede ser devuelto de tu funcion, tambien ***para la ejecucion de tu codigo dentro de una funcion o de una declaracion en bloque***, esto significa que cualquier codigo despues del `return` no va a funcionar.
```
function padRow(name) {
  const test = "Testing";
  
  return test;

}
```