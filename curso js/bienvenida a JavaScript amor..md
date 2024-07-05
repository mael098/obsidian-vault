![[Pasted image 20240623103058.png]]
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


# Operadores de Comparación

Los operadores de comparación comparan los valores de dos operandos y evalúan si la declaración que forman es `true` o `false`. En el siguiente ejemplo, se usa el operador de igualdad estricta (`===`) para comparar dos operandos: la expresión `2 + 2` y el valor `4`. Debido a que el resultado de la expresión y el valor numérico `4` son iguales, esta expresión se evalúa como `true`:
```js
2 + 2 === 4 // true
```

## Coerción y igualdad de tipos

Dos de los operadores de comparación más usados son `==` para la igualdad baja y `===` para la igualdad estricta. `==` realiza una comparación general entre dos valores mediante la coerción de los operandos para que coincidan con los tipos de datos, si es posible. Por ejemplo, `2 == "2"` muestra `true`, aunque la comparación se realice entre un valor numérico y un valor de string:

javascript
```js
2 == 2 // true  
2 == "2" // true
```



Lo mismo sucede con `!=`, que muestra `true` solo si los operandos que se comparan no son iguales de manera general:

javascript

```js
2 != 3 // true  
2 != "2" // false
```



Las comparaciones estrictas con `===` o `!==` no realizan la coerción de tipos. Para que una comparación estricta evalúe como `true`, los valores que se comparen deben tener el mismo tipo de datos. Por este motivo, `2 == "2"` muestra `true`, pero `2 === "2"` muestra `false`:

javascript

```js
2 === 3 // false  
2 === "2" // false
```



Para evitar ambigüedades causadas por la coerción automática, es recomendable utilizar `===` siempre que sea posible.

## Operadores de Comparación

|Operador|Descripción|Ejemplo|Resultado|
|---|---|---|---|
|`===`|Estrictamente igual|`2 === 2`|`true`|
|`!==`|No estrictamente igual|`2 !== "2"`|`true`|
|`==`|Igual (o "inigualable")|`2 == "2"`|`true`|
|`!=`|No igual|`2 != "3"`|`true`|
|`>`|Mayor que|`3 > 2`|`true`|
|`>=`|Mayor o igual que|`2 >= 2`|`true`|
|`<`|Menor que|`2 < 3`|`true`|
|`<=`|Menor o igual que|`2 <= 3`|`true`|

## Valores Verdaderos y Falsos

Todos los valores en JavaScript son `true` o `false` de manera implícita. Algunos valores se fuerzan a `false`:

- `0`
- `null`
- `undefined`
- `NaN`
- Cadena vacía (`""`)

Todos los demás valores se consideran `true`, incluyendo cualquier string que no esté vacía y todos los números que no sean cero.

## Operadores Lógicos

Los operadores lógicos (`&&`, `||`, `!`) se utilizan para controlar el flujo de una secuencia de comandos basado en la evaluación de una o más sentencias condicionales:

javascript

```js
2 === 3 || 5 === 5; 
// true  
2 === 2 && 2 === "2"; 
// false  
2 === 2 && !"My string."; 
// false  
!true; 
// false  
!false; 
// true
```



Usar el operador lógico `!` frente a otro tipo de datos, como un número o una cadena, coerciona ese valor a un valor booleano y revierte el valor verdadero o falso del resultado.

javascript

```js
"string"; 
// "string"  
!"string"; 
// false  
0; 
// 0  
!0; 
// true
```


Es común utilizar dos operadores `!` consecutivos para forzar rápidamente los datos a su valor booleano coincidente:

javascript

```js
!!"string"; 
// true  
!!0; 
// false
```



Los operadores lógicos `&&` y `||` no realizan coerción por sí mismos. Muestran el valor de uno de los dos operandos evaluados, y esa evaluación determina el operando elegido.

javascript

```js
true && false; 
// false  
false || true; 
// true
```



### Operador Coalescente Nulo (`??`)

Presentado en ES2020, el operador coalescente nulo (`??`) muestra el primer operando solo si ese operando tiene algún valor distinto de `null` o `undefined`. De lo contrario, muestra el segundo operando.

javascript

```js
null ?? "My string"; 
// "My string"  
undefined ?? "My string"; 
// "My string"
true ?? "My string"; 
// true
```



El operador `??` es similar a un `||` lógico, pero más estricto en la forma en que evalúa el primer operando. `||` muestra el segundo operando para cualquier expresión que se pueda forzar a `false`, incluidos `undefined` y `null`. `??` muestra el segundo operando cuando el primer operando no es `null` ni `undefined`, incluso si se puede forzar a `false`.

### Operadores Lógicos de Asignación

Los operadores lógicos de asignación (`&&=`, `||=`) permiten asignar condicionalmente un valor a una variable según el valor verdadero o falso de esa variable.

javascript

```js
let myVariable = false; myVariable &&= 2 + 2; 
// false  
myVariable = true; myVariable &&= 2 + 2; 
// 4
```



El valor verdadero o falso del primer operando determina si se realiza una asignación. Sin embargo, cuando se intenta evaluar el primer operando con un operador de comparación, se genera un valor booleano `true` o `false`, al que no se le puede asignar un valor.

javascript

```js
let myVariable = 5; 
myVariable > 2 &&= "My string"; 
// SyntaxError: Invalid left-hand side in assignment
```


javascript

```js
let myVariable = false;
myVariable ||= 2 + 2; 
// 4  
myVariable = true; 
myVariable ||= 2 + 2; 
// true
```



# Flujo de control


El _flujo de control_ es el orden en el que el intérprete de JavaScript ejecuta las declaraciones. Si una secuencia de comandos no incluye declaraciones que alteren su flujo, se ejecuta de principio a fin, una línea a la vez. Las _estructuras de control_ se usan para determinar si un conjunto de declaraciones se ejecuta según un conjunto definido de criterios, si se ejecuta un conjunto de declaraciones repetidamente o si se interrumpe una secuencia de declaraciones.

## Instrucciones condicionales

Las instrucciones condicionales determinan si el código se debe ejecutar en función de una o más condiciones. Una sentencia condicional ejecuta el código que contiene si la condición asociada (o el conjunto de condiciones) se evalúa como `true`. De lo contrario, se omite el código.

### `if`…`else`

Una declaración `if` evalúa una condición dentro de los paréntesis coincidentes que siguen. Si la condición dentro de los paréntesis se evalúa como `true`, se ejecuta la declaración o [declaración de bloque](https://web.dev/learn/javascript/introduction?hl=es-419#block-statements) que sigue a los paréntesis coincidentes:

```js
if ( true ) 
console.log( "True." )
> "True."
 if ( true ) {    
  const myString = "True.";    
  console.log( myString );
 }
> "True."
```

Si la condición dentro de los paréntesis se evalúa como `false`, se ignora la declaración que la sigue:

```js
if ( false ) 
console.log( "True." );
```

Una palabra clave `else` que sigue inmediatamente a una declaración `if` y su declaración ejecutada condicionalmente especifica la declaración que se ejecutará si la condición `if` se evalúa como `false`:

```js
if ( false ) 
console.log( "True." )''
else console.log( "False" );
> "False."
```

Para encadenar varias declaraciones `if`, puedes crear una declaración ejecutada de forma condicional después de `else` otra declaración `if`:

```js
const myCondition = 2;
if ( myCondition === 5 ) console.log( "Five." );
else if ( myCondition === 2 ) console.log( "Two." );
```

Te recomendamos que uses la sintaxis de sentencias de bloque después de los condicionales para mejorar la legibilidad, pero las cláusulas `else if` suelen ser una excepción a esto:

```js
if ( myCondition === 5 ) {    
console.log( "Five." );
} else if ( myCondition === 3 ) {    
console.log( "Three" );
} else {    
console.log( "Neither five nor three." );
}
> "Neither five nor three."
```

#### Operador ternario

`if` ejecuta una sentencia de forma condicional. El operador ternario (más preciso, pero menos común, se llama _operador condicional ternario_) es la abreviatura para ejecutar una expresión de forma condicional. Como su nombre lo indica, el operador ternario es el único operador de JavaScript que usa tres operandos:

- Una condición que se evaluará, seguida de un signo de interrogación (`?`).
- La expresión que se ejecutará si la condición se evalúa como `true`, seguida de dos puntos (`:`).
- La expresión que se ejecutará si la condición se evalúa como `false`.

Esto se usa con frecuencia para establecer o pasar un valor de manera condicional:

```js
const myFirstResult  = true  ? "First value." : "Second value.";
const mySecondResult = false ? "First value." : "Second value.";
myFirstResult;
> "First value."mySecondResult;
> "Second value."
```

### `switch`…`case`

Usa la sentencia `switch` para comparar el valor de una expresión con una lista de valores potenciales definidos con una o más palabras clave `case`. Esta sintaxis es inusual porque proviene de algunas de las primeras decisiones de diseño de JavaScript. La sintaxis `switch`...`case` usa la palabra clave `switch`, seguida de una expresión que se evaluará entre paréntesis y, luego, un par de llaves coincidentes. El cuerpo de `switch` puede contener palabras clave `case`, por lo general, una o más, seguidas de una expresión o un valor y seguidas de dos puntos (`:`).

Cuando el intérprete alcanza un `case` con un valor que coincide con la expresión que se está evaluando entre paréntesis después de la palabra clave `switch`, ejecuta cualquier declaración que siga a esa cláusula `case`:

```js
switch ( 2 + 2 === 4 ) {  
case false:    
 console.log( "False." );
case true:
 console.log( "True." );
}
> "True."
```

Se ejecutan todas las declaraciones que siguen al `case` coincidente, incluso si están incluidas en una [declaración de bloque](https://web.dev/learn/javascript/introduction?hl=es-419#block-statements).

```js
switch ( 2 + 2 === 4 ) {    
 case false: 
 console.log( "False." );  
case true:    
 let myVariable = "True.";
 console.log( myVariable );
}
> "True."
```

Un error de usar `switch…case` es que, después de encontrar una coincidencia, el intérprete de JavaScript ejecuta _cualquier_ declaración que siga a la `case` coincidente, incluso aquellas dentro de otras cláusulas `case`. Esto se llama "falla" al siguiente `case`:

```js
switch ( 2 + 2 === 7 ) {    
case false:    
console.log( "False." );  
case true:    
console.log( "True." );
}
> "False."
> "True."
```

Para evitar la conmutación por error, finaliza cada caso con la palabra clave `break`, que detiene inmediatamente la evaluación del cuerpo `switch`:

```js
switch ( 2 + 2 === 7 ) {    
 case false:    
 console.log( "False." );
break;  
case true:    
 console.log( "True." );
break;
}
> "False."
```

Si ningún `case` coincide con el valor condicional, `switch` selecciona la cláusula `default` si la hay:

```js
switch ( 20 ) {
case 5:
console.log( "The value was five." ); 
break;  
case 10:    
console.log( "The value was ten." ); 
break;  
default:    
console.log( "The value was something unexpected." );
}
> "The value was something unexpected."
```

Sin embargo, la falla también se aplica a `default`, lo que puede generar resultados inesperados. Para solucionar este problema, finaliza tu instrucción `default` con `break` o colócala al final de la lista de casos.

```js
switch ( 20 ) {  
default:    
console.log( "The value was something unexpected." );  case 10:
console.log( "The value was ten." );
break;  
case 5:    
console.log( "The value was five." );    
break;
}
> The value was something unexpected.
> The value was ten.
```

Debido a que las cláusulas `case` no requieren una [declaración de bloque](https://web.dev/learn/javascript/introduction?hl=es-419#block-statements) para agrupar varias declaraciones, las cláusulas `case` y `default` no crean un [alcance léxico](https://web.dev/learn/javascript/data-types/variable?hl=es-419#scope) por sí mismas:

```js
let myVariable;
switch ( true ) { 
case true:  
let myVariable = "True.";  
break; 
default:   
let myVariable = "False."; 
break;
}
> Uncaught SyntaxError: redeclaration of 
let myVariable
```

Para administrar el alcance, usa sentencias de bloque:

```js
let myVariable;
 switch ( true ) {
  case true: {    
  let myVariable = "True.";
 break;  
}  
default: {    
   let myVariable = "False.";
   break;  
  }
}
```

## Iteración y bucles

Los bucles te permiten repetir un conjunto de declaraciones mientras se cumpla una condición o hasta que se cumpla una condición. Usa bucles para ejecutar un conjunto de instrucciones una cantidad fija de veces, hasta que se logre un resultado específico o hasta que el intérprete llegue al final de una estructura de datos iterable (por ejemplo, el elemento final de un array, un mapa o un conjunto, la propiedad final de un objeto o el último carácter de una cadena).

Los bucles interrumpen el flujo "de arriba abajo" de la ejecución de una secuencia de comandos cuando itera sobre un conjunto de declaraciones hasta que se cumplen una o más condiciones, o hasta que ya no se cumplen, según la sintaxis utilizada para crear el bucle. Una vez que finaliza el bucle, la ejecución continúa a las declaraciones que lo siguen. En el siguiente ejemplo, las instrucciones en el cuerpo del bucle se ejecutan tres veces antes de que el intérprete avance:

```js
let iterationCount = 0;
console.log( "Pre-loop." );
while( iterationCount < 3 ) {  
iterationCount++;
console.log( "Loop iteration." );
}
console.log( "Continuing on." );
> "Pre-loop."
> "Loop iteration."
> "Loop iteration."
> "Loop iteration."
> "Continuing on."
```

Si no se pueden cumplir las condiciones durante la ejecución del bucle, este continúa de forma indefinida. Estos _bucles infinitos_ son un error de programación común que puede hacer que el [subproceso de ejecución principal](https://web.dev/learn/javascript/appendix?hl=es-419#main-thread) se pause de forma indefinida o incluso que falle una pestaña del navegador.

El siguiente ejemplo se ejecuta mientras el valor booleano `true` permanezca `true`. Dado que los [valores booleanos son inmutables](https://web.dev/learn/javascript/data-types/boolean?hl=es-419), esto crea un bucle infinito.

**Advertencia:** La ejecución del siguiente código puede ralentizar el navegador o hacer que falle la pestaña actual del navegador.

```js
console.log( "Pre-loop." );
while( true ) {
console.log( "Loop iteration." );
}
> "Pre-loop."
> "Loop iteration."
> "Loop iteration."
> "Loop iteration."
> "Loop iteration."
> "Loop iteration."…
```

Evita dejar bucles infinitos en tu código de producción. Si creas una por error durante el desarrollo, puedes corregirla cerrando la pestaña del navegador en la que se está ejecutando, actualizando el código para que el bucle ya no sea infinito y volviendo a abrir la página.

### `while`

Se crea un bucle `while` con la palabra clave `while` seguida de un par de paréntesis coincidentes que contienen una condición para evaluar. Si la condición especificada se evalúa en un principio como `true`, se ejecuta la instrucción (o la [declaración de bloque](https://web.dev/learn/javascript/introduction?hl=es-419#block-statements)) que sigue a esos paréntesis. De lo contrario, el bucle nunca se ejecuta. Después de cada iteración, la condición se vuelve a evaluar y, si aún es `true`, se repite el bucle.

```js
let iterationCount = 0;
while( iterationCount < 3 ) {
iterationCount++;  
console.log( `Loop ${ iterationCount }.` );
}
> "Loop 1."
> "Loop 2."
```

Si el intérprete encuentra una declaración `continue` en un bucle `while`, detiene esa iteración, vuelve a evaluar la condición y, si es posible, continúa el bucle:

```js
let iterationCount = 0;
while( iterationCount <= 5 ) {  
iterationCount++;  
if( iterationCount === 3 ) {
continue;  
}  
console.log( `Loop ${ iterationCount }.` );
}
console.log( "Loop ended." );
> "Loop 1." 
> "Loop 2."
> "Loop 4."
> "Loop 5."
> "Loop ended."
```

Si el intérprete encuentra una declaración `break` en un bucle `while`, se detiene la iteración y no se vuelve a evaluar la condición, lo que permite que el intérprete continúe:

```js
let iterationCount = 1;
while( iterationCount <= 5 ) {
if( iterationCount === 3 ) {
console.log(`Iteration skipped.``);`break;  
}  
console.log( `Loop ${ iterationCount }.` );
iterationCount++;
}
console.log( "Loop ended." );
> "Loop 1."
> "Loop 2."
> "Iteration skipped.> "Loop ended."
```

Puedes usar `while` para iterar una cantidad específica de veces, como se ve en el ejemplo anterior, pero el caso de uso más común de `while` es un bucle de longitud indeterminada:

```js
let randomize = () => Math.floor( Math.random() * 10 );
let randomNum = randomize();
while( randomNum !== 3 ){
console.log( `The number is not ${ randomNum }.` );
randomNum = randomize();
}
console.log( `The correct number, ${ randomNum }, was found.` );
> "The number is not 0."
> "The number is not 6."
> "The number is not 1."
> "The number is not 8."
> "The correct number, 3, was found."
```

### `do`…`while`

`do`... `while` es una variante del bucle `while` en la que la evaluación condicional ocurre al _final_ de cada iteración del bucle. Esto significa que el cuerpo del bucle siempre se ejecuta al menos una vez.

Para crear un bucle `do`...`while`, usa la palabra clave `do` seguida de la declaración (o la [declaración de bloque](https://web.dev/learn/javascript/introduction?hl=es-419#block-statements)) que se ejecutará en cada iteración del bucle. Inmediatamente después de esa declaración, agrega `while` y los paréntesis que coincidan con la condición que se evaluará. Cuando esta condición ya no se evalúa como `true`, el bucle finaliza.

```js
let iterationCount = 1;
do { 
console.log( `Loop ${ iterationCount }.` );  iterationCount++;} while ( iterationCount < 3 );
>"Loop 1."
>"Loop 2."
> "Loop 3."
```

Al igual que con un bucle `while`, el caso de uso más común para `do`... `while` es un bucle de longitud indeterminada:

```js
let randomNum;
do {  
randomNum = ( () => Math.floor( Math.random() * 10 ) )(); 
console.log( `Is the number ${ randomNum }?` );
} 
while ( randomNum !== 3 );
console.log( `Yes, ${ randomNum } was the correct number.` );
>"Is the number 9?"
>"Is the number 2?"
>"Is the number 8?">
>"Is the number 2?">
>"Is the number 3?">
>"Yes, 3 was the correct number."
```

### `for`

Usa bucles `for` para iterar en una cantidad conocida. En las bases de código heredadas, se usaba con frecuencia para iterar sobre los elementos de un array.

Para crear un bucle `for`, usa la palabra clave `for` seguida de un conjunto de paréntesis que acepte las siguientes tres expresiones en orden y separadas por punto y coma:

1. Una expresión que se evaluará cuando comience el bucle.
2. Una condición que determina si el bucle debe continuar
3. Una expresión que se ejecutará al final de cada bucle

Después de estos paréntesis, agrega la declaración (por lo general, una [declaración de bloque](https://web.dev/learn/javascript/introduction?hl=es-419#block-statements)) que se ejecutará durante el bucle.

```js
for( let i = 0; i < 3; i++ ) {  
console.log( "This loop will run three times.")
}
```

La primera expresión inicializa una variable que actúa como un contador. Esta expresión se evalúa una vez, antes de la primera iteración del bucle. Puedes inicializar esta variable con `let` (o `var`, históricamente) como cualquier otra variable y su alcance es el cuerpo del bucle. Estas variables pueden tener cualquier identificador válido, pero con frecuencia se las llama `i` para "iteración" o "índice". Esto parece contradecir las [prácticas recomendadas establecidas para nombres de identificadores predecibles](https://web.dev/learn/javascript/data-types/variable?hl=es-419), pero la convención está lo suficientemente bien establecida como para ser clara con otros desarrolladores de un vistazo. Debido a que las [colecciones indexadas no se indexan](https://web.dev/learn/javascript/collections/indexed?hl=es-419), estas variables casi siempre tienen un valor inicial de `0`.

Al igual que con otras formas de bucle, la condición es una expresión que determina si el bucle debe ejecutarse. Se usa con mayor frecuencia a fin de establecer un límite superior para el contador de iteraciones. El intérprete evalúa la condición antes de ejecutar el bucle `for` por primera vez.Si la condición no se evalúa en un principio como `true`, el cuerpo del bucle no se ejecuta.

La expresión final se ejecuta al final de cada iteración a través del bucle. Por lo general, se usa para aumentar el identificador en uno.

Por lo general, verás que los bucles `for` iteran a través de arrays en bases de código más antiguas. En estos casos, la condición especificada para que el bucle continúe es un recuento de iteraciones menor o igual que la longitud del arreglo que se itera. La variable que se usa para rastrear el recuento de iteraciones actual se usa con el objetivo de buscar el valor asociado con ese índice en el array, lo que permite que se actúe en orden en cada elemento del array:

```js
var myArray = [ true, false, true ];
for( let i = 0; i <= myArray.length; i++ ) {  console.log( myArray[ i ] );
}
>true
>false
>true
```

Este enfoque dejó de usarse y se reemplazó por enfoques más modernos de bucle a través de [estructuras de datos iterables](https://web.dev/learn/javascript/control-flow?hl=es-419#iterators).

#### `for` [...] `of` [...]

Usa bucles `for`...`of`... para iterar sobre los valores almacenados en una [estructura de datos iterables](https://web.dev/learn/javascript/control-flow?hl=es-419#iterators), como un array, un conjunto o un mapa.

Un bucle `for`...`of`... usa la palabra clave `for` seguida de un conjunto de paréntesis que contiene una variable, seguida de `of` y, luego, la estructura de datos que se itera. La variable puede ser una declaración realizada aquí mediante `let`, `const` o `var`, una variable declarada previamente dentro del alcance actual, una propiedad de objeto o una instancia de [asignación de desestructuración](https://web.dev/learn/javascript/collections/indexed?hl=es-419#destructuring-assignment). Contiene el valor del elemento que corresponde a la iteración actual del bucle.

```js
const myIterable = [ true, false, true ];
for( const myElement of myIterable ) {
console.log( myElement );
}
>true
>false
>true
```

En este ejemplo, el uso de `const` para `myElement` funciona aunque `myElement` recibe un valor nuevo en cada iteración del bucle. Esto se debe a que el alcance de las variables declaradas con `let` o `const` se define en la declaración de bloque dentro del bucle. La variable se inicializa al comienzo de cada iteración y se quita al final.

#### `for`…`in`…

Usa bucles `for`...`in`... para iterar sobre las propiedades que se pueden enumerar de un objeto, incluidas las propiedades heredadas que se pueden enumerar. Al igual que con un bucle `for`...`of`..., un bucle `for`...`in`... usa la palabra clave `for` seguida de un conjunto de paréntesis que contiene una variable que contiene el valor de la clave de propiedad correspondiente a la iteración actual del bucle. Esta variable va seguida de la palabra clave `in` y, luego, el objeto que se itera:

```js
const myObject = { "myProperty" : true, "mySecondProperty" : false };
for( const myKey in myObject ) {  
console.log( myKey );
}
>"myProperty"
>>"mySecondProperty"
```

Una vez más, a pesar de que el valor de `myKey` cambia con cada iteración del bucle, puedes usar `const` sin errores porque la variable se descarta de manera efectiva al final de cada iteración y se vuelve a crear al comienzo.

El valor asociado con cada clave de propiedad no está disponible directamente para la sintaxis `for`...`in`.... Sin embargo, debido a que el bucle tiene acceso a una clave de propiedad en cada iteración, puedes usar esa clave para "buscar" su valor:

```js
const myObject = { "myProperty" : true, "mySecondProperty" : false };
for( const myKey in myObject ) { 
const myValue = myObject[ myKey ];
console.log( `${ myKey } : ${ myValue }` );
}
>"myProperty : true"
>"mySecondProperty : false"
```

Las propiedades heredadas de los constructores integrados no son enumerables, lo que significa que `for`...`in`... no itera a través de propiedades heredadas del constructor `Object`. Sin embargo, sí se incluyen las propiedades que se pueden enumerar dentro de la [cadena del prototipo](https://web.dev/learn/javascript/objects/property-descriptors?hl=es-419) del objeto:

```js
const myPrototype = { "protoProperty" : true };
const myObject = Object.create( myPrototype, {    myProperty: {    value: true,    enumerable: true    }});
for ( const myKey in myObject ) { 
const myValue = myObject[ myKey ];
console.log( `${ myKey } : ${ myValue }` );
}
>"myProperty : true"
>"protoProperty : true"
```

JavaScript proporciona métodos integrados para determinar si una propiedad es una propiedad directa del objeto en lugar de una propiedad de la cadena de prototipos del objeto: los métodos [modernos](https://caniuse.com/mdn-javascript_builtins_object_hasown) `Object.hasOwn()` y `Object.prototype.hasOwnProperty()` heredados. Estos métodos evalúan si una propiedad especificada es heredada (o no declarada) y muestran `true` solo para las propiedades inmediatas de un objeto especificado:

```js
const myPrototype = { "protoProperty" : true };
const myObject = Object.create( myPrototype, {    myProperty: {    value: true,    enumerable: true    }});
for ( const myKey in myObject ) {  const myValue = myObject[ myKey ];
if ( Object.hasOwn( myObject, myKey ) ) {    console.log( `${ myKey } : ${ myValue }` );
 }
}
>"myProperty : true"
```

También hay tres métodos estáticos, cada uno de los cuales muestra un array compuesto por las claves enumerables (`Object.keys()`), los valores (`Object.values()`) o los pares clave-valor (`Object.entries()`) de un objeto:

```js
const myObject = { "myProperty" : true, "mySecondProperty" : false };
Object.keys( myObject );
>Array [ "myProperty", "mySecondProperty" ]
```

Esto te permite iterar claves, valores o pares clave-valor de objetos (mediante la [asignación de desestructuración](https://web.dev/learn/javascript/collections/indexed?hl=es-419#destructuring-assignment)) sin incluir propiedades del prototipo de ese objeto:

```js
const myPrototype = { "protoProperty" : "Non-enumerable property value." };
const myObject = Object.create( myPrototype, {    myProperty: {    value: "Enumerable property value.",    enumerable: true    }});
for ( const propKey of Object.keys( myObject ) ) {  console.log( propKey );
}
> "myProperty"
for ( const propValue of Object.values( myObject ) ) {  
console.log( propValue );
}
> "Enumerable property value."
for ( const [ propKey, propValue ] of Object.entries( myObject ) ){ 
console.log( `${ propKey } : ${ propValue }` );
}
> "myProperty : Enumerable property value."
```

#### `forEach()`

Los métodos `forEach()` que proporcionan los constructores [Array](https://web.dev/learn/javascript/collections/indexed?hl=es-419#array), [Map](https://web.dev/learn/javascript/collections/keyed?hl=es-419#map), [Set](https://web.dev/learn/javascript/collections/keyed?hl=es-419#set) y NodeList proporcionan una abreviatura útil para iterar sobre una estructura de datos en el contexto de una función de devolución de llamada. A diferencia de otras formas de bucle, un bucle creado con cualquier método `forEach()` no se puede interrumpir usando `break` ni `continue`.

`forEach` es un método que pertenece al prototipo de cada estructura de datos. Cada método `forEach` espera una función de devolución de llamada como argumento, aunque varían ligeramente en términos de los argumentos incluidos cuando se llama a esa función. Un segundo argumento opcional especifica un valor `this` para usar como contexto de invocación de la función de devolución de llamada.

La función de devolución de llamada que se usa con `Array.forEach` proporciona parámetros que contienen el valor del elemento actual, el índice del elemento actual y el array en el que se invocó el método `forEach`:

```js
const myArray = [ true, false ];
myArray.forEach( ( myElement, i, originalArray ) => {  console.log( i, myElement, originalArray  );
});
> 0 true 
> Array(3) [ true, false ]
> 1 false 
> Array(3) [ true, false ]
```

La función de devolución de llamada que se usa con `Map.forEach` proporciona parámetros que contienen el valor asociado con el elemento actual, la clave asociada con este y el mapa en el que se invocó el método `forEach`:

```js
const myMap = new Map([  ['myKey', true],  ['mySecondKey', false ],]);
myMap.forEach( ( myValue, myKey, originalMap ) => {    console.log( myValue, myKey, originalMap  );
});
> true "myKey" Map { myKey → true, mySecondKey → false }
> false "mySecondKey" Map { myKey → true, mySecondKey → false }
```

Una devolución de llamada `Set.forEach` incluye parámetros similares. Debido a que Set no tiene índices ni claves distintos de los valores, el segundo argumento proporciona un valor redundante que se puede ignorar estrictamente para mantener la coherencia de la sintaxis con los otros métodos `forEach`.

```js
const mySet = new Set([ true, false ]);
mySet.forEach( ( myValue, myKey, originalSet ) => {  console.log( myValue, myKey, originalSet  );
});
> true true Set [ true, false ]
> false false Set [ true, false ]
```

### Iteradores

Un _iterable_ es cualquier estructura de datos compuesta por elementos individuales que se pueden iterar con los enfoques detallados anteriormente. Un _iterador_ es un objeto iterable que sigue el _protocolo iterador_, lo que significa que debe implementar un método `next()` que avance por los elementos que contiene, uno a la vez, cada vez que se llama a ese método y muestra un objeto para cada elemento secuencial en un formato específico.

Las estructuras de datos iterables integradas de JavaScript (como [Array](https://web.dev/learn/javascript/collections/indexed?hl=es-419#array), [Map](https://web.dev/learn/javascript/collections/keyed?hl=es-419#map) y [Set](https://web.dev/learn/javascript/collections/keyed?hl=es-419#set)) no son iteradores por sí mismos, pero todas heredan un método `iterator`, al que se puede acceder mediante el [símbolo conocido](https://web.dev/learn/javascript/data-types/symbol?hl=es-419#well-known) de `@@iterator`, que muestra un objeto iterador creado a partir de la estructura de datos iterable:

```js
const myIterable = [ 1, 2, 3 ];
const myIterator = myIterable[ Symbol.iterator ]();
>myIterable;
> (3) [1, 2, 3]myIterator;
> Array Iterator {}
```

Llamar al método `next()` en un iterador recorre los elementos que contiene, uno a la vez, y cada llamada muestra un objeto que contiene dos propiedades: `value`, que contiene el valor del elemento actual, y `done`, un valor booleano que indica si el iterador pasó el último elemento de la estructura de datos. El valor de `done` es `true` solo cuando una llamada a `next()` da como resultado un intento de acceso a un elemento más allá del último elemento del iterador.

```js
const myIterable = [ 1, 2, 3 ];
const myIterator = myIterable[ Symbol.iterator ]();
myIterator.next();
> Object { value: 1, done: false }
 myIterator.next();
> Object { value: 2, done: false }
myIterator.next();
> Object { value: 3, done: false }
myIterator.next();
> Object { value: undefined, done: true }
```

#### Funciones de generador

Usa la palabra clave `function*` (ten en cuenta el asterisco) para declarar una función de generador o definir una expresión de función de generador:

```js
function* myGeneratorFunction() { };
```

Al igual que los [iteradores](https://web.dev/learn/javascript/control-flow?hl=es-419#iterators), las funciones de generador mantienen el estado. Si llamas a una función de generador, se muestra un objeto Generador nuevo, pero no se ejecuta de inmediato el código en el cuerpo de la función:

```js
function* myGeneratorFunction() {  
console.log( "Generator function body ")};
const myGeneratorObject = myGeneratorFunction();myGeneratorObject;
> Generator {  }typeof myGeneratorObject;
> "object"
```

Los objetos generadores siguen el [protocolo iterador](https://web.dev/learn/javascript/control-flow?hl=es-419#iterators). El valor que muestra cada llamada a `next()` en una función de generador está determinado por una expresión `yield`, que pausa la ejecución de la función del generador y muestra el valor de la expresión que contiene la palabra clave `yield`. Las llamadas posteriores a `next()` continúan la ejecución de la función, se detiene en la siguiente expresión `yield` y se muestra el valor asociado.

```js
function* myGeneratorFunction() { 
yield "My first yielded value.";
yield "My second yielded value.";
};
const myGeneratorObject = myGeneratorFunction();
myGeneratorObject.next();
> Object { value: "My first yielded value.", done: false }
> myGeneratorObject.next();
> Object { value: "My second yielded value.", done: false }
```

Cuando se llama a `next()` después de que no se especifican más valores mediante `yield`, `return` o `throw` (en caso de que se produzca un error), se ejecuta el resto del cuerpo de la función, y el objeto que se muestra tiene un `value` de `undefined` y una propiedad `done` de `true`:

```js
function* myGeneratorFunction() {    
console.log( "Start of the generator function." );   yield "First";    
console.log( "Second part of the generator function."  );    
yield "Second";    
console.log( "Third part of the generator function." );  
yield "Third";
};
const myGeneratorObject = myGeneratorFunction();
myGeneratorObject.next();
> "Start of the generator function."
> Object { value: "First", done: false }
myGeneratorObject.next();
> "Second part of the generator function."
> Object { value: "Second", done: false }
> myGeneratorObject.next();
> "Third part of the generator function."> Object { value: "Third", done: false }
> myGeneratorObject.next();
> Object { value: undefined, done: true }
```

Usa `next()` solo en el objeto que muestra la función de generador, no en la función de generador en sí. De lo contrario, cada llamada a la función de generador crea un nuevo objeto generador:

```js
function* myGeneratorFunction() {
yield "First";
yield "Second";};
myGeneratorFunction().next();
> Object { value: "First", done: false }
> myGeneratorFunction().next();
> Object { value: "First", done: false }
```

Al igual que con cualquier función, la función del generador se detiene cuando encuentra una palabra clave `return`. Luego, muestra un objeto al contexto de invocación que contiene el valor mostrado y una propiedad `done` con el valor `true`.

```js
function* myGeneratorFunction() {
yield 1;  yield 2;  return 3;};
const myGeneratorObject = myGeneratorFunction();
myGeneratorObject.next().done;
> Object { value: 1, done: false }
> myGeneratorObject.next().done;
> Object { value: 2, done: false }
> myGeneratorObject.next();
> Object { value: 3, done: true }
```

Una expresión `yield` puede adoptar parte de la semántica de un identificador, lo que permite una “comunicación” bidireccional desde y hacia la parte suspendida de la función del generador. Cuando se pasa un valor al método `next()` de un generador como argumento, se reemplaza el valor asociado con la expresión `yield` suspendida anterior:

```js
function* myGeneratorFunction() {   
const firstYield = yield;    
yield firstYield + 10;
};
const myGeneratorObject = myGeneratorFunction();
myGeneratorObject.next();
> Object { value: undefined, done: false }
> myGeneratorObject.next( 5 );
> Object { value: 15, done: false }
```

Ten en cuenta que esto reemplaza toda la expresión asociada con la `yield` anterior y no solo reasigna el valor del `yield` anterior al valor especificado en `next()`:

```js
function* myGeneratorFunction() { 
const firstYield = yield;
const secondYield = yield firstYield + 100;
yield secondYield + 10;
};
const myGeneratorObject = myGeneratorFunction();
myGeneratorObject.next();
> Object { value: undefined, done: false }
> myGeneratorObject.next( 10 ); 
// Can be thought of as changing the value of the `firstYield` variable to `10
> Object { value: 110, done: false }myGeneratorObject.next( 20 ); 
// Can be thought of as changing the value of the `secondYield` variable to `20`, _not_ `20 + 100;`
> Object { value: 30, done: false }
```

Se ignora cualquier argumento que se pase a la primera llamada a `next()`, ya que no hay ninguna expresión `yield` anterior para aceptar ese valor. Al igual que con cualquier otra función, los argumentos pasados a la llamada inicial a la función del generador están disponibles en todo el alcance del cuerpo de la función del generador:

```js
function* myGeneratorFunction( startingValue ) {    let newValue = yield startingValue + 1;
newValue = yield newValue + 10;
yield startingValue + 20;
};
const myGeneratorObject = myGeneratorFunction( 2 );
myGeneratorObject.next( 1 );
> Object { value: 3, done: false }
> myGeneratorObject.next( 5 );
> Object { value: 15, done: false }
> myGeneratorObject.next( 10 );
> Object { value: 22, done: false }
```

El operador `yield*` (ten en cuenta el asterisco) se usa con un iterable, como otra función de generador, para iterar y generar cada valor que muestra su operando:

```js
function* mySecondaryGenerator() {  
yield 2;
yield 3;
}
function* myGenerator() { 
yield 1; 
yield* mySecondaryGenerator();
yield 4;
return 5;
}
const myIterator = myGenerator();
myIterator.next();
> Object { value: 1, done: false }
> myIterator.next();
> Object { value: 2, done: false }myIterator.next();
> Object { value: 3, done: false }
> myIterator.next();
> Object { value: 4, done: false }
> myIterator.next();
> Object { value: 5, done: true }
```

## JavaScript asíncrono

Si bien JavaScript es en esencia [síncrono](https://web.dev/learn/javascript/appendix?hl=es-419#main-thread) en ejecución, hay mecanismos que permiten a los desarrolladores aprovechar el [bucle de eventos](https://web.dev/learn/javascript/appendix?hl=es-419#event-loop) para realizar tareas asíncronas.

### Promesas

Una promesa es un marcador de posición para un valor que se desconoce cuando se crea la promesa. Es un contenedor que dicta una operación asíncrona, los términos por los cuales la operación se considera un éxito o un fracaso, las acciones que se deben realizar en cualquier caso y el valor que se genera.

Crea una instancia de promesa mediante el operador `new` con la función de constructor `Promise` integrada. Este constructor acepta una función llamada _executor_ como argumento. Esa función ejecutor normalmente se usa para realizar una o más acciones asíncronas y, luego, dictar los términos por los cuales la promesa debe considerarse completada o rechazada de forma correcta. Una promesa se define como _pending_ mientras se ejecuta la función ejecutor. Cuando el ejecutor finaliza, una promesa se considera _cumplida_ (o _resuelta_, en algunas fuentes de documentación) si la función del ejecutor y la acción asíncrona que realiza se completan con éxito, y _se rechazan_ si la función del ejecutor encuentra un error o falla la acción asíncrona. Después de que se cumple o rechaza una promesa, esta se considera _cumplida_.

```js
const myPromise = new Promise( () => {});
```

El constructor llama a la función ejecutor con dos argumentos. Esos argumentos son funciones que te permiten cumplir o rechazar la promesa de forma manual:

```js
const  myPromise = new Promise( ( fulfill, reject ) => { });
```

Se llama a las funciones que se usan para cumplir o rechazar una promesa con el valor resultante de la promesa como argumento (por lo general, un error de rechazo):

```js
const myPromise = new Promise( ( fulfill, reject ) => {  
const myResult = true;
setTimeout(() => {   
if( myResult === true ) {
fulfill( "This Promise was successful." ); 
}else {    
reject( new Error( "This Promise has been rejected." ) );
 }  
}, 10000);
});
myPromise;
> Promise { <state>: "pending" }
 myPromise;
 > Promise { <state>: "fulfilled", <value>: "This Promise was successful." }
```

#### Encadenamiento de promesas

Se puede actuar sobre el objeto Promise resultante con los métodos `then()`, `catch()` y `finally()` heredados del constructor Promise. Cada uno de estos métodos muestra una promesa, en la que se puede actuar de inmediato con `then()`, `catch()` o `finally()` otra vez, lo que te permite _encadenar_ las promesas resultantes.

`then()` proporciona dos funciones de devolución de llamada como argumentos. Usa la primera para cumplir la promesa resultante y la segunda para rechazarla. Ambos métodos aceptan un solo argumento que le da su valor a la promesa resultante.

```js
const myPromise = new Promise( ( fulfill, reject ) => { 
const myResult = true;
setTimeout(() => {    
if( myResult === true ) {
fulfill( "This Promise was fulfilled." );       
}else { 
reject( new Error( "This Promise has been rejected." ) );  
} 
}, 100);
});
myPromise.then( successfulResult => console.log( successfulResult ),failedResult => console.error( failedResult ) );
>"This Promise was successful."
```

También puedes usar `then()` para controlar solo el estado entregado y `catch` para manejar el estado rechazado. Llama a `catch` con un solo argumento que contenga el valor proporcionado en el método de rechazo de la promesa:

```js
const myPromise = new Promise( ( fulfill, reject ) => {  
const myResult = false;
setTimeout(() => { 
if( myResult === true ) { 
fulfill( "This Promise was fulfilled." );        } else {    
reject( new Error( "This Promise has been rejected." ) ); 
} }, 100);
});
myPromise  
.then( fulfilledResult => console.log(fulfilledResult ) )  
.catch( rejectedResult => console.log( rejectedResult ) )  
.finally( () => console.log( "The Promise has settled." ) );
> "Error: This Promise has been rejected."
> "The Promise has settled."
```

A diferencia de `then` y `catch`, que permiten que una función de controlador se ejecute cuando se cumple o se rechaza una promesa, se llama a una función pasada como argumento al método `finally` sin importar si la promesa se cumplió o se rechazó. Se llama a la función del controlador sin argumentos porque no está diseñada para trabajar con los valores que se pasaron desde la Promesa, sino solo para ejecutar el código después de que se completa la Promesa.

#### Simultaneidad

El constructor Promise proporciona cuatro métodos para trabajar con varias promesas relacionadas mediante un [iterable](https://web.dev/learn/javascript/control-flow?hl=es-419#iterators) que contiene objetos Promise. Cada uno de estos métodos muestra una promesa, que se cumple o se rechaza según el estado de las promesas que se le hayan pasado. `Promise.all()`, por ejemplo, crea una promesa que se cumple solo si se cumple cada promesa que se pasa a ese método:

```js
const firstPromise  = new Promise( ( fulfill, reject )=> fulfill( "Successful. ") );

const secondPromise = new Promise( ( fulfill, reject ) => fulfill( "Successful. ") );
const thirdPromise  = new Promise( ( fulfill, reject ) => fulfill( "Successful. ") );
const failedPromise = new Promise( ( fulfill, reject ) => reject( "Failed.") );
const successfulPromises = [ firstPromise, secondPromise, thirdPromise ];
const oneFailedPromise = [ failedPromise, ...successfulPromises ];
Promise.all( successfulPromises )  
.then( ( allValues ) => {    
console.log( allValues ); 
}) 
.catch( ( failValue ) => {  
console.error( failValue );
});
> Array(3) [ "Successful. ", "Successful. ", "Successful. " ]
 Promise.all( oneFailedPromise  ) 
 .then( ( allValues ) => {    
console.log( allValues ); 
})  
.catch( ( failValue ) => { 
console.error( failValue );  
});
> "Failed."
```

Los métodos de simultaneidad de Promise son los siguientes:

`Promise.all()`

Se completa solo si se cumplen todas las promesas proporcionadas.

`Promise.any()`

Se completa si se cumple alguna de las promesas proporcionadas y se rechaza solo si se rechazan todas.

`Promise.allSettled()`

Se cumplen cuando se cumplen las promesas, independientemente del resultado.

`Promise.race()`

Se rechaza o se cumple en función del resultado de la primera promesa que se concilia, se ignoran todas las promesas liquidadas más tarde.

#### `async`/`await`

Cuando usas la palabra clave `async` antes de una [declaración de función](https://web.dev/learn/javascript/functions?hl=es-419) o una [expresión de función](https://web.dev/learn/javascript/functions/function-expressions?hl=es-419), cualquier valor que muestre esa función se muestra como una promesa cumplida que contiene ese valor. Esto te permite ejecutar y administrar operaciones asíncronas con los mismos flujos de trabajo que el desarrollo síncrono.

```js
async function myFunction() {
return "This is my returned value.";
}
myFunction()
.then( myReturnedValue => console.log( myReturnedValue ) );
> "This is my returned value."
```

La expresión `await` pausa la ejecución de una función asíncrona mientras se establece la promesa asociada. Una vez que se establece la promesa, el valor de la expresión `await` es el valor cumplido o rechazado de la promesa.

```js
async function myFunction() {
const myPromise  = new Promise( ( fulfill, reject ) => { setTimeout( () => fulfill( "Successful. "), 5000 );
});
const myPromisedResult = await myPromise;  
return myPromisedResult;
}
myFunction()  
.then( myResult => console.log( myResult ) ) 
.catch( myFailedResult => console.error( myFailedResult ) );
> "Successful."
```

Cualquier valor que no sea promesa incluido en una expresión `await` se muestra como una promesa completada:

```js
async function myFunction() { 
const myPromisedResult = await "String value.";  return myPromisedResult;
}
myFunction() 
.then( myResult => console.log( myResult ) ) 
.catch( myFailedResult => console.error( myFailedResult ) );
> "String value."
```






------



### Funciones en JavaScript

Una función es un bloque modular y reutilizable de sentencias que se usa para realizar un conjunto de tareas relacionadas, como calcular y mostrar un valor según los argumentos proporcionados a la función. Las funciones son objetos únicos porque se pueden llamar para ejecutar código, pasar datos en forma de argumentos y retornar un valor.

### Conceptos Clave

- **Funciones como Objetos de "Primera Clase"**: Esto significa que las funciones pueden usarse en los mismos contextos que cualquier otro objeto de JavaScript. Por ejemplo, una función puede asignarse a una variable, pasarse como argumento a otras funciones y ser devuelta por otras funciones.

#### Ejemplo de Función Básica

javascript

```js
function myFunction() {    
console.log("This is my function."); 
}  
myFunction();  // Llama a la función // Output: "This is my function."
```


### Declaraciones de Funciones

Una declaración de función crea una función con nombre que se puede invocar en otro lugar del alcance que la contiene.

#### Ejemplo de Declaración de Función

javascript

```js
function myFunction() {    
console.log("This is my function."); 
}  
myFunction();  // Llama a la función // Output: "This is my function."
```

### Comportamiento de Elevación

Las declaraciones de funciones se elevan a la parte superior de su alcance, lo que significa que se puede llamar a la función antes de su declaración.

#### Ejemplo de Elevación

javascript

```js
"use strict"; {
myFunction();
function myFunction() {
console.log("This is my function."); 
} 
} // Output: "This is my function."
```


### Llamada a Función

Para ejecutar el código dentro del cuerpo de la función, se llama a la función siguiendo el nombre de la función con un par de paréntesis.

#### Ejemplo de Llamada a Función

javascript

Copiar código

```js
function myFunction() { 
console.log("My function has been executed."); 
}  
myFunction();  // Llama a la función // Output: "My function has been executed."
```

### Parámetros y Argumentos

Los parámetros en la definición de la función actúan como variables de marcador de posición para los valores que se pueden pasar al cuerpo de la función cuando se la llama.

#### Ejemplo de Parámetros y Argumentos

javascript

```js
function myFunction(myParameter) {  
console.log(`The value is: ${myParameter}.`); 
} 
myFunction("this string");  // Pasa un argumento 
// Output: "The value is: this string."``

```

### Valores Predeterminados de Parámetros

Para configurar los valores predeterminados de los parámetros, inicialízalos de la misma manera en que inicializarías una variable.

#### Ejemplo de Valores Predeterminados

javascript

```js
function myFunction(myParameter = "omitted") {    console.log(`The value is: ${myParameter}.`);
}  
myFunction("this string");  // Pasa un argumento 
// Output: "The value is: this string."  myFunction(); // No pasa argumentos 
// Output: "The value is: omitted."
```


### El Objeto `arguments`

El cuerpo de una función también tiene acceso a un objeto `arguments` tipo array con índice cero que contiene todos los valores pasados como argumentos.

#### Ejemplo del Objeto `arguments`

javascript

```js

```
function myFunction() {    console.log(arguments); }  myFunction(3, true, "My string"); // Output: Arguments { 0: 3, 1: true, 2: "My string", … }`

### Funciones Variádicas

Las funciones variádicas pueden aceptar una cantidad variable de argumentos utilizando la sintaxis del parámetro REST.

#### Ejemplo de Funciones Variádicas

javascript

Copiar código

`function myFunction(mySeparator, ...myStrings) {   console.log(myStrings.join(mySeparator)); }  myFunction(" - ", "My first string", "My second string", "my third string"); // Output: "My first string - My second string - my third string"`

### Resumen

Las funciones en JavaScript son poderosas y flexibles, permitiendo modularidad, reutilización de código y una variedad de maneras de trabajar con parámetros y argumentos. Entender cómo declarar, llamar y manejar funciones es fundamental para desarrollar aplicaciones eficientes y mantenibles en JavaScript.