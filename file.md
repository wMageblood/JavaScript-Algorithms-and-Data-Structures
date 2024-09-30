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
  console.log("This Works!");
  return test;

  console.log("This Works!"); // este no funciona
}
```

#

Ahora, nuestra variable `call` tiene el valor de `"Testing"`, pero la funcion ya no esta utilizando el parametro `name`.

Remover el parametro `name` de la declaracion de la funcion, luego remueve el string `"CamperChan"` del calleo de `padRow`

Tambien removamos los dos `console.logs()` de la funcion `padRow`.
```
function padRow() {
  const test = "Testing";
  return test;
}
const call = padRow();
console.log(call);
```

Debido a que mi funcion ya no utiliza un parametro, cambiar el argumento no la afecto.

Vamos a remover la declaracion de `test` y la declaracion de `return` de nuestra funcion `padRow`, para que la funcion este vacia nuevamente.
```
function padRow() {

}
const call = padRow();
console.log(call);
```

Como lo esperabamos, la funcion devuelve `undefined` otra vez. Nuestra variable `call` ya no es necesaria, entonces removamos la declaracion de `call` y el `console.log(call)`.
```
function padRow() {

}
```

Para formatear una linea, nuestra funcion `padRow` va a necesitar saber en que linea estamos, y cuantas lineas en total vamos a generar.

La mejor forma de hacer esto es creando parametros para ellos.

Vamos a darle a nuestra funcion `padRow`, dos parametros, `rowNumber` y un `rowCount`
```
function padRow(rowNumber, rowCount) {

}
```

Recordemos que en un paso anterior, aprendimos sobre los valores de retorno. Una funcion puede devolver un valor para que la aplicacion lo consuma por separado.

En una funcion, la palabra clave `return` es utilizada para especificar un valor de retorno.

Por ejemplo, esta funcion devolvera el valor dado al primer parametro.

Utilicemos la palabra clave `return` para devolver el valor de la variable `character.repeat(rowNumber);`.
```
function padRow(rowNumber, rowCount) {
  return character.repeat(rowNumber);
}
```

Una *llamada de funcion* nos deja utilizar la funcion.

Tal vez no te diste cuenta, pero metodos como `.push()` que estuvimos utilizando fueron llamadas de funciones.

Una funcion es llamada referenciando el nombre de la funcion, agregando `()`.

Asi es como se llama una funcion de `test`

`test();`

Reemplacemos el `character.repeat(i + 1)` en nuestra llamada `.push()` con una llamada de la funcion `padRow`.
```
for (let i = 0; i < count; i = i + 1) {
  rows.push(padRow())
}
```

Nuestra funcion `padRow` tiene dos parametros que definimos.

Valores son proporcionados a una llamada de funcion como *argumentos*, y nosotros *pasamos* argumentos a esas llamdas de funciones.

Aca hay una funcion, con el valor `"Hello"` pasada al parametro de la funcion.

`test ("Hello");`

Pasemos `i + 1` y `count` como argumentos para nuestra llamada de `padRow`, como parametros, los argumentos son separados por una coma.
```
for (let i = 0; i < count; i = i + 1) {
  rows.push(padRow(i + 1, count))
}
```

Deberiamos de ver la misma cantidad de caracteres en la consola. Nuestra funcion `padRow` esta haciendo exactamente lo mismo que hacia antes, pero ahora con una seccion reutilizable.

Utilizando el operador de suma para concatenar un solo espacio `" "` al principio y al final de nuestro `character` string.

Recordemos que podemos utilizar el operador `"+"` para concatenar strings, como por ejemplo

`" " + "string"`
```
function padRow(rowNumber, rowCount) {
  return " " + character.repeat(rowNumber) + " ";
}
```
Ahora, es el momento de un poco de matematica, consideremos una piramode de tres lineas.

Si la queremos centrada, se va a ver asi 
```
··#··
·###·
#####
```

Los espacios vacios fueron reemplazados por puntos medios, para que sea mas facil de leer. 
Si extrapolamos el patron, podemos ver que los espacios al principio y al final siguen un patron.

Actualicemos nuestro espacio en blanco para que sean repetidos `rowCount - rowNumber` cantidad de veces.

Abramos la consola para ver los resultados.
```
function padRow(rowNumber, rowCount) {
  return " ".repeat(rowCount - rowNumber) + character.repeat(rowNumber) + " ".repeat(rowCount - rowNumber);
}
```
Podemos pasar expresiones completas como argumentos. La funcion va a recibir el resultado de la evaluacion de esa expresion. Por ejemplo estas dos funciones te entregan el mismo resultado:
```
test(2 * 3 + 1);
test(7);
```

Viendo el patron nuevamente: 
```
··#··
·###·
#####
```
Actualicemos el valor de `character` para que se repita `2 * rowNumber - 1` cantidad de veces.

Abramos la consola nuevamente para ver ocmo queda el resultado actualizado.
```
function padRow(rowNumber, rowCount) {
  return " ".repeat(rowCount - rowNumber) + character.repeat(2 * rowNumber - 1) + " ".repeat(rowCount - rowNumber);
}
```

Tu piramide ahora funciona como esperado. Pero esta es una excelente oportunidad para explorar el codigo que hemos escrito.

El operador de adicion no es la unica forma de agregar valores a una variable.

El operador de adicion puede ser utilizado para significar "tomar el valor original de la varialbe, agregar este valor y asignarlo otra vez a la variable"

Por ejemplo, estas dos declaraciones resultarian iguales.

```
test = test + 1;
test +=;
```

Actualicemos nuestro declaracion de iteracion en nuestro `for loop` para que use `addition assignment`.
```
for (let i = 0; i < count; i += 1);{

}
```

Porque solamente estamos incrementando `i` por `i` podemos utilizar el `operador de incremento "++"` Este operador incrementa el valor de la variable por 1, actualizando la asignacion a esa variable.

Por ejemplo `test` devolvera `8`:
```
test = 7;
test++;
```
Reemplacemos nuestra asignacion de suma con el `increment operator` para nuestro loop.
```
for (let i = 0; i < count; i++) {}
```
En lugar de pasarle `i + 1` a mi llamada de `padRow`, vamos a empezar con un loop en `1`. Esto nos va a dejar crear un loop de 1 index.

Actualicemos nuestro iterador para que empiece en `1` en lugar de `0`.
```
for (let i = 1; i < count; i++) {
  rows.push(padRow(i + 1, count));
}
```

La piramide se ve un poco chistosa ahora. Porquie estamos empezando el loop en `1` en lugar de `0`, pero no necesitamos agregarle `1` a `i` cuando lo pasamos a `padRow`

Actualicemos nuestro primer argumento en  la llamada de `padRow` para que sea `i`.
```
for (let i = 1; i < count; i++) {
  rows.push(padRow(i + 1, count));
}
```

Desafortunadamente, el piso de nuestra piramide desaparecio. Esto se debe a que creamos otro `off-by-one error`.

El loop original fue por los valores de `i` del `0` al `7`, porque `count` es `8`, y nuestra condicion requiere que `i` sea menor que `count`. Nuestro loop esta corriendo los valores de `i` del `1` al `7`

Nuestro loop tiene que ser actualizado cuando tambien `i = 8`.

Mirando tu logica, esto significa que tu loop va a correr cuando `i` *sea menor* o *igual a* `count`. Podemos utilizar el ***menor o igual que `<=`***

Actualicemos nuestra condicion de loop para que corra cuando `i` ***es menor o igual que*** `count`
```
for (let i = 1; i <= count; i++) {
  rows.push(padRow(i, count));
}
```

Los comentarios pueden ayudarte a explicar poque tu codigo toma cierto rumbo, o incluso te ayuda a dejarte notas para el futuro.

En JavaScript podemos utilizar `//` para dejar un comentario de una sola linea.

