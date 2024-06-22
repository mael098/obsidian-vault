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
// Resultado: This //is a string.
```


### Interpolación en Literales de Plantilla

Puedes insertar expresiones dentro de un literal de plantilla usando `${}`:

javascript

Copy code

``console.log(`The result is ${2 + 4}.`); // Resultado: The result is 6.``

### Plantillas Etiquetadas

Se pueden usar funciones personalizadas con literales de plantilla, recibiendo un array con la cadena dividida y los marcadores de posición como argumentos:

javascript

Copy code

``const myNoun = "template literal";  function myTagFunction(myStrings, myPlaceholder) {     const myInitialString = myStrings[0];     console.log(`${myInitialString}modified ${myPlaceholder}.`); }  myTagFunction`I'm a ${myNoun}.`; // Resultado: I'm a modified template literal.``