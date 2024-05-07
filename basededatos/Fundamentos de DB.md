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

[[Drawing 2024-04-22 10.54.33.excalidraw]]