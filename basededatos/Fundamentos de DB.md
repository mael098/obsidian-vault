Morales Dias Selene Valeria

### Competencia especifica de la asignatiura
Analiza requerimientos y disena db para generar soluciones al tratamiento de informacion basandose en modelos y estandares

### Competencia previa
Comprende y aplica los conceptos basicos de logica matematica, conjuntos y relaciones para aplicarlos en modelos que resuelvan problemas computacionales

**datos:**
> es un texto, numero, o conjunto arbitrariamente grande de ambos

**informacion:**
> conjunto de datos relacionados que dan un contexto
![[erp1.png]]


---

## Practica 2
Revisar y obtener el entorno que nos rodea, 5 fuentes de recolección de datos de uso distinto.

![[Pasted image 20240207113804.png]]

---
# Diagrama ER

es un tipo de diagrama de flujo que ilustra como las entidades , como personas , objetos o conceptos, se relacionan entre si dentro de un sistema. Los ERD se usan para diseñar o depurar bd relacionales en los campos de ingeniería de software, sistemas de información empresarial, educación e investigación..
Estos emplean un conjunto definido de símbolos, tales como rectángulos, diamantes, óvalos y lineas de conexión para representar la interpolación de entidad del , relaciones y sus atributos; Las entidades se escriben como sustantivos y las relaciones como verbos

# Entidad
algo que se puede definir, como una persona, objeto, concepto u evento,que puede tened datos almacenados acerca de este. Piensa en las entidades como si fueran sustantivos, por ejemplo, un cliente, un estudiante, un auto 

## Tipo de entidad:
un grupo de cosas que se puede definir como estudiantes o atletas.

## Conjunto de entidades:
es igual que un tipo de entidad pero se define en un momento determinado,  como por ejemplo estudiantes que se inscribieron en una clase el primer día. Un termio relacionado es una instancia en la que una persona relacionada podría ser una instancia de un conjunto de entidades
## Categoría de entidades:
Se dividen en tres, fuertes, débiles o asociativas. Una entidad fuerte se puede por sus propios atributos una entidad es aquella que relaciona entidades

## Relación:
Como la entidades interactuan o se asocian entre si piense en las entidades como si fueran verbos por ejemplo el estudiante podría inscribirse a un curso, las dos entidades son estudiantes y el curso y la relación es la inscripción que conecta ambas entidades y su representación es el diamante

## Atributo:
Es una propiedad o característica de una entidad y se muestra como un ovalo

## Cardinalidad:
Define los atributos numéricos de la relación entre dos entidades o conjunto de entidades. Las tres relaciones cardinales principales son `1:1`, `1:n` y `n:n` 
**Ejemplo de 1:1** seria un estudiante asociado a una dirección de correo electrónico
**Ejemplo de 1:n** seria un estudiante que se inscribe en muchos cursos, y todos esos cursos se asocian a ese estudiante en particular
**Ejemplo de n:n** serian los estudiantes en grupo están asociados a multiples miembros de la facultad y a su vez, los miembros de la facultad están asociados a multiples estudiantes

### Ej1
```
Alumno (n de matricula, nombre, fecha de nacimeinto, tefelono)
Asignatura (Codigo asignatura, nombre)
Profesor (id_profesror, nombre, especialidad, telefono)
```
- Teniendo en cuenta un alumno puede estar matriculado a una o varias materias, ademas puede estar matriculado en la misma asignatura mas de un curso escolar (si repite)
- Se quiere saber el curso escolar en el que cada alumno esta matriculado de cada asignatura
- En cada asignatura habrá como mínimo 10 y como máximo 25 alumnos
- una asignatura es impartida por un único profesor. 
- un profesor podrá impartir varias asignaturas

---
Ej3
Se necesita realizar una base de datos que permita apoyar la administración de un sistema de ventas. La organización necesita llevar un control de proveedores, clientes, productos y ventas.
- Un **==proveedor==** tiene un id, nombre, dirección, teléfono y pagina web. 
- Un **==cliente==** también tiene id, nombre, dirección, pero puede tener varios **==teléfonos==** de contacto. 
- La dirección se entiende por calle, numero, colonia y ciudad.
- Un **==producto==** tiene un id único, nombre, precio actual, stock y nombre del proveedor.
- Ademas los productos se organizan en **==categorías==** y cada producto va solo en una categoría
- Una categoría tiene id, nombre y descripción
- Por razones de contabilidad se debe registrar la información de cada **==venta==** con un id, fecha, cliente, descuento, y monto final.
- Ademas se debe guardar el precio al momento de la venta, la cantidad vendida y el monto total por el producto