Agreguemos un comentario de una sola linea arriba de tu funcion para recordarte como cambiar el codigo a una clase diferente de loop.
```
// gotta change type of loop
for (let i = 1; i <= count; i++) {
  rows.push(padRow(i, count));
}
```

Tambien podemos hacer comentarios multi-linea. Empiezan con `/*` y terminan con `*/`

Utilicemos esto para comentar el codigo.
```
/* for (let i = 1; i <= count; i++) {
  rows.push(padRow(i, count));
} */
```

La piramide desaparecio otra vez. Pero no me tengo que preocupar, ya que esto era esperado.

Antes de que creemos un nuevo loop, vamos a tener que aprender sobre los `if`. Una declaracion `if` nos ayuda a correr un bloque de codigo solamente cuando la condicion se encuentra.

Se utiliza el siguiente sintaxis:
```
if (condition) {
  logic
}
```

Creemos una declaracion `if` con el `boolean` `true` como la condicion. En el cuerpo imprimamos `"Condition is true"`.
```
if (true) {
  console.log("Condition is true");
}
```

Vamos a ver el string impreso en la consola, porque `true`, verdaderamente es `true`.

Cambiemos la condicion de nuestro `if` al `boolean` `false`.
```
if (false) {
  console.log("Condition is true");
}
```
Ahora el string no se ve, porque `false` no es `true`. Pero que hay sobre los otros valores?

