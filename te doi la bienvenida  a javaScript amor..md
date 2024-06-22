JavaScript es el lenguaje que hace que una página web sea interactiva. Una página web tiene tres partes principales:

1. **Capa estructural (HTML):** Esta es la base de la página, como los cimientos de una casa. Define la estructura y el contenido, como los textos, las imágenes y los botones.
2. **Capa presentacional (CSS):** Esta es la apariencia de la página, como la pintura y la decoración de una casa. Define los colores, las fuentes, y el diseño.
3. **Capa interactiva (JavaScript):** Esta es la parte que hace que la página responda a las acciones del usuario, como cuando haces clic en un botón y algo cambia en la página.

JavaScript permite a los desarrolladores (las personas que crean páginas web) cambiar la estructura (HTML) y la apariencia (CSS) de la página en respuesta a lo que hace el usuario. Por ejemplo, pueden agregar o quitar elementos, o cambiar el estilo de la página cuando alguien hace clic en un botón.

JavaScript también permite controlar muchas otras cosas del comportamiento de una página web y del navegador (el programa que usas para visitar páginas web).

En el curso, se enseñan los conceptos básicos de JavaScript, desde cómo escribirlo correctamente hasta cómo usar las herramientas que ofrece.

<img src="https://i.pinimg.com/564x/b7/33/1a/b7331a41f11dca573f3d005fde773f98.jpg" alt="Descripción de la imagen" class="centered-image">


-----

# **Introducción a JavaScript**

Aunque su nombre sugiere lo contrario, JavaScript no está realmente relacionado con Java. Solo comparten algunas similitudes en cómo se escriben. Al principio, JavaScript se inspiró un poco en Java.

**Historia:**

- JavaScript se llamó originalmente "LiveScript".
- Fue introducido en 1995 en una versión de prueba del navegador Netscape Navigator.
- Microsoft creó su propia versión de JavaScript llamada "JScript" para Internet Explorer 3.0.

**Estandarización:**

- Netscape llevó JavaScript a una organización llamada Ecma International para que creara un estándar que todos los navegadores pudieran seguir.
- En 1997, Ecma International lanzó el estándar ECMA-262, que describe cómo debe funcionar JavaScript. Este estándar se llama ECMAScript.

**Versiones de ECMAScript:**

- **ES5:** La versión 5 del estándar ECMAScript, lanzada en 2009. Es una de las versiones más importantes.
- **ES6 (o ES2015):** La versión 6 del estándar, lanzada en 2015, introdujo muchas mejoras. Después de ES6, se lanza una nueva versión del estándar cada año, como ES2016, ES2017, etc.

---

# Declaraciones

Una **declaración** en JavaScript es una instrucción que dice al navegador que haga algo. Por ejemplo, esta declaración asigna el valor 4 a una variable llamada `myVariable`:

javascript

```js
let myVariable = 4; myVariable; // Resultado: 4`
```


Las instrucciones suelen terminar con un punto y coma (`;`), aunque no siempre es obligatorio. Si falta un punto y coma, JavaScript intenta añadirlo automáticamente, pero es mejor ponerlo siempre para evitar errores.

# Sentencias de Bloque

Una **sentencia de bloque** agrupa varias declaraciones entre llaves (`{}`). Esto es útil para usar varias instrucciones donde JavaScript solo espera una. Por ejemplo, en una instrucción `if`:

javascript

```js
if (x === 2) {   // Algunas acciones }`
``` 

# Expresiones

Una **expresión** es un trozo de código que produce un valor. Por ejemplo, `2 + 2` es una expresión que produce el valor 4:

javascript

```js
2 + 2; // Resultado: 4
```

Los paréntesis pueden agrupar partes de una expresión para asegurar que se evalúen juntas:

javascript

```js
(2 + 2) * 4; // Resultado: 16
```


# Escritura Débil

JavaScript tiene **escritura débil**, lo que significa que no es necesario especificar el tipo de dato. Puede convertir tipos automáticamente (coerción de tipos). Por ejemplo:

javascript

```js
"1" + 1; // Resultado: "11"
```


También puedes convertir tipos manualmente:

javascript

```js
let myVariable = 100; myVariable = myVariable.toString(); // myVariable ahora es "100"
```

# Distinción entre Mayúsculas y Minúsculas

JavaScript distingue entre mayúsculas y minúsculas. Esto significa que `myVariable` y `myvariable` son diferentes:

javascript

```js
const myVariable = 2; myvariable; // Error: myvariable no está definida myVariable; // Resultado: 2
```


# Espacio en Blanco

JavaScript no es sensible a los espacios en blanco. Esto significa que el intérprete ignora la cantidad y el tipo de espacio en blanco usado, ya sean pestañas o espacios.

javascript

```js
console.log("Log this"); 
console.log("Log this too"); // Resultado:  
// "Log this." 
// "Log this too."
```

Sin embargo, la presencia de espacios en blanco puede ser importante para separar partes del código (tokens léxicos):

javascript

```js
let x; // Correcto: [tokens: [let] [x] ] letx; // Error: letx no está definido [tokens: [letx] ]
```

Cuando se usa espacio en blanco para separar estos tokens, el intérprete ignora la cantidad de espacio en blanco usado:

javascript

```js
let x = 2; // [tokens: [let] [x] [=] [2] ]
```


Lo mismo ocurre con los saltos de línea. A veces, los saltos de línea pueden causar problemas si una instrucción se termina prematuramente:

javascript

```js
let x = 2; // [tokens: [let] [x] [=] [2] ]
```


## Estilo de Código

Algunos tipos de declaraciones suelen ocupar una sola línea:

javascript

```js
let x = 1; 
let y = 2;
```


Otras declaraciones suelen ocupar varias líneas para mejorar la legibilidad:

javascript

```js
if (x == 2) {   // Algunas acciones }
```


Estas convenciones son solo para facilitar la lectura. JavaScript interpretará el código de la misma manera:

javascript

```js
let x=1;
let y=2;  

if(x==2){
}
```


## Optimización

Es común en la preparación de JavaScript para producción eliminar los espacios en blanco no esenciales para reducir el tamaño del archivo. Este proceso se llama minificación.

## Convenciones de Espacio en Blanco

El uso de espacio en blanco depende de las preferencias del autor y del mantenimiento del código. En proyectos con varios desarrolladores, se suelen sugerir o aplicar ciertas convenciones para garantizar un formato de código coherente. Por ejemplo, usar tabulaciones o espacios para indentar declaraciones anidadas:

javascript

```js
let myVariable = 10;  
if (typeof myVariable === "number") {                   console.log("This variable is a number.");
if (myVariable > 5) {         
  console.log("This variable is greater than five.");        } 
}  // Resultado: 
// "This variable is a number." 
// "This variable is greater than five."
```
-----

**¡Hola amor!

Quiero felicitarte por llegar al tema de "Tipos y Estructuras de Datos" en tu aprendizaje de JavaScript. Sé cuánto has trabajado y lo mucho que te estás esforzando, y me llena de orgullo ver tu progreso.

Entender los tipos de datos primitivos y cómo funcionan es un gran paso y sé que lo vas a dominar rápidamente. Sigue así, cada día estás más cerca de convertirte en una experta en programación. ¡Estoy aquí para apoyarte en cada paso del camino!

¡Felicidades, mi amor! ¡Sigue brillando!**

----

# Tipos y Estructuras de Datos

## Primitivas

Las **primitivas** son los tipos de datos más simples en JavaScript. Un literal primitivo es un valor simple que no tiene propiedades ni métodos propios. Las primitivas son **inmutables**, lo que significa que no se pueden cambiar.

Por ejemplo, el valor de una variable llamada `theTruth` se puede cambiar de `true` a `false`, pero el literal booleano `true` siempre será `true` y no puede representar otro valor. Lo mismo ocurre con los números: el literal `5` siempre será `5` y no puede representar otro número.

## Tipos Primitivos de Datos

Existen siete tipos primitivos de datos en JavaScript:

1. **Números**: Representan valores numéricos, por ejemplo, `5`, `3.14`.
2. **Cadenas**: Representan texto, por ejemplo, `"hola"`, `"JavaScript"`.
3. **Booleanos**: Representan valores verdaderos o falsos, `true` o `false`.
4. **null**: Representa la ausencia intencional de un valor.
5. **undefined**: Representa una variable que ha sido declarada pero no tiene un valor asignado.
6. **BigInt**: Representa números enteros grandes que están más allá del límite de los números normales.
7. **Símbolo**: Representa un valor único y estático, principalmente usado para identificadores únicos.
---
# Números

## Valor Numérico

Un valor numérico se compone de cualquier serie de caracteres numéricos. Por ejemplo: `5`.

El tipo de datos numéricos también incluye propiedades globales especiales como `Infinity` y `NaN` ("Not a Number"). `NaN` aparece al intentar realizar cálculos con valores no numéricos.

## El Objeto Number

Cuando se pasa un valor a la función `Number()`, ese valor se convierte en su equivalente numérico. Por ejemplo, una cadena de texto numérica se convierte en un número:

javascript

```js
Number("10"); // Resultado: 10
```


Si pasas `false` o `null` a `Number()`, se convierte en `0`, y `true` se convierte en `1`:

javascript

```js
Number(null); // Resultado: 0  
Number(false); // Resultado: 0  
Number(true); // Resultado: 1
```

Si el valor no se puede convertir, como `undefined` o una cadena con caracteres no numéricos, `Number` muestra `NaN`:

javascript

```js
Number(undefined); // Resultado: NaN  
Number("The number 3."); // Resultado: NaN
```


### Objeto Number como Constructor

Usar `Number` como constructor no es común ni recomendable porque crea un objeto Number en lugar de un literal numérico:

javascript

```js
let numObject = new Number(15); 
numObject;
// Resultado: Number { 15 }  
let tenObject = new Number(10); tenObject + 5; 
// Resultado: 15  tenObject === 10; 
// Resultado: false
```


## Números de Punto Flotante y Enteros

JavaScript tiene un solo tipo de número: números de punto flotante de doble precisión de 64 bits. Esto puede causar errores de precisión:

javascript

```js
0.1 + 0.7; // Resultado: 0.7999999999999999
```


Para evitar errores de precisión, se recomienda usar enteros siempre que sea posible.

## Operadores Numéricos

JavaScript sigue el orden matemático estándar para operaciones: paréntesis, exponentes, multiplicación, división, suma y resta.

| Operador | Nombre         | Uso  | Resultado |
| -------- | -------------- | ---- | --------- |
| `+`      | Adición        | 2+2  | 4         |
| `-`      | Resta          | 4-2  | 2         |
| `*`      | Multiplicación | 2*5  | 10        |
| `/`      | División       | 10/5 | 2         |
| `++`     | Incremento     | 2++  | 3         |
| `--`     | Decremento     | 3--  | 2         |
| `**`     | Exponente      | 2**4 | 16        |
| `%`      | Resto          | 12%5 | 2         |

### Operadores de Asignación Matemática

Se pueden usar para realizar una operación matemática y asignar el resultado a una variable:

| Operador | Nombre                       | Uso             |
| -------- | ---------------------------- | --------------- |
| `+=`     | Asignación de adición        | `myValue += 2`  |
| `-=`     | Asignación de resta          | `myValue -= 2`  |
| `*=`     | Asignación de multiplicación | `myValue *= 2`  |
| `/=`     | Asignación de división       | `myValue /= 2`  |
| `**=`    | Asignación de exponencial    | `myValue **= 2` |
| `%=`     | Asignación del resto         | `myValue %= 2`  |

## Valores Simbólicos

La primitiva de número incluye `NaN` (No es un número) y `Infinity` (positivo o negativo):

javascript

```js
10 / 0; 
// Resultado: Infinity  Infinity; 
// Resultado: Infinity  infinity; 
// Error: ReferenceError: infinity is not defined
```


### NaN

`NaN` aparece cuando el resultado de una operación no puede expresarse como un número:

javascript

```js
"2" * 2; // Resultado: 4  
"two" * 2; // Resultado: NaN
```



Ejemplos comunes de `NaN`:

- Conversiones fallidas (`parseInt(undefined)`)
- Operaciones aritméticas inválidas (`0 / 0`, `Math.sqrt(-10)`)
- Operaciones con `NaN` (`NaN + 2`)

------
# Cadenas

## Primitivas de String

Cualquier conjunto de caracteres entre comillas dobles (`"`), comillas simples (`'`), o acentos graves (``) es una primitiva de string. Ejemplos:

javascript

```js
console.log("Hello, World."); 
// Resultado: Hello, World.  
console.log('Hello, World.'); 
// Resultado: Hello, World.  
console.log(`Hello, World.`); 
// Resultado: Hello, World.
```

### Literales de String y Caracteres Especiales

Las comillas dentro de una string pueden complicar su uso:

javascript

```js
console.log("I'm a string."); 
// Resultado: I'm a string.  
console.log('"A string," I said.'); 
// Resultado: "A string," I said.
```


Si necesitas usar el mismo carácter de cierre dentro de la string, debes escaparlo con una barra inversa (`\`):

javascript

```js
console.log('"I\'m a string," I said.'); 
// Resultado: "I'm a string," I said.
```

## Objeto String

Cuando se llama como función, `String()` convierte un valor en un literal de string:

javascript

```js
let myString = String(10); 
console.log(myString); 
// Resultado: "10"  
typeof myString; 
// Resultado: string
```


### Uso del Objeto String

Usar el objeto `String` como constructor no es común debido a que crea un objeto con métodos adicionales, no solo el valor literal:

javascript

```js
let stringObj = new String("My new string."); console.log(typeof stringObj); 
// Resultado: object
console.log(stringObj); 
// Resultado: String { "My new string." }
```


## Concatenación

El operador `+` se usa para concatenar strings:

javascript

```js
console.log("My" + " string."); 
// Resultado: My string.
```


## Literales de Plantilla

Los literales de plantilla permiten interpolación y múltiples líneas:

javascript

```js
const myString = `This is a string.`;  console.log(myString); 
// Resultado: This is a string.
```

### Interpolación en Literales de Plantilla

Puedes insertar expresiones dentro de un literal de plantilla usando `${}`:

javascript

```js
console.log(`The result is ${2 + 4}.`); 
// Resultado: The result is 6.
```
### Plantillas Etiquetadas

Se pueden usar funciones personalizadas con literales de plantilla, recibiendo un array con la cadena dividida y los marcadores de posición como argumentos:

javascript

```js
const myNoun = "template literal";  
function myTagFunction(myStrings, myPlaceholder) {      const myInitialString = myStrings[0];     console.log(`${myInitialString}modified ${myPlaceholder}.`); 
}  
myTagFunction`I'm a ${myNoun}.`; 
// Resultado: I'm a modified template literal.
```

# Booleano

## Primitiva Booleana

El tipo de dato booleano representa valores lógicos con dos estados: `true` (verdadero) y `false` (falso).

## Objeto Booleano

El objeto `Boolean` se usa para forzar valores a un estado booleano explícito:

javascript

```js
Boolean( "A string literal" ); // Resultado: true
```



### Valores que se Evalúan como `false`

Algunos valores se evalúan como `false` al ser convertidos a booleanos:

javascript

```js
Boolean( NaN ); 
// Resultado: false  
Boolean( 0 ); 
// Resultado: false  
Boolean( "" ); 
// cadena vacía 
// Resultado: false  
Boolean( null ); 
// Resultado: false  
Boolean( undefined ); 
// Resultado: false  
Boolean( false ); 
// Resultado: false
```

### Todos los Otros Valores

Cualquier otro valor se evalúa como `true`:

javascript

```js
Boolean( 5 ); 
// Resultado: true  
Boolean( "false" ); 
// la cadena "false" es una string, por lo tanto, es implícitamente true. 
// Resultado: true
```


### Uso del Objeto Boolean

Evita usar el constructor `Boolean` para crear objetos booleanos. En su lugar, usa las primitivas booleanas:

javascript

```js
const falsePrimitive = Boolean( 0 ); 
const falseObject = new Boolean( 0 );  
console.log( falsePrimitive ); 
// Resultado: false  
console.log( falseObject ); 
// Resultado: Boolean { false }  
falseObject.valueOf(); 
// Resultado: false
```


Debido a que todos los objetos son considerados verdaderos, incluso si contienen un valor falso, se evaluarán como verdaderos en contextos booleanos:

javascript

```js
const falsePrimitive = Boolean( 0 ); 
const falseObject = new Boolean( 0 );  
console.log( falsePrimitive == true ); 
// Resultado: false  
console.log( falseObject == true ); 
// Resultado: true
```


# Nulo e Indefinido

## null

La palabra clave `null` representa la ausencia intencional de cualquier valor. Aunque `null` es una primitiva, el operador `typeof` muestra incorrectamente que `null` es un objeto. Este comportamiento erróneo se ha mantenido desde las primeras versiones de JavaScript para evitar interrumpir el comportamiento existente en la web.

javascript


```js
typeof null // Resultado: "object"
```

Puedes asignar `null` a una variable para indicar explícitamente que no tiene ningún valor asignado actualmente o para borrar un valor previamente asignado.

javascript

```js
let myVar = null;
```

## undefined

`undefined` es un valor que se asigna automáticamente a variables que se han declarado pero no inicializado, o a funciones que no tienen una declaración `return`.

javascript

```js
let myVar; console.log(myVar); 
// Resultado: undefined  
function myFunction() {
}
console.log(myFunction()); 
// Resultado: undefined
```



## Comparación entre null y undefined

Aunque `null` y `undefined` tienen superposiciones funcionales, tienen propósitos diferentes. `null` representa la ausencia intencional de valor, mientras que `undefined` indica la falta de un valor asignado.

javascript

```js
null == undefined 
// Resultado: true  null === undefined 
// Resultado: false
```


El operador de igualdad flexible (`==`) hace coerción de tipo, permitiendo que `null` y `undefined` sean considerados iguales. En contraste, el operador de igualdad estricta (`===`) verifica la igualdad sin coerción de tipo, por lo que `null` y `undefined` no son estrictamente iguales.

## Propiedad undefined

A diferencia de `null`, `undefined` es una propiedad del objeto global en JavaScript. Esta decisión de diseño inicial permitió a los navegadores heredados sobrescribir el valor de `undefined` por completo. En navegadores modernos, es posible declarar `undefined` como una variable local dentro de una función, pero esto es generalmente desaconsejado debido a posibles confusiones y comportamientos inesperados.


# BigInt

## Introducción a BigInt

Los primitivos BigInt son una adición relativamente nueva a JavaScript que permite operaciones matemáticas con números fuera del rango manejable por el tipo `Number`. Para crear un BigInt, simplemente agrega una `n` al final de un literal numérico o pasa un valor entero numérico o una cadena a la función `BigInt()`.

javascript

```js
const myNumber = 9999999999999999; 
const myBigInt = 9999999999999999n;  
typeof myNumber; 
// Resultado: "number"  
typeof myBigInt; 
// Resultado: "bigint"  
myNumber; 
// Resultado: 10000000000000000  
myBigInt; 
// Resultado: 9999999999999999n
```


En el ejemplo anterior, `9999999999999999` está fuera del rango seguro de dígitos que puede representar `Number`, lo que causa un error de redondeo.

## Limitaciones y Uso de BigInt

Los valores de BigInt no heredan los métodos ni propiedades del objeto `Number`, y no se pueden utilizar con los métodos proporcionados por el objeto integrado `Math` de JavaScript. Es crucial destacar que no se pueden mezclar primitivos `BigInt` y `Number` en operaciones aritméticas estándar:

javascript

```js
9999999999999999n + 5; 
// Resultado: Uncaught TypeError: can't convert BigInt to number
```


Para realizar operaciones aritméticas con BigInt, ambos operandos deben ser valores de BigInt:

javascript

```js
console.log( 9999999999999999 + 10 );  
// Off by one 
// Resultado: 10000000000000010  
console.log( 9999999999999999n + 10n ); 
// Resultado: 10000000000000009n
```


# Símbolo

## Introducción a Símbolo

Los símbolos son una primitiva relativamente nueva introducida en ES6. Un símbolo representa un valor único que nunca es igual a ningún otro valor, incluidos otros símbolos.

javascript

```js
Symbol() === Symbol(); // Resultado: false
```


A diferencia de otros tipos primitivos como las strings o los números, dos símbolos con la misma descripción no son iguales.

## Creación de Símbolos

Puedes crear símbolos utilizando la función `Symbol()`. Puedes opcionalmente pasar una descripción que es útil para depuración pero no afecta la unicidad del símbolo:

javascript

```js
let mySymbol = Symbol("My symbol description");  
typeof mySymbol; // Resultado: "symbol"  
mySymbol.description; 
// Resultado: "My symbol description"
```


Intentar crear un símbolo con `new Symbol()` resultará en un error, ya que `Symbol` no es un constructor:

javascript

```js
let mySymbol = new Symbol(); 
// Resultado: Uncaught TypeError: Symbol is not a constructor
```


## Uso de Símbolos

Los símbolos se utilizan comúnmente como claves únicas en objetos para evitar colisiones con otras propiedades:

javascript

```js
const mySymbol = Symbol("Description"); 
const myObject = {};  
myObject[mySymbol] = "Value";
```



## Símbolos Compartidos

JavaScript también proporciona símbolos compartidos a través de un registro global con `Symbol.for()`. Esto permite recuperar un símbolo existente o crear uno nuevo si no existe:

javascript

```js
let sharedSymbol = Symbol.for("My key");  
sharedSymbol === Symbol.for("My key"); 
// Resultado: true
```


## Símbolos Conocidos

JavaScript define una serie de símbolos conocidos como propiedades estáticas en el objeto `Symbol`. Estos símbolos proporcionan acceso a métodos y comportamientos internos de JavaScript:

javascript

```js
Symbol.iterator; 
// Accede al símbolo de iterador 
Symbol.match;    
// Accede al símbolo de coincidencia
```



Los símbolos conocidos son identificados con un prefijo `@@` o `%` para distinguirlos de las propiedades normales.


# Variables

## Introducción a las Variables

Las variables en JavaScript son estructuras que asignan un nombre representativo a un valor. Pueden contener datos de cualquier tipo y se identifican por nombres denominados identificadores. Es importante seguir reglas específicas al nombrar variables para evitar errores de sintaxis y mantener la legibilidad del código.

## Reglas para Identificadores

Los identificadores válidos en JavaScript:

- Pueden contener letras Unicode, signos de dólar ($), guiones bajos (_), dígitos (0-9) y algunos caracteres Unicode.
- No pueden contener espacios en blanco, ya que estos separan elementos en el código.
- Deben comenzar con una letra, guion bajo (_) o signo de dólar ($); no pueden empezar con dígitos.

javascript

```js
let 1a = true; // Incorrecto
```


## Convenciones de Nomenclatura

Es recomendable seguir convenciones de nomenclatura que mejoren la legibilidad del código. Por ejemplo, utilizar camelCase (inicial en minúscula, mayúsculas en las primeras letras de palabras subsiguientes) para identificadores compuestos.

javascript

```js
let camelCasedIdentifier = true;
```

## Declaración de Variables

Existen tres palabras clave para declarar variables en JavaScript:

- `let`: Declara una variable que puede cambiar su valor.
- `const`: Declara una constante cuyo valor no puede cambiar después de inicializarse.
- `var`: Declara una variable con un alcance más amplio que `let` y `const`, aunque tiene comportamientos menos intuitivos.

javascript

```js
let myVariable = 5; 
const myConstant = true; 
var functionScopedVariable = "scope";
```


## Alcance de las Variables

El alcance de una variable determina dónde en el código puede ser utilizada.

- **Alcance de Bloque**: Variables declaradas con `let` o `const` están limitadas al bloque que las contiene.

javascript
```js
{let scopedVariable = true;     console.log(scopedVariable); 
 // Accesible aquí 
 } 
 console.log(scopedVariable);
  // Error, fuera de alcance
```


- **Alcance de Función**: Variables declaradas con `var` tienen alcance dentro de la función que las contiene.

javascript

```js
function myFunction() {     
var functionScopedVariable = "scope";     console.log(functionScopedVariable); 
// Accesible aquí 
} 
console.log(functionScopedVariable); 
// Error, fuera de alcance
```


- **Alcance Global**: Variables declaradas fuera de cualquier bloque o función tienen alcance global, accesible en toda la aplicación.

javascript

```js
var globalVariable = "global scope"; console.log(globalVariable); 
// Accesible en cualquier lugar
```


## Consideraciones Adicionales

- **Elevación (Hoisting)**: Las declaraciones de variables en JavaScript son "elevadas" al principio de su alcance, pero solo la declaración, no la inicialización.

javascript

```js
console.log(hoistedVariable); // undefined 
var hoistedVariable = 5; 
console.log(hoistedVariable); // 5
```


- **Temporal Dead Zone (TDZ)**: Las variables declaradas con `let` y `const` no están disponibles hasta después de la declaración.

javascript

```js
{ console.log(blockScopedVariable); 
 // Error     
 let blockScopedVariable = true; 
 }
```


Estas prácticas y convenciones ayudan a mantener un código claro y eficiente, facilitando la colaboración y el mantenimiento del proyecto.

----------

¡Hola mi amor!

Hoy quiero celebrar lo especial que eres para mí con un mensaje muy único y geek, justo como a ti te gusta. Eres como esos operadores en JavaScript que hacen que todo en mi vida tenga sentido y funcione perfectamente.

Eres mi `===` porque contigo todo encaja perfectamente, sin necesidad de comparaciones adicionales. Eres mi `!==` porque contigo no hay desigualdades ni dudas. Eres mi `>` porque superas todas mis expectativas y me haces crecer cada día más. Eres mi `<` porque me dejas sin palabras con tu ternura y amor.

Nuestro amor es como un bucle `for`, siempre encontrando nuevas formas de crecer y fortalecerse juntos. Como un bucle `while`, nunca nos detenemos en nuestro camino hacia un futuro brillante. Y como un `switch`, eliges cada día estar a mi lado, haciendo que cada momento sea especial.

Gracias por llenar mi vida de alegría, amor y aventuras. ¡Eres la constante en mi vida que nunca cambiaría!

Te amo más allá de las líneas de código y hasta el infinito y más allá. 💖


# Operadores, Comparaciones y Flujo