---

1. **Base de Datos**:
   - *Definición*: Una base de datos es un conjunto organizado de datos que están estructurados y almacenados electrónicamente en un sistema informático. Está diseñada para permitir el acceso, recuperación y gestión eficiente de la información.
   - *Ejemplo*: Una base de datos de una biblioteca puede contener información sobre libros, autores, préstamos y usuarios. Estos datos estarían organizados en tablas relacionadas entre sí, lo que permite a los usuarios buscar y acceder a la información de manera rápida y eficiente.
2. **Tabla**:
   - *Definición*: Una tabla es una estructura fundamental en una base de datos relacional que organiza los datos en filas y columnas. Cada fila representa una entidad individual y cada columna representa un atributo de esa entidad.
   - *Ejemplo*: Una tabla de empleados en una base de datos de recursos humanos podría tener columnas como "ID de empleado", "Nombre", "Apellido", "Departamento", etc.

3. **Campo y Tipos de campos**:
   - *Definición*: Un campo es una unidad individual para almacenar datos en una tabla. Los tipos de campos definen qué tipo de datos pueden almacenarse en un campo específico, como números, texto, fechas, etc.
   - *Ejemplo*: En una tabla de empleados, el campo "Nombre" podría ser de tipo texto, mientras que el campo "Edad" podría ser de tipo numérico.

4. **Registro**:
   - *Definición*: Un registro, también conocido como fila, es una instancia individual de datos en una tabla que contiene valores para cada uno de los campos definidos en la tabla.
   - *Ejemplo*: Cada entrada única en la tabla de empleados, como "001, Juan, Pérez, Ventas", representa un registro individual.

5. **Campo Llave**:
   - *Definición*: Un campo clave es un campo o conjunto de campos que identifican de forma única cada registro en una tabla. Se utiliza para establecer relaciones entre tablas.
   - *Ejemplo*: En la tabla de empleados, el campo "ID de empleado" podría ser una clave primaria única que identifica de manera exclusiva a cada empleado.

6. **Trigger**:
   - *Definición*: Un trigger es un tipo de procedimiento almacenado en una base de datos que se ejecuta automáticamente cuando se produce un evento específico, como la inserción, actualización o eliminación de datos en una tabla.
   - *Ejemplo*: Un trigger puede configurarse para enviar un correo electrónico a un administrador cada vez que se inserta un nuevo empleado en la tabla de empleados.

7. **Diagrama E/R (Entidad/Relación)**:
   - *Definición*: Un diagrama E/R es una representación visual de las entidades dentro de un sistema y las relaciones entre ellas. Se utiliza para diseñar la estructura de una base de datos relacional.
   - *Ejemplo*: En un diagrama E/R de una base de datos de ventas, tendrías entidades como "Cliente", "Producto" y "Pedido", y relaciones que indican cómo están relacionadas estas entidades.

8. **Diagrama R (Relacional)**:
   - *Definición*: Un diagrama relacional muestra la estructura de las tablas en una base de datos relacional, incluyendo los campos y las relaciones entre ellas.
   - *Ejemplo*: Un diagrama relacional de una base de datos de biblioteca mostraría las tablas "Libro", "Autor" y "Préstamo", junto con las relaciones entre ellas.

9. **Normalizaciones**:
   - *Definición*: Las normalizaciones son reglas y directrices utilizadas para diseñar y optimizar la estructura de una base de datos relacional, con el objetivo de reducir la redundancia y mejorar la integridad de los datos.
   - *Ejemplo*: La primera forma normal (1NF) garantiza que cada campo en una tabla contenga valores atómicos, mientras que la tercera forma normal (3NF) elimina las dependencias transitivas entre los campos.

---

### Clientes
- ID_Cliente
- Correo
- Nombre

### Productos
- ID_Producto
- Precio
- Nombre_Producto
- ID_Categoria

### Envios
- ID_Envio
- Direccion
- CP
- Ciudad
- Pais
- Estado
- Nombre

### Ventas
- ID_Venta
- Tipo_de_Pago
- Fecha
- Hora
- ID_Cliente
- ID_Envio

### Categorias
- ID_Categorias
- Tipo

![[Fundamentos de DB 2024-04-22 11.06.54.excalidraw]]

---
Tarea

![[Fundamentos de DB 2024-04-26 10.08.32.excalidraw]]
 
 ![[Pasted image 20240426102810.png]]
 ----




select => la instrucción  select en SQL se utiliza para seleccionar datos de una base de datos. Los datos de vueltos se  almacenan en una tabla de resultados llamada conjunto de resultados.


```sql
SELECT column1, column2, ...
```


from :  =>  la clausula from de SQL es el origen de un conjunto de filas sobre el que se va a operar en un instrucción de lenguaje de manipulación de datos 
```SQL
FROM table_name;
```

where =>La **cláusula WHERE** en SQL es fundamental para filtrar datos en una consulta. Permite incluir solo las filas que cumplen ciertas condiciones. 
```SQL
SELECT title, author_name, year
FROM books
WHERE year >= 2020
ORDER BY author_name;
```


like =>
El SQL `LIKE` es un operador lógico que comprueba si una cadena contiene o no un patrón específico.
```SQL
SELECT column_1, column_2, ... column_n
FROM table_name
WHERE column_1 LIKE pattern
```

,and=> **AND**: Este operador se utiliza para combinar múltiples condiciones en una consulta. Devolverá todas las filas que cumplan **todas** las condiciones dadas.
```SQL
SELECT * FROM members WHERE Age < 50 AND Location = 'Los Angeles';
```

order  by => La **cláusula ORDER BY** en SQL se utiliza para organizar los resultados de una consulta en un orden específico.
```SQL
SELECT * FROM sales_performance ORDER BY sales_person_id;
```

asc =>  - **ASC** es la forma corta de “ascendente”. Se utiliza para ordenar los resultados de la consulta de arriba hacia abajo.
```SQL
SELECT columna1, columna2
FROM tabla
ORDER BY columna1 ASC/DESC;
```

desc => - **DESC** es la forma corta de “descendente”. Se utiliza para ordenar los resultados de la consulta de abajo hacia arriba.
```SQL
SELECT columna1, columna2
FROM tabla
ORDER BY columna1 ASC/DESC;
```

 Group By =>**GROUP BY** te permite agrupar datos por un atributo común y realizar cálculos en cada grupo por separado.
 ```SQL
 SELECT director,

      count (*)  AS number_of_movies

FROM movies

GROUP BY director;
```

count => La función **COUNT()** en SQL se utiliza para contar filas. Específicamente, cuenta las filas en el conjunto de resultados, no en la tabla directamente. Aquí tienes algunos detalles sobre su uso 
```SQL
SELECT COUNT(*) AS total_filas
FROM nombre_de_tabla;
```
, as =>La cláusula Alias (AS) es un comando que se utiliza para asignar un nombre alternativo a una tabla o columna en una consulta SQL. Esto significa que puedes cambiar el nombre de una tabla o columna para que sea más fácil de entender o de recordar.
```SQL
SELECT nombre_completo AS nombre FROM empleados
```
, avg => La función **AVG()** en SQL se utiliza para encontrar el promedio de valores sobre los registros de una tabla.
```SQL
SELECT AVG(skill_level) FROM employees;
```


, having =>- **Concepto:** La cláusula HAVING se utiliza en SQL para filtrar filas después de que se hayan agrupado utilizando la cláusula GROUP BY. Permite aplicar condiciones a grupos de filas, similar a cómo WHERE se aplica a filas individuales.
```SQL
SELECT producto, SUM(cantidad) AS total_cantidad
FROM ventas
GROUP BY producto
HAVING SUM(cantidad) > 100;
```


, join=> - **Concepto:** JOIN se utiliza para combinar filas de dos o más tablas en función de una condición relacionada entre ellas. Se pueden utilizar diferentes tipos de JOIN, como INNER JOIN, LEFT JOIN, RIGHT JOIN y FULL JOIN, para controlar qué filas se incluyen en el resultado final.
```SQL
SELECT clientes.nombre, pedidos.producto, pedidos.cantidad
FROM clientes
JOIN pedidos ON clientes.id = pedidos.id_cliente;
```

, on => - **Concepto:** La cláusula ON se utiliza en combinación con la cláusula JOIN para especificar las condiciones de unión entre las tablas. Indica cómo se relacionan las filas de una tabla con las de otra en el resultado de la consulta.

```SQL
SELECT clientes.nombre, pedidos.producto, pedidos.cantidad
FROM clientes
JOIN pedidos ON clientes.id = pedidos.id_cliente;
```



----

# data base

ejercisio 1

tabla 


```SQL 
create database ejercio1
use ejercio1

create table (
id var('30')
)

create table peliculas (
id in not null autoincremental
titulo_peli, 
ratik,
año_extreno,
presupuesto ,
ingresos, 
lenguaje 
);
```
