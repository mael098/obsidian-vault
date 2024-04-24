

1. conceptos base de datos 


| conceptos                 | definiciones                                                                                      | ejemplos                                                                                                                                  |
| ------------------------- | ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| base de datos             | se encarga no solo de almacenar datos, sino también de conectarlos entre sí en una unidad lógica. | En las bases de datos, los datos deben estar estructurados e interrelacionados según un modelo que refleje el máximo contenido semántico. |
| tabla                     |                                                                                                   |                                                                                                                                           |
| campos de tipos de campos |                                                                                                   |                                                                                                                                           |
| registros                 |                                                                                                   |                                                                                                                                           |
| campo llave               |                                                                                                   |                                                                                                                                           |
| diagrama E/R              |                                                                                                   |                                                                                                                                           |
| diagrama R                |                                                                                                   |                                                                                                                                           |
| normalizacion             |                                                                                                   |                                                                                                                                           |




 - revisado

| Concepto                 | Definiciones                                                                                                                                                | Ejemplos                                                                                                                                    |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Base de datos            | Conjunto organizado de datos que se estructuran y relacionan entre sí para su almacenamiento y uso.                                                         | Un sistema de gestión de base de datos (SGBD) como MySQL, PostgreSQL o MongoDB.                                                             |
| Tabla                    | Estructura de datos que organiza la información en filas y columnas.                                                                                        | En una base de datos de un sistema de gestión de biblioteca, puede haber una tabla para libros, otra para clientes, etc.                    |
| Campos y tipos de campos | Campos son los componentes individuales de una tabla que contienen la información. Tipos de campos se refiere al tipo de datos que puede contener un campo. | Un campo "Nombre" de tipo texto en una tabla de clientes. Un campo "Edad" de tipo entero en una tabla de empleados.                         |
| Registros                | Conjunto de datos relacionados que conforman una fila en una tabla.                                                                                         | Un registro en una tabla de empleados puede incluir el nombre, la edad, el salario, etc., de un empleado específico.                        |
| Campo llave              | Campo o conjunto de campos cuyos valores identifican de manera única cada registro en una tabla.                                                            | Un campo "ID" que contiene un número único para cada empleado en una tabla de empleados.                                                    |
| Diagrama E/R             | Representación gráfica de las entidades y las relaciones entre ellas en una base de datos.                                                                  | Un diagrama que muestra cómo las entidades "Empleado", "Departamento" y "Proyecto" están relacionadas entre sí en una base de datos.        |
| Diagrama R               | Representación gráfica de las restricciones de integridad referencial entre tablas.                                                                         | Un diagrama que muestra cómo las tablas de "Empleado" y "Departamento" están relacionadas mediante una clave foránea.                       |
| Normalización            | Proceso de diseño de bases de datos que se centra en organizar los datos y minimizar la redundancia.                                                        | Dividir una tabla grande y poco estructurada en tablas más pequeñas y relacionadas para mejorar la eficiencia y la integridad de los datos. |



-----
---
___




| clients                                  | producto                                  | envios    | ventas       | categorias   |     |
| ---------------------------------------- | ----------------------------------------- | --------- | ------------ | ------------ | --- |
| clien_id   int not null auto_inclemental | id_producto int not null auto_inclemental | dirección | tipo de pago | id_categoria |     |
| correo carchat() not null                | nombre del producto not null              | cp        | fecha        | tipos        |     |
| nombre not null                          |                                           | ciudad    | hora         | id_producto  |     |
|                                          |                                           | pais      | id_cliente   |              |     |
|                                          |                                           | estado    | id_envio     |              |     |
|                                          |                                           | Id_envio  |              |              |     |
|                                          |                                           | id_ventas |              |              |     |
|                                          |                                           | cliente   |              |              |     |



------


| Tabla: Estudiante  |
| :----------------- |
| ID (PK)            |
| Nombre             |
| Apellido           |
| Correo electrónico |
| Teléfono           |
| Carrera            |

| Tabla: Inscripción   |
| :------------------- |
| ID (PK)              |
| ID_Estudiante (FK)   |
| ID_Jornada (FK)      |
| Fecha de inscripción |

| Tabla: Jornada       |
| :------------------- |
| ID (PK)              |
| Nombre de la jornada |
| Fecha                |
| Hora de inicio       |
| Hora de finalización |
| Lugar                |



- estudiantes

| Field    | Type         | Null | Key | Default | Extra          |
| -------- | ------------ | ---- | --- | ------- | -------------- |
| ID       | int          | NO   | PRI | NULL    | auto_increment |
| Nombre   | varchar(100) | NO   |     | NULL    |                |
| Apellido | varchar(100) | NO   |     | NULL    |                |
| Email    | varchar(100) | NO   |     | NULL    |                |
| Telefono | varchar(20)  | YES  |     | NULL    |                |
| Carrera  | varchar(100) | YES  |     | NULL    |                |


- jornada

| Field             | Type         | Null | Key | Default | Extra          |
| ----------------- | ------------ | ---- | --- | ------- | -------------- |
| ID                | int          | NO   | PRI | NULL    | auto_increment |
| Nombre_Jornada    | varchar(100) | NO   |     | NULL    |                |
| Fecha             | date         | NO   |     | NULL    |                |
| Hora_Inicio       | time         | NO   |     | NULL    |                |
| Hora_Finalizacion | time         | NO   |     | NULL    |                |
| Lugar             | varchar(100) | NO   |     | NULL    |                |


- inscripciones

| Field             | Type     | Null | Key | Default | Extra          |
| ----------------- | -------- | ---- | --- | ------- | -------------- |
| ID                | int      | NO   | PRI | NULL    | auto_increment |
| ID_Estudiante     | int      | NO   | MUL | NULL    |                |
| ID_Jornada        | int      | NO   | MUL | NULL    |                |
| Fecha_Inscripcion | datetime | NO   |     | NULL    |                |
