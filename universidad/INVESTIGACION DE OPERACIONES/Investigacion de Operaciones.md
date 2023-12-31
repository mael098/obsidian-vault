Jesus orlando Gonez Alvirenga
## Evaluacion
| -                         | -   |
| ------------------------- | --- |
| Trabajo en clase y tareas | 30  |
| Trabajo mensual           | 30  |
| Problemario               | 20  |
| Examen                    | 20  |

## Competencias previas
- algebra
- algebra lineal

## Programas sugeridos
- QSB

## Temario
1. Programacion lineal
	1. Definicion de modelos
	2. Modelos
	3. Metodo grafico
	4. Metodo simple
	5. Aplicaciones
2. Analisis de redes
	1. Conceptos basicos
	2. Prob. transporte
	3. Prob. asignacion
	4. Prob. ruta mas corta
	5. PERT-CPM
3. Programacion no lineal
	1. Conceptos
	2. Graficos de PNL
	3. Problemas programacion
	4. Optimizacion
	5. Puntos inflexion, maximos y minimos
4. Teoria de inventarios
	1. Sistemas de administracion y control
	2. Modelos deterministicos
	3. Lotes con deficit
	4. Lotes sin deficit
	5. Cantidad economica pedido
5. Lineas de espera
	1. Definiciones y caracteristicas
	2. Terminologia y notacion
	3. Proceso de vida de la linea
	4. Modelo posicion
		- 1 servidor
		- 2 o mas servidores

## Intro
La i de o es la aplicacion por grupos interdiciplinarios del metodo cientifico a problemas relacionados con el control de las organizaciones o sistemas a din que se produzcan soluciones que mejor sirvan a los objeticos de la oirfanizacion
![[ww2.excalidraw]]

1. la tactica principal fue el metodo simplez creado por B.Dantzig
2. Creacion de la computadora

Idea uso/aplicar la IO es la toma de deciciones
- Logro de objetivos
- Informacion documentada
- Hechos
- Recursos y didponibilidad
- Ampliar variable o reducir algunas
Se basa en el metodo cientifico siquiendo los pasos que son:
- Observacion
- Formacion
- Creae modelo matematico
- Hipotesis
- Creificar hipotesis
- Concluir
Sin embargo se encargan tambien de la administracion

La optmizacion de la IO proviene de:
1. Estructuracion situacion vida real en un modelo matematico
2. analisis de estructura
3. Desarrollar soluciones
Con lo anterior obtenemos *fases de la IO*
1. Formulacion del problema
2. Crear modelo
3. Solucionar modelo
4. Validar modelo
5. Implementacion personal
Los modelos de IO pueden ser:
* Deterministicos
* Probabilisticos

# Formulacion de un modelo de programacion lineal
1. **Determinar las variables de decision**. respetar los elementos del sistema a modelar que son controlables. En los modelos estas variables toman valores numericos reales y se representan como $X_{1}, X_{2}, X_{3}...X_n$
2. **Determinar las restricciones** que son las limitaciones practicas de determinados recursos o imposiciones fisicas de la realidad. Se expresan como ecuaciones /inecuaciones lineales de las variables. Tienen la forma: 
	$$\begin{align}
	g: (x) \ge b_i; g_{i(x)} \le b_{i}; g_{i(x)} = b_i
	\end{align}$$
	$_i=1...m$ con $g_i$, funcion lineal 
	> se asignan al final Restriccion de no negatividad
3.  **Formulacion de funcion objetivo**: se trata de la funcion que mide la claidad de la solucion y que hay que optimizar. (es una funcion lineal), ejemplo:
	Maximizar o Minimizar
	$$\begin{align}
	Max X=Z=F(x); o Min Z=F(x)
	\end{align}$$
## Ejemplo 1
Una compañia dispone de *14 hrs diarias* de M. de obra para fabricar 2 productos $P_1$ y $P_2$. una unidad de $P_1$ requiere de 4 horas y para una unidad de $P_2$ se requiere 3. para la produccion se necesita una marteria prima de la que dispone 12 unidades diarias, 2 unidades por producto de $P_1$ y 3 unidades por producto para $P_2$

Que cantidad de c/producto maximiza la produccion?
### Solucion
##### Variables
$X_1$= cantidad de producto de $P_1$
$X_2$= cantidad de producto de $P_2$
##### Restricciones
Horas para producir $X_1$ y $X_2$ $\le$ hrs disponibles de M. de O.
Materia prima $X_1$ unidades y $X_2$ unidades unidad de M.P. disponible al dia

##### Funcion Objetivo (FO)
$Max: Z=X_{1}+X_{2}$
###### Matematicamente el modelo queda:
$Max: Z=X_{1}+X_{2}$ (FO)
Sujeto a:
$4X_{1}+3X_{2}\le14$
$2X_{1}+3X_{2}\le12$ 
$X_{1}+X_{2}\ge0$

