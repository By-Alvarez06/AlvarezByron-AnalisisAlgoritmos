# Alvarez Byron - Análisis Algoritmos
Repositorio de la materia Análisis de Algoritmos - 4to Ciclo "B"

# Resúmenes
## Libro: Introduction to Algorithms. Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest, Clifford Stein
### Capítulo 1: The Role of Algorithms in Computing

El capítulo 1 nos provee una descripción general de los algoritmos y cómo podemos encontrarlos en los sistemas modernos computacionales. Se busca partir con bases para una
buena introducción al libro y a los temas que se verán, por lo tanto, tal como define el nombre del capítulo, nos define qué es un algoritmo junto con unos ejemplos para un 
mejor aprendizaje y su rol en la computación.

#### 1.1 Algoritmos

El libro nos define el concepto principal del capítulo, los algoritmos, de la siguiente forma: "Informalmente, un **algoritmo** es cualquier proceso computacional bien definido 
que toma algun **valor**, o conjunto de valores, como **entrada** y produce algún valor, o a su vez, un conjunto de valores, como **salida** en una cantidad de tiempo finita".

Por lo tanto, en términos simples, podemos entender al algoritmo como la secuencia de pasos computacionales que toma valores de entrada, para convertirlos y devolver unos valores 
de salida.

Los algoritmos sirven como herramientas para los problemas computacionales, debido a que describen un proceso específico a seguir para, con valores de entrada, generar valores de 
salida y conseguir esa relación de valores que da solución al problema.

Un ejemplo claro de esto es precisamente el que nos provee el libro:

![image](https://github.com/user-attachments/assets/5cd1f3fa-d34e-42d9-8152-36e7bae46338)

*Imagen de ejemplo de valores de entrada y salida de un problema*

Supongamos que debemos ordenar una secuencia de números de manera ascendente, la manera en que un algoritmo trabajaría sería:
- Input o Entrada: Secuencia *n* de números
- Output o Salida: Una permutación o ordenamiento de la secuencia dada como entrada, de tal manera que quede ordenado como solicita el problema

En consecuencia, si damos la secuencia de entrada: (5,7,1,3,4,6,9,8,2), un algoritmo de permutación correcto daría como salida una secuencia como: (1,2,3,4,5,6,7,8,9). Una 
secuencia de entrada como la del problema, se denomina **instancia**. Una instancia de un problema consiste en la entrada (que satisface cualquier regla o necesidad que 
impone el problema) necesario para calcular la solución al problema.

Un algoritmo para un problema computacional es **correcto** si, para cada instancia que se provee para el problema, se detiene (es decir, finaliza el proceso de cálculo en un 
periodo finito de tiempo) y da como salida la solución del problema. Un algoritmo correcto **soluciona** el problema computacional dado. Un algoritmo incorrecto podría no terminar 
siempre con todas las instancias dadas, o podría terminar con una respuesta incorrecta. Contrario a lo que se piensa, algoritmos incorrectos pueden ser útiles a veces, si se 
controla el rango de error.

Además, los algoritmos son de gran importancia ya que pueden dar solución a una gran cantidad de problemas, y pueden tener muchas aplicaciones prácticas como:
- Problemas biológicos como el Proyecto Genoma Humano que requieren el análisis del ADN y su almacenamiento en bases de datos y generar herramientas para el análisis de los mismos.
- Manipulación de grandes volúmenes de datos en internet (encontrar rutas con información de viajes, motores de búsqueda que permitan rápidamente encontrar páginas con información específica).
- Algoritmos numéricos para gestionar privacidad de información en compras en línea.

Otro concepto clave es usar las apropiadas estructuras de datos, es una parte importante del diseño de los algoritmos. Una **estructura de datos** es una manera de almacenar y 
organizar datos de manera que facilite el acceso y modificación de estos.

#### 1.2 Algoritmos como una tecnología

El subtema nos presenta una introducción de la importancia de implementar algoritmos que nos permitan optimizar los recursos disponibles de la mejor manera posible, y dando a 
su vez solución a los problemas computacionales. Entre los recursos más importantes tenemos el tiempo y la memoria, refiriendose a que deben ser eficientes en consumo de tiempo 
de ejecución y la cantidad de memoria a usar en la ejecución de algoritmos de manera que sea eficiente.

***Eficiencia***

Diferentes algoritmos diseñados para solucionar un mismo problema a menudo suelen diferir drásticamente en su eficiencia. Estas diferencias pueden ser mucho más significantes 
que las diferencias debido a hardware o software.

***Algoritmos y otras tecnologías***

El desempeño del sistema total de un computador depende de escoger algoritmos eficientes tanto como escoger hardware rápido. Tan rápido como se estan dando avances en tecnológas 
computacionales, se estan dando avances en algoritmos. Los algoritmos tienen una gran importancia en la computación contemporanea en procesos como:
- Arquitecturas de computadores avanzados y tecnologías de fabricación
- Interfaces gráficas de usuario, intuitivas y fáciles de usar (GUIs)

### Capítulo 2: Getting Started
#### 2.1 Insertion sort

En este capítulo, inicia con una introducción a los algoritmos que conoceremos y se nos especifica como estos se nos explicarán en un pseudocódigo el cual será bastante fácil 
de entender debido a nuestros conocimientos sobre computación y programación. ¿Qué separa al pseudocódigo del código real?: la diferencia radica en que, en pseudocódigo, 
empleamos cualquier expresión que sea necesaria para expresar un método de la forma más clara y concisa.

El algoritmo de **Orden por Insercion** (Insertion sort) soluciona el problema de ordenar una secuencia *n* de números. Estos números se los conoce también como **llaves**

![image](https://github.com/user-attachments/assets/b65854b6-fc45-4f81-97b8-5eac7a7fae8d)

*Ejemplo de inserción con cartas*

El ejemplo que nos brinda el libro es un método de inserción en el cual se toman cartas con la mano derecha de una baraja, para colocarlas de manera ascendente en la otra mano, es decir, que con cada carta que se tome del mazo, se hace una comparación con las cartas que ya se posee en la otra mano. Dándonos así un pseudocódigo el cual compara, por cada iteración, que la carta o el número anterior sea menor que el posterior, sino, se realiza el ordenamiento y la permutación de estos. Como se puede observa en la siguiente imagen en la que se tiene una lista de números (5, 2, 4, 6, 1, 3).

![image](https://github.com/user-attachments/assets/d88e4973-6101-4fd8-a65d-04c5624282c3)

*Imagen de muestra del proceso de permutación*

#### 2.2 Analyzing algorithms

**Analizar** un algoritmo se refiere a predecir la cantidad de recursos que este requerirá, considerando aspectos como memoria, ancho de banda o consumo de energia.
Se usa el modelo **RAM** (Random Access Machine), donde cada operación básica (suma, comparación, acceso a memoria) toma una cantidad constante de tiempo. Y para determinar la 
cantidad de recursos, se toman en consideración puntos importantes como:
- El tiempo de ejecución depende del tamaño de la entrada.
- Se busca una expresión matemática que relacione el tamaño de la entrada *n* con el número de operaciones realizadas.

Además se nos presenta una notación asíntota, ya que para analizar un algoritmo es preferente tomar en cuenta el peor escenario, en lugar del escenario promedio o el mejor escenario:
- O-notation: Límite superior ("no peor que").
- Ω-notation: Límite inferior ("no mejor que").
- Θ-notation: Límite ajustado ("exactamente del orden de").

Y al analizar el *insertion sort* podemos sacar la conclusión de que es eficiente para entradas pequeñas o casi ordenadas, pero ineficiente para *n* grande.

#### 2.3 Designing algorithms

El capítulo nos da una introducción a los métodos y diferentes proceso existentes para diseñar un algoritmo. Hay una amplia gama de métodos para diseñar algoritmos, por ejemplo, 
*Insertion Sort* usa el método incremental: inserta cada nuevo elemento en su lugar dentro de un subarreglo previamente ordenado.

*Introducción al método divide y vencerás (divide-and-conquer):*
Esta técnica permite diseñar algoritmos mucho más eficientes en el peor caso que el método incremental, además, su análisis suele ser más sencillo. Muchos algoritmos útiles 
son recursivos: resuelven un problema grande dividiéndolo en varios subproblemas más pequeños (similares al original), resolviéndolos recursivamente y combinando sus soluciones.

Este proceso cuenta de tres partes o tres pasos a tomar en cuenta:
- Dividir: Partir el problema en subproblemas más pequeños.
- Conquistar: Resolver los subproblemas (normalmente de manera recursiva).
- Combinar: Unir las soluciones de los subproblemas para formar la solución del problema original.

### Capítulo 3: Caracterizando los Tiempos de Ejecución (Characterizing Running Times)

Este capítulo profundiza en cómo podemos describir de forma más precisa y útil el tiempo que tarda un algoritmo en ejecutarse. En capítulos anteriores vimos cómo calcular tiempos exactos (como con Insertion Sort), pero aquí nos enfocamos en algo más general: el **crecimiento del tiempo de ejecución** cuando la entrada se vuelve muy grande. Este enfoque se conoce como **eficiencia asintótica**.

#### ¿Por qué importa esto?

Cuando trabajamos con algoritmos que van a procesar entradas grandes (que es lo más común en la vida real), no nos interesa tanto saber cuántas operaciones hace exactamente, sino **cómo crece ese número en relación al tamaño de la entrada**. Por ejemplo, sabemos que Merge Sort es más rápido que Insertion Sort en entradas grandes, porque su tiempo de ejecución crece como $n \log n$ y no como $n^2$.

---

#### 3.1 Notaciones O, Ω y Θ

Aquí se introducen tres notaciones súper importantes para hablar del crecimiento de funciones:

* **O-grande (O)**: Da una *cota superior*, es decir, el algoritmo no toma más tiempo que eso (en el peor caso).
* **Ω-grande (Ω)**: Es una *cota inferior*, nos dice que al menos ese tiempo va a tomar (en el mejor caso).
* **Θ (Theta)**: Cuando ambas anteriores se cumplen, es una *cota ajustada*. O sea, sabemos que el algoritmo se comporta así en todos los casos, sin desviarse mucho.

Estas notaciones son clave para comparar algoritmos sin tener que meternos en cuentas complicadas ni fijarnos en los detalles como las constantes o términos de menor orden.

---

#### 3.2 Definiciones formales

Después de explicarlas de forma intuitiva, se pasa a dar definiciones matemáticas más precisas. Esto es útil si se quiere demostrar con rigor que un algoritmo es $O(n^2)$ o $Θ(n \log n)$, por ejemplo. También se muestran propiedades como reflexividad, simetría y transposición, que ayudan a manipular expresiones con estas notaciones.

---

#### 3.3 Notaciones estándar y funciones comunes

Finalmente, el capítulo revisa **funciones que aparecen seguido en el análisis de algoritmos**, como:

* Polinomios ($n$, $n^2$, etc.)
* Logaritmos ($\log n$, $\log \log n$)
* Exponenciales ($2^n$)
* Factoriales ($n!$)
* Otras funciones menos comunes, pero útiles en análisis avanzados.

También se exploran conceptos matemáticos básicos como suelos y techos (floor y ceiling), aritmética modular, y propiedades de funciones iteradas.

**En resumen**, este capítulo nos da las herramientas para hablar el "idioma matemático" del análisis de algoritmos. Aprendemos a ignorar detalles poco relevantes y a enfocarnos en lo que realmente importa: cómo escala un algoritmo cuando la entrada crece.


---
## Libro: Fundamentos de algoritmia. Brassard, G. & Bratley, P. (2000).
### Capítulo 1: Preliminares

#### 1.1 Introducción

El capítulo introductorio del libro establece los fundamentos conceptuales y metodológicos para el estudio de algoritmos. En primer lugar, define los términos algoritmos 
(procedimientos sistemáticos para resolver problemas) y algoritmia (ciencia que los estudia), ilustrándolos con ejemplos prácticos como técnicas de multiplicación. Destaca que 
incluso tareas cotidianas esconden complejidades algorítmicas, y justifica la relevancia de su estudio por su utilidad e interés teórico-práctico.

#### 1.2 ¿Qué es un algoritmo?

El capítulo inicia con la definición que los autores tienen de algoritmo: "Un algoritmo, nombre que proviene del matemático persa del siglo IX *alKhowarizmi*, es sencillamente 
un conjunto de reglas para efectuar algún cálculo, bien sea a mano o, más frecuentemente, en una máquina." Nos presentan la idea de que un algoritmo, por lo general, no debe 
implicar decisiones subjetivas, como en el caso de recetas al decir "a su gusto", "hasta estar medio hecho", ya que de ser el caso, no se podría llamar algoritmo.

Se nos dice además que no todos los algortimos siguen un mismo propósito, debido a la cantidad de escenarios o problemas, se pueden dar **algoritmos probabilistas** o, en el caso 
de algoritmos matemáticos, se busca que el algoritmo dé una respuesta que sea tan precisa según el usuario requiera (cantidad de dígitos de precisión). En otros casos, cuando no 
se tiene un algoritmo práctico definido para un problema, se lleva a cabo un procedimiento basado fundamentalmente en el optimismo y frecuentemente con un apoyo teórico mínimo, es 
decir, tratar de dar una aproximación de la respuesta correcta en un tiempo razonable; a este proceso se lo denomina **algoritmo heurístico**. La *diferencia entre los algoritmos 
aproximados y la heurística*: con los primeros podemos especificar el error que estamos dispuestos a aceptar, con la segunda no podemos controlar el error, pero quizá seamos capaces 
de estimar su magnitud.

Por otro lado, nos muestran la importancia de, al momento de buscar resolver un problema, seleccionar el algoritmo que mejor se adapte a las prioridades; tales como: menor tiempo 
de ejecución posible, menor uso de espacio, más fácil de programar, entre otros. Y aquí es donde conocemos el concepto de ***Algoritmia*** como la ciencia que nos permite evaluar 
el efecto de estos diferentes factores externos (prioridades o limitaciones del equipo) sobre los algoritmos disponibles; también es la ciencia que nos indica la forma de diseñar 
un nuevo algoritmo para una tarea concreta.

**Ejemplos del libro de distintos algorítmos aritmético**

![image](https://github.com/user-attachments/assets/e1ddd236-45b7-4c81-af17-5f962fa85f08)

*Ejemplo de diferencia entre multiplicación americana e inglesa*

![image](https://github.com/user-attachments/assets/e2a031ae-757b-4812-81b3-6b8b542eb4fa)

*Ejemplo de multiplicación a la russe*

![image](https://github.com/user-attachments/assets/e0a554b4-edd0-4b3a-987a-5d58c5780cf1)

*Ejemplo de método de multiplicación mediante divide y vencerás*

En el caso de todos estos métodos de multiplicación, todos cumplen un mismo propósito: brindar la respuesta al producto de dos número, su diferencia radica en la manera de 
realizarlo, el proceso, los pasos y por supuesto su enfoque prioritario. 

Los métodos americano e inglés o "algoritmo clásico" no presentan mucha diferencia, el método *"a la russe"* requiere de un proceso más repetitivo; para la primera columna de 
divisiones enteras para 2, y la segunda columna sumas sucesivas de si mismo, tomando unicamente los términos impares de la primera columna y se suman los números de la columna 
derecha de los términos tomados. O por otro lado, el método divide y vencerás, poco común pero que busca realizar más operaciones, con menor cantidad de dígitos, sin embargo, 
es el más veloz para ejecutar en una computadora siempre que los números a multiplicar sean lo suficientemente grandes.



### Capítulo 2: Algoritmia elemental