Tratemos de cambiar la condicion al `string` `"false"`.

El texto aparecio nuevamente! Esto se debe a que `"false"` es un **string**, que cuando es evaluado con un `boolean` se torna `true`. Esto significa que `"false"` es un valor verdadero.

Un *valor verdadero* significa que un valor es considerado verdadero cuando es evaluado como boolean.

La mayoria de los valores que nos encontremos en JavaScript van a ser verdaderos.

Un *falsy value* es lo opuesto, un valor considerado falso cuando es evaluado como un boolean. JavaScript tiene una lista definida de *falsy values*, algunos de ellos incluyen `false`, `0`, `""`, `null`, `undefined` y `NaN`.

Tratemos de cambiar nuestra condicion `if` a que sea un ***empty string `""`*** el cual es un *falsy value*.
```
if ("") {
  console.log("Condition is true");
}
```

El texto desaparecio nuevamente!

Los strings vacios se evaluan como `false`, haciendolos un `falsy value`. Vamos a aprender mas sobre los valores verdaderos y falsos en los futuros proyectos.

En adicion a las declaraciones `if`, JavaScript tambien tiene declaraciones `else if`.

Declaraciones `else if` te dejan comparar multiples condiciones con un solo bloque de codigo.

Este es un sintaxis para una declaracion `else if`.
```
if (condition1) {
  // code to run if condition1 is true
} else if (condition2) {
  // code to run if condition2 is true
} else if (condition3) {
  // code to run if condition3 is true
} 
```

La primera condicion es `false`, JavaScript va a comparar la proxima condicion en la cadena.

Si la segunda condicion es `false` JavaScript va a comparar la tercera condicion, y asi sucesivamente.

Debajo de nuestra declaracion `if` agreguemos una declaracion `else if` que compara si `5` es menor a `10`.

Dentro del cuerpo de la declaracion `else if`, `console.log("5 is less than 10")`;.
```
if (condition) {
} else if (5 < 10) {
  console.log("5 is less than 10")
}
```
A veces vamos a querer un codigo diferente cuando todas las condiciones de `if...else if` son `false`. Podemos hacer esto agregando un `else` block.

Un block `else` solamente va a evaluar las condiciones cuando las condiciones en el `if` y en el `else if` no son encontradas.

Aca, el `else` block es agregado al `else if` block.
```
if (condition) {
  // this code will run if condition is true
} else if (condition2) {
  // this code will run if the first condition is false
} else {
  // this code will run 
  // if the first and second conditions are false
}
```

Agreguemos un `else block` al `else if block`.

Dentro del `else block` loggeemos `console.log("This is the else block")`.

Para ver los resultados en la consola, manualmente cambiemos el `<` en el `else if` a `>`. Esto va a hacer la condicion `false` y el `else block` va a ejecutarse.
```
if ("") {
  console.log("Condition is true");
} else if (5 < 10) {
  console.log("5 is less than 10");
} else {
  console.log("This is the else block);
}
```

Ahora que estuvimos trabajando con declaraciones `if...else` podemos removerlo del codigo.

Una vez completado, utiliza `let` para declarar una variable llamada `continueLoop` y asignarle el boolean `false`. Luego utilicemos `let` para declarar una variable llamada `done` y asignemosle el valor de `0`.
```
let continueLoop = false;
let done = 0;
```
Un `while loop` va a correr una y otra vez hasta que la condicion especifica ya no sea `true` y tiene la siguiente sintaxis:
```
while (condition) {
  logic;
}
```

Utilicemos esa sintaxis para declarar un loop `while` con `continueLoop` como la condicion.
El Cuerpo deberia estar vacio.
```
while (continueLoop) {

}
```

Ahora mismo, si cambiamos `continueLoop` a verdadero, tu `while` loop va a correr para siempre. Esto es llamado un `infinite loop`, y deberias de ser cuidadoso de evitar estos. Un loop infinito puede bloquear tu sistema, requiriendo un `full restart` para escaparlo.

Para evitar esto, empecemos utilizando el operador de incremento para incrementar la variable `done` dentro de nuestro loop.
```
while (continueLoop) {
  done++;
}
```
El operador de ecualidad `==` es utilizado para comparar si dos valores son iguales.
Para comprar dos valores utilizariamos una declaracion como esta `value == 8`

Debajo de `done++` dentro de tu codigo, agrega una declaracion `if`. La declaracion debera de comparar si `done` es igual a `count` utilizando el `equality operator`.
```
while (continueLoop) {
  done++;
  if (done == count) {
  }
}
```

El `equality operator` puede llegar a tener un comportamiento extraño en JavaScript, por ejemplo `"0" == 0` es `true`, aunque uno es un string y el otro es un numero.

El `strict equality operator "==="` es utilizado para comprar si dos valores son iguales y si comparten el mismo tipo de dato.

Como una regla general, este es el tipo de `equality operator` que deberias utilizar siempre. Con el `strict equality operator` `"0" === 0` es `false` debido a que tienen el mismo valor pero no comparten el mismo tipo de dato.

Actualicemos nuestra condicion `done == count` para que use el `strict equality operator`.
```
if (done === count) {
}
```

Cuando `done` llegó al valor de `count`, queremos que el loop no se ejecute más.

Dentro del cuerpo de tu `if` asignemos el boolean `false` a nuestra variable `continueLoop`.
```
  if (done === count) {
    continueLoop = false
  }
```

Para hacer que se genere otra vez la piramide, `.push()` el resultado de callear `padRow` con `done` y `count` como los argumentos de tu array `rows`, similar a lo que hicimos en el primer loop.
```
rows.push(padRow(done, count))
```

El `strict inequality operator "!=="` te deja comparar si dos valores son ***no iguales, o no tienen el mismo tipo***, la sintaxis es similar al `equality operator: value !== 4`

Actualiza la condicion de tu `while loop` para comparar si `done` no es igual a `count`.
```
while (done !== count) {
  done !== count;
  rows.push(padRow(done, count));
  if (done === count) {
    continueLoop = false;
  } 
}
```

Ahora que movimos la comparacion a la condicion del `while`, podemos remover totalmente la declaracion `if`.
```
while (done !== count) {
  done++;
  rows.push(padRow(done, count));
}
```

Nuestro loop ya no depende en la variable `continueLoop`, esto hace que la variable sea una `unused declaration`. Generalmente queremos evitar declaraciones no utiliadas para prevenir confusion en el futuro.

Removamos la variable `continueLoop`.

Nuestro generador de piramides todavia funciona, aunque es posible que termine con un loop infinito nuevamente.

Porque solamente estamos chequeando si `done` `!== ( no es igual )` a `count`, si `done` fuera mas *grande* que `count`, nuestro loop correria para siempre.

Actualicemos nuestra condicion de loop para comparar si `done` es menor o igual a `count`.
```
let done = 0;

while (done <= count) {
  done++;
  rows.push(padRow(done, count));
}
```

Utilizando `done` para trackea el numbero de filas que fueron generadas es funcional, pero podemos limpiar un poco mas la logica.

Los arrays tienen una propiedad especial llamada `length`, que nos deja ver cuantos valores o elementos hay en el array.

Accederiamos a esta propiedad utiliando la sintaxis `myArray.length`.

Notemos que `rows.length` en la llamada de `padRow` nos dara `off-by-one-error`, porque `done` es incrementado **antes** de la llamada.

Actualicemos nuestra condicion para comparar si `rows.length` es menor a `count`.
```
let done = 0;

while (rows.length < count) {
  done++;
  rows.push(padRow(done, count));
}
```

Reemplacemos la referencia de `done` en la llamada de tu `padRow` con `rows.length + 1`.
```
let done = 0;

while (rows.length + 1 < count) {
  done++;
  rows.push(padRow(rows.length + 1, count));
}
```

Ahora nuestra funcion ya no va a necesitar la variable `done`, removamos el operador de incremento de nuestro loop, y la declaracion de variable para `done`.
```
while (rows.length < count) {
  rows.push(padRow(rows.length + 1, count));
}
```

Ahora es un loop muy funcional, utiliando comentarios multi-linea comentemos nuestro `while loop`.

Que pasaria si tu piramide este de abajo a arriba? o invertida?

Empecemos creando un nuevo `for loop`. Declaremos nuestro iterador `i` asignemosle el valor de `count`, luego utilicemos un boolean `false` para nuestra declaracion de iteracion y condicion.
```
for (let i = count; false; false) {

}
```

Ya que estamos utilizando el loop en la direccion opuesta, vamos a necesitar que nuestro codigo corra cunado `i` es mayor a `0`. Podemos utilizar el operador `greater than ">" `

Pongamos la condicion de nuestro loop para que corra cuando `i` es mayor a `0`.
```
for (let i = count; i > 0; false) {

}
```
Nuestra declaracion de iteracion tambien se va a ver afectada. En lugar de agregar `1` a `i` en cada loop, vamos a tener que `restar 1`.

Como hicimos antes con `i = i + 1`, actualicemos nuestra declaracion de iteracion y demosle el valor de `i` para que se reste `1` a si mismo.
```
for (let i = count; i > 0; i = i - 1) {

}
```

Ahora, pusheemos el valor de llamar `padRow` con nuestras variables `i` y `count` a nuestro  array `rows`.
```
for (let i = count; i > 0; i = i - 1) {
  rows.push(padRow(i, count))
}
```

Justo como en la suma, hay diferentes tipos de operadores que podemos utilizar para sustraer numeros. El `substraction assignment operator "-="` sustrae el valor dado de la varaiable actual, luego asigna el resultado a la variable.

Reemplacemos la declaracion de iteracion con el tipo correcto de declaracion utilizando la `subtraction assignment operator`.
```
for (let i = count; i > 0; i -= 1) {
  rows.push(padRow(i, count));
}
```

Porque solamente estamos sustrayendo uno de `i`, podemos utilizar el `decrement operator` `"--"`

Reemplacemos nuestra asignacion de resta con el `decrement operator`.
```
for (let i = count; i > 0; i--) {
  rows.push(padRow(i, count));
}
```
Nosotros podemos crear la piramide invertida sin la necesidad de tener un **"loop invertido"**.

Para hacer esto, vamos a tener que aprender un par de metodos de arrays nuevos.

Empecemos utilizando `const` para declarar una variable llamada `numbers`. Asignemosla a un array con los elementos `1`, `2` y `3`. Luego `console.log(numbers)`.
```
const numbers = [1, 2, 3];
console.log(numbers)
```

El metodo de un array `.unshift()`, nos deja agregar un valor al principio del array, al contrario de `.push()` que nos deja agregar un valor al final del array. `.unshift()` devuelve la nueva longitud del array en el que fue llamado.
```
const countDown = [2, 1, 0];
const newLength = countDown.unshift(3);
console.log(countDown); // [3, 2, 1, 0]
console.log(newLength); // 4
```

Utilicemos `const` para declarar una variable llamada `unshifted`, asignemosle el valor de llamar `.unshift()` en nuestro array `numbers`, pasemosle `5` como el argumento.

Luego `console.log(unshifted)`.
```
const numbers = [1, 2, 3];
const unshifted = numbers.unshift(5)
console.log(unshifted)
console.log(numbers);
```

Los arrays tambien tienen el metodo `.shift()`, esto remueve el **primer elemento** de un array, al contrario de `pop()` que remueve el ultimo elemento.

Este es un ejemplo del metodo `.shift()`.
```
const numbers = [1, 2, 3];
numbers.shift();
```
El array `numbers` va a ser `[2, 3]`.

Directamente debajo de nuestro array `numbers`, declaremos una variable llamada `shifted` y asignemosle el valor del resultado de llamar `.shift()` el el array `numbers`. En la proxima linea, hagamos `console.log(shifted)`.
```
const numbers = [1, 2, 3];
const shifted = numbers.shift(numbers)
console.log(numbers)
const unshifted = numbers.unshift(5);
console.log(unshifted);
console.log(numbers);
```
Ahora que probamos estos metodos, podemos hacerle otro acercamiento a la piramide invertida. Pero primero vamos a tener que limpiar la experimentacion.

Removamos el array `numbers`, los `methods` y los `console.logs`.

A veces vamos a querer traer de regreso parte de codigo que habiamos comentado. Podemos hacerlo removiendo el `/*` y el `*/` alrededor de ese codigo. Esto se llama `uncommenting`.

`Uncomment` solamente nuestro primer `for loop`.
```
// TODO: use a different type of loop
for (let i = 1; i <= count; i++) {
  rows.push(padRow(i, count));
}

/*while (rows.length < count) {
  rows.push(padRow(rows.length + 1, count));
}*/

/*for (let i = count; i > 0; i--) {
  rows.push(padRow(i, count));
}*/
```

Nuestra piramide ya no se encuentra invertida, esto es porque agregamos nuevas filaes al **final** de nuestro array.

Actualicemos el cuerpo de nuestro loop y agreguemos nuevas filas al principio y al final del array.
```
for (let i = 1; i <= count; i++) {
  rows.unshift(padRow(i, count));
}
```

Y qué si tuvieramos una forma alternar entre una piramide hacia abajo o hacia arriba?

Empecemos declarando una variable `inverted`, y asignemoslé el valor de `true`. No estamos cambiando esta variable en nuestro código, pero vamos a tener que utilizar `let` para nuestras pruebas puedan cambiarla más tarde.
```
let inverted = true;
```

Utilicemos una declaracion de `if` para checar si `inverted` es `true`. Recordemos que no tenemos que utilizar un `equality operator` acá.
```
for (let i = 1; i <= count; i++) {
  if (inverted == true) { //Remember that you dont need to use equality operator
  rows.unshift(padRow(i, count))
  }
}

for (let i = 1; i <= count; i++) {
  if (inverted) { //not using equality operator
  rows.unshift(padRow(i, count));
  }
}
```

Ahora movamos nuestro metodo `.unshift()` a nuestro bloque `if`.
```
for (let i = 1; i <= count; i++) {
  if (inverted) {
  rows.unshift(padRow(i, count));
  }
}
```

Si nuestra piramide no esta invertida, entonces vamos a tener que utilizar un bloque `else` que arregla la piramide a un orden normal.

En los pasos anteriores, aprendimos a como trabajar con declaraciones `else`.
```
if (condition) {
  // if condition is true, run this code
} else {
  // if condition is false, run this code
}
```

Agreguemos un `else` a nuestro bloque `if`.
```
for (let i = 1; i <= count; i++) {
  if (inverted) {
    rows.unshift(padRow(i, count));
  } else {

  }
}
```

Cuando `inverted` es false, vamos a querer construir una piramide normal.

Utilicemos `.push()` como lo utilizamos antes, para lograr el resultado.
```
for (let i = 1; i <= count; i++) {
  if (inverted) {
    rows.unshift(padRow(i, count));
  } else {
    rows.push(padRow(i, count));
  }
}
```

El generador de piramodes ahora esta terminado, con mas funcionalidad de la que habiamos planeado anteriormente.

En el proximo paso es limpiar nuestro codigo, removamos todos los comentarios, tanto singulares como de multi-linea de nuestro codigo.

Ahora, experimentemos con diferentes valores para nuestras variables `character`, `count`, e `inverted`.

Cuando estamos listos para avanzara al proximo projecto, setteemos `character` a `"!"`, `count` a `10` e `inverted` a `false` para continuar.