## una empresa de juguetes fabrica pelotas y juegos de mesa , cada pelota produce  una utilidad  de $2 y cada juego una utilidad $4

- la fabricasion de una pelota require 4horas de la maquina A y 2  dela maquina B 
- la fabricasion de un jurgo ocupa  6 horas de las maquina B y 1  de la maquina c


las disponibilidadesde las maquinas son :
- 120 horas de la aquina A
- 74 horas de la maquina B
- 10 horas de la maquina C
se require maximazar  la utilidad, cuanto producir de cada producto?

| -          | pelotas | horas | FO $Z=X_{1}+X_{2}$     |
| ---------- | ------- | ----- | ---------------------- |
| horas A    | 4       | 6     | $2X_{1}+6X_{2}\le 120$ |
| horas B    | 2       | 6     | $2X_{1}+6X_{2}\le 72$  |
| horas C    | 0       | 1     | $X_{2}\le10$        |
| utilidades | 2       | 4     | $2X_{1}+4X_2\le0$   |




# problema

un estudiante de ingeniero  necesia completar  65 cursos 
 P/Graduarse el numero de cursos de 
 ingenieria  liene que ser mayor  o igual a
 23. el numero  de cursos  ajenos a ingenieria debe ser mayor o igual a 
 20.  el curso de ingenieria  promedio  requiere  un libro de texto  que cuesta  $60 e implica 120hrs. de estudio los cursos 
ajenos a ingenieria  requieren un libro  de texto que cuesta  $24, e implican 200hrs de estudios 
el estudiante dispone de $3000 de propuesto  p/libro 
¿con que conbinacion de cursos de ing. y ajenos 

minimizaria el numero 
total de horas de estudio ?
x= curso de ingenieria 
y=cursos ajenos a ingenieria 

se pide:
F.O. = $Z= 120x + 200y$
restriciones. 
$X+y=65$ 
$x\ge 23$
$y\ge20$
$60x+24y\le3000$

$$\begin{align}
x+y=65\\
65-y&\ge 23\\
\\
60(65-y)+24y\ge3000\\

\end{align}$$
![[Drawing 2023-09-09 12.10.41.excalidraw]]


- X = 40
- Y = 25

- s1 = 40 – 23 = 17
- s2 = 25 – 20 = 5


------
1. the Realy  big shos es un fabricante  de calzones de deportivo para basquetbol y futbol. El generente de marketing, ed sullivan, tiene que decirle  la mejor forma  de gastar los recursos  destinados a publicidad  cada unos delos quipsoo de fultbol  patonados requiere 120 pares  de zapatos. cada aquipo de basquqtbol require 32 pares zapatos. los  entrenadores de futbol reciben $300,000 por  concepto de patrocinio para calzodo , y los entrandores de basquetbol recibe $1,000,000
el presupuesto  de sullivan  para  promociones  ascinde a $30,000,000.
the  really  big shoe dispone  de una provision limitada(4 litros, o sea 4,000 centimetros cubicos) de flubber, un compuesto raro  y costoso que se utiliza  en la fabricacion del calzado atletico  de promocion. cada par de zapatos  de futbol 1 cc. sullivan  desea  patrocinar  el mayor numero  de quipos  de basquetbol y futbol que sus  recursos  le permitan.

a) formule un conjunto de ecuaciones lineales para describir  la funcion objetivo  y las  restriciones. 
b) utilice  el analisis grafico para encontrar  la solucion  visual.
c) ¿cual es el numero  maximo  de cada tipo  de quipo  que the really big shoe podra patrocinar?


solucion 1: 
a) el planteamiento del problema  de programacion lineal seria:


X= Numeros de equipos de futbol apatrocinar 
y = Números de equipos de basquetbol a patrocinar 

$$Z=Maximizar(x+y)$$

- presupuesto : $300,000x+1,000,000y\le30,000,000$
- Flubber: $120x+ 96y\le4000$
- No negatividad :$x,y\ge0$

curso nesesario para graduarse: X+y =65
cantidad  de cursos  de adminitracion: $X\ge23$	
cantidad  de cursos  ajenos a administración: $Y\ge20$ 
tiempo  total  de estudio: $120X + 200y\le12600$

$$x=23$$
$$y=42$$
$$z=2388$$
para la restricción sobre  la cantidad  de curso  ajenos  ala adminitracion  y  la variable de holgura alas  horas de estudio .

$adminitracion = 42- 20 = 5$
$horas de estudio = 12600-(120*23+200*42)=1440$
![[Pasted image 20230910220440.png]]

---
2. Mile-High Microbrewery fabrica una cerveza clara y una oscura. Mile-High dispone de una provisión limitada de cebada, tiene capacidad de embotellamiento limitada y un mercado también limitado para su cerveza clara. Las utilidades son de $0.20 por cada botella de cerveza clara y $0.50 por cada botella de cerveza oscura.

1. La siguiente tabla muestra la disponibilidad de recursos en la Mile-High Microbrewery. Aplique el método gráfico de programación lineal para maximizar las utilidades. ¿Cuántas botellas de cada producto deberán fabricarse cada mes?

| producto    |                      |                        |                                          |
| ----------- | -------------------- | ---------------------- | ---------------------------------------- |
| recursos    | cerveza clara($x_1$) | cerversa oscura($X_2$) | disponibilidades  de  recursos (por mes) |
| cebada      | 0.1 gramos           | 0.6 gramo              |       2,000 gramos      |
| embotellada | 1 botella            | 1 botella              |       6,000 botella     |
| mercado     | 1 botella            |    ---               |         4,000 botella     |

solución 
$X_1=$Número de botellas  de cerveza clara
$X_2=$ Numero de botellas de cerveza oscura  

$Z=$ Maximizar $(0.20X_1+0.50X_2)$

Restricciones:

cebada:$0.1X_1+0.6X_2\le2000$
embotellado:$X_1+X_2\le6000$
mercado: $X_1\le4000$

![[Pasted image 20230910220752.png]]
- x1 =3200
- x2 = 2800
- Z = 2040




---
El gerente de la planta de producción de un fabricante de tubos de plástico tiene la opción de utilizar dos rutas diferentes para la fabricación de un tipo de tubo de plástico en particular.

La ruta 1 utiliza la extrusora A y la ruta 2 utiliza la extrusora B. Ambas rutas requieren el mismo proceso de fusión. La siguiente tabla muestra los requisitos de tiempo y las capacidades de estos procesos.

![datos programación lineal problema 5](https://www.plandemejora.com/wp-content/uploads/image010.png)

Cada 100 pies de tubo procesado en la ruta 1 utilizan 5 libras de materias primas, mientras que cada 100 pies de tubo producidos en la ruta 2 utilizan solamente 4 libras. Esta diferencia es el resultado de las diferentes tasas de desperdicio de cada una de las máquinas de extrusión. En consecuencia, la utilidad por 100 pies de tubo procesados en la ruta 1 es de $60 y en la ruta 2 es de $80. Hay en total 200 libras de materias primas disponibles.

1. Formule un conjunto de ecuaciones lineales para describir la función objetivo y las restricciones.
2. Aplique el análisis gráfico para encontrar la solución visual.
3. ¿Cuál es la utilidad máxima?
### Solución 

**a)** El planteamiento para este ejemplo de programación lineal es:

**Variables:**

- x = Número de tubos de 100 pies procesados en la ruta 1
- y = Número de tubos de 100 pies procesados en la ruta 2

**Función Objetivo:**

_Z = Maximizar (60x + 80y)_

**Restricciones:**

- Fusión: _x + y ≤ 45_
- Extrusora A: _3x ≤ 90_
- Extrusora B: _y ≤ 160_
- Materia Prima: _5x + 4y ≤ **200_**




- La solución visual se encontraría en el punto B:

- x = 0
- y = 45


![[fabricante de tubos de plástico.excalidraw]]




una empresa victivinicola  ha adquirido  recientemente un terreno  nde 110 sectarias   debido  ala cantida  del sol  y el exelente  clima 
de al region, se puede vender  toda  la produccion  de unas sauvignon blanc y chardonnay.  se desea conocer cuanto plantar cada variedad   en las 110 hetarias, dado los constos beneficios netos requimintos  de mano de obra segun los datos que se muestra  continuacion:


| variable        | coste(us$) | beneficios neto | dias hombre |     |
| --------------- | ---------- | --------------- | ----------- | --- |
| sauvignon blanc | 100        |  50             |  10         |     |
|  chadonnay      |200         |       120       |  30         |     |

su pongamos que se posee un presupuesto de us$ 10,000 y una disponibilidad de 1,200 dias hombre durante el horizonte de planificacion formule y resuelva graficamente un modelo de programacion lineal para este problema. detalle claramente el dominio de soluciones factibles y el procedimiento utilizando para encontrar la solucion optima y valor optimo.

---

inventarios:
los inventarios los conocemos como: 
existen inventario de : 

materia prima 
producto en proceso
producto  terminado
producto en entrega 






las varibles a utilidades en el manejo de inventarios son:
inventario
inventarios
 cantidad o  demanda 
 costo de unitario
 rasto de pedir 
 costo de mantener 
 costo total 
 inventario promedio 
 numero de pedidos

----


## enfoque tabular 

entre método por  medio de una tabla nos da la medio de   una tabla nos  da la  cantidad option de pedido (donde económicamente nos conviene)


| c1 | c2 |c3 |
| --- | --- | ---- |
|     | --- | ---- |























