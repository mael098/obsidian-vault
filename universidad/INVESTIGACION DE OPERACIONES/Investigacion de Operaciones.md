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



resolver por  metodos  graficos  

graficar
conbinacion mejor 



