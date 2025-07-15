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

---

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

---

### Capítulo 3: Caracterizando los Tiempos de Ejecución (Characterizing Running Times)

Este capítulo profundiza en cómo podemos describir de forma más precisa y útil el tiempo que tarda un algoritmo en ejecutarse. En capítulos anteriores vimos cómo calcular tiempos exactos (como con Insertion Sort), pero aquí nos enfocamos en algo más general: el **crecimiento del tiempo de ejecución** cuando la entrada se vuelve muy grande. Este enfoque se conoce como **eficiencia asintótica**.

#### ¿Por qué importa esto?

Cuando trabajamos con algoritmos que van a procesar entradas grandes (que es lo más común en la vida real), no nos interesa tanto saber cuántas operaciones hace exactamente, sino **cómo crece ese número en relación al tamaño de la entrada**. Por ejemplo, sabemos que Merge Sort es más rápido que Insertion Sort en entradas grandes, porque su tiempo de ejecución crece como $n \log n$ y no como $n^2$.

#### 3.1 Notaciones O, Ω y Θ

Aquí se introducen tres notaciones súper importantes para hablar del crecimiento de funciones:

* **O-grande (O)**: Da una *cota superior*, es decir, el algoritmo no toma más tiempo que eso (en el peor caso).
* **Ω-grande (Ω)**: Es una *cota inferior*, nos dice que al menos ese tiempo va a tomar (en el mejor caso).
* **Θ (Theta)**: Cuando ambas anteriores se cumplen, es una *cota ajustada*. O sea, sabemos que el algoritmo se comporta así en todos los casos, sin desviarse mucho.

Estas notaciones son clave para comparar algoritmos sin tener que meternos en cuentas complicadas ni fijarnos en los detalles como las constantes o términos de menor orden.

#### 3.2 Definiciones formales

Después de explicarlas de forma intuitiva, se pasa a dar definiciones matemáticas más precisas. Esto es útil si se quiere demostrar con rigor que un algoritmo es $O(n^2)$ o $Θ(n \log n)$, por ejemplo. También se muestran propiedades como reflexividad, simetría y transposición, que ayudan a manipular expresiones con estas notaciones.

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
## Libro: Fundamentos de algoritmia. Brassard, G. & Bratley, P. (2006).
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

---
### Capítulo 2: Algoritmia elemental

Este capítulo es clave para comenzar a pensar como alguien que realmente diseña algoritmos, no solo los aplica. Nos introduce al análisis de eficiencia, es decir, cómo medir cuán "bueno" o rápido es un algoritmo cuando lo ejecutamos con diferentes tamaños de entrada. No basta con que un algoritmo funcione, también queremos que sea lo más eficiente posible, sobre todo cuando la entrada crece mucho.

#### ¿Por qué necesitamos analizar algoritmos?

Imaginemos dos algoritmos que hacen lo mismo, pero uno se tarda minutos y el otro horas cuando les das muchos datos. ¿Cuál preferirías usar? Exacto. El análisis de algoritmos nos permite predecir estos comportamientos y elegir el mejor.

#### Modelos de costo y unidades de medida

Los autores explican que para analizar el tiempo de un algoritmo, se necesita contar el número de operaciones "básicas" que hace, como sumas, comparaciones o accesos a arreglos. Para eso, se define un modelo simplificado (como el modelo RAM) donde cada operación cuesta lo mismo.

También se menciona que no siempre se mide solo el tiempo: a veces importa también el **espacio**, o sea, cuánta memoria usa el algoritmo.

#### Casos: mejor, peor y promedio

El capítulo distingue entre distintos escenarios:

* **Mejor caso**: cuando el algoritmo tiene suerte y resuelve el problema rapidísimo.
* **Peor caso**: cuando se enfrenta a los datos más difíciles.
* **Caso promedio**: lo que normalmente esperaríamos.

Pero ojo: aunque el promedio suena más útil, muchas veces analizamos el **peor caso**, porque nos da una garantía mínima de rendimiento (como pensar en lo peor que podría pasar).

#### Análisis empírico vs. teórico

También se habla de la diferencia entre:

* **Medir** el tiempo con un cronómetro (análisis empírico), lo cual puede variar dependiendo del computador, compilador, etc.
* **Estimar** el comportamiento con fórmulas matemáticas (análisis teórico), que es más general y no depende del equipo.

Este capítulo nos deja una idea súper importante: el diseño de algoritmos no se trata solo de que "funcionen", sino de que sean eficientes, sobre todo cuando enfrentan entradas muy grandes. También nos da las herramientas básicas para empezar a analizar algoritmos y comparar su rendimiento en diferentes situaciones.

---
### Capítulo 3: Notación Asintótica

Este capítulo nos enseña a hablar el idioma universal del análisis de algoritmos: la notación asintótica. Básicamente, es una forma matemática de describir cómo crece el tiempo (o espacio) que usa un algoritmo a medida que aumentamos el tamaño de los datos de entrada. No nos interesa tanto saber cuántas instrucciones exactas se ejecutan, sino cómo se comporta ese número cuando el problema se hace gigante.

#### ¿Por qué usamos notación asintótica?

Porque no queremos depender de detalles como:

* El lenguaje de programación
* El hardware
* El compilador

Queremos comparar algoritmos en abstracto, y para eso nos enfocamos en lo que más influye: el crecimiento.

Ejemplo: No es lo mismo un algoritmo que crece como $n^2$ que uno que crece como $n \log n$. Cuando $n$ es pequeño no se nota mucho, pero cuando es grande, la diferencia es brutal.

#### Las tres notaciones clave

1. **O-grande** (también llamada "cota superior"):
   Se usa para decir que el tiempo de ejecución no crece más rápido que una cierta función.
   Es decir, el algoritmo es como mucho tan lento como eso.
   Ejemplo: Si decimos que algo es $O(n^2)$, puede que a veces funcione más rápido, pero nunca será peor que eso (para valores grandes de $n$).

2. **Ω-grande** (cota inferior):
   Esta nos dice que el algoritmo al menos necesita ese tiempo.
   O sea, no va a ser más rápido que eso en general.

3. **Θ (Theta)**:
   Es la notación más precisa.
   Significa que el algoritmo tiene exactamente ese crecimiento, ni más ni menos (salvo constantes y detalles menores).
   Cuando algo es $Θ(n \log n)$, eso es lo que realmente podemos esperar, sin sorpresas.

#### Ejemplos útiles

* **$O(1)$** → Tiempo constante: no importa cuánto crezca el input.
* **$O(\log n)$** → Crecimiento muy lento, ideal.
* **$O(n)$** → Tiempo lineal, súper razonable.
* **$O(n^2)$** → Empieza a doler en inputs grandes.
* **$O(2^n)$** → Básicamente impracticable si $n$ es mayor que 30–40.

#### ¿Cómo usar esta notación?

El capítulo también muestra cómo podemos usar estas notaciones para **comparar algoritmos**, ignorando los detalles que no afectan el crecimiento (como multiplicar por 10 o sumar 50).

También da reglas útiles:

* Podemos ignorar constantes.
* Podemos ignorar términos de menor orden.

Por ejemplo, si una función es $5n^2 + 3n + 10$, su notación asintótica es simplemente $Θ(n^2)$.

Este capítulo es fundamental para poder analizar algoritmos como verdaderos profesionales. Aprendemos a abstraer lo que realmente importa: cómo escala el algoritmo cuando los problemas se hacen grandes. Saber usar O, Ω y Θ te da el poder de comparar algoritmos sin necesidad de correrlos, solo con matemática y lógica.

---
### Capítulo 4.2 Análisis de las estructuras de control

En este apartado, los autores se enfocan en cómo analizar el **tiempo de ejecución** de las **estructuras básicas de control** que usamos en la mayoría de los algoritmos, como los condicionales y los bucles. La idea es ver cómo afectan estas estructuras al comportamiento general del algoritmo, sobre todo en términos del crecimiento de tiempo cuando la entrada aumenta.

#### Instrucciones simples

Primero, se parte con lo más básico: una **instrucción elemental** (como una suma, una asignación, una comparación) se considera que tiene un **costo constante**. Es decir, si un algoritmo hace 5 sumas, eso cuesta 5 unidades de tiempo.

#### Estructuras condicionales (if/else)

Cuando tenemos algo como:

```c
if (condición) {
   instrucción A;
} else {
   instrucción B;
}
```

El análisis se basa en el **peor caso**. Eso significa que, aunque tal vez una de las ramas se ejecute más seguido que la otra, asumimos que se puede ejecutar **la rama más costosa** para tener una garantía sólida del rendimiento.

#### Bucles (for, while)

Esta parte es clave. El análisis de un bucle depende de cuántas veces se repite el cuerpo del bucle y qué tan costoso es lo que hay dentro.

Por ejemplo:

```c
for (i = 1; i <= n; i++) {
   hacerAlgoConstante();
}
```

Este bucle tiene un **costo total de $Θ(n)$** porque ejecuta una operación constante $n$ veces.

Si dentro del bucle hay otro bucle:

```c
for (i = 1; i <= n; i++) {
   for (j = 1; j <= n; j++) {
      hacerAlgoConstante();
   }
}
```

Entonces el costo total es **$Θ(n^2)$** porque cada una de las $n$ iteraciones del bucle externo ejecuta $n$ operaciones más del bucle interno.

También se mencionan bucles en los que el número de repeticiones **no es lineal**, como cuando se va dividiendo algo por dos (caso típico de algoritmos como la búsqueda binaria), y ahí el costo tiende a ser **logarítmico** $Θ(\log n)$.

#### Secuencias de instrucciones

Cuando un algoritmo tiene varias instrucciones o bloques en secuencia (uno después del otro), el costo total es la **suma de los costos** de cada parte. Pero para el análisis asintótico, nos quedamos con el **mayor crecimiento** (el término dominante), ignorando los menores.

Ejemplo:

```c
bloque A → Θ(n)
bloque B → Θ(n^2)
→ Total: Θ(n^2)
```

Este tema nos enseña que para analizar el tiempo de un algoritmo no hay que medir cada línea como si estuviéramos programando en una hoja de cálculo. En lugar de eso, analizamos bloques completos usando el comportamiento de las estructuras de control. Esto nos permite estimar con claridad cómo escalará nuestro algoritmo cuando los datos de entrada sean cada vez más grandes.

### Capítulo 6: Algoritmos Voraces

En este capítulo se nos introduce una nueva estrategia de diseño de algoritmos llamada voraz (o greedy en inglés). La idea principal es bastante intuitiva: en cada paso del algoritmo, se toma la decisión que parece ser la mejor en ese momento, sin preocuparse por si eso nos lleva a una solución global óptima o no. O sea, el algoritmo actúa como si estuviera diciendo: “tomo lo que más me conviene ahora”.

#### ¿Cómo funcionan los algoritmos voraces?

Un algoritmo voraz construye la solución paso a paso, eligiendo en cada etapa un elemento que parece el mejor localmente, con la esperanza de que eso conduzca a una solución global óptima.

Pero ojo: no siempre funcionan para todos los problemas. Para que un algoritmo voraz sea correcto, se deben cumplir ciertas condiciones específicas en el problema que se está resolviendo.

#### Características clave
Para que un problema se pueda resolver correctamente con un algoritmo voraz, normalmente debe cumplir dos propiedades importantes:

1. Subestructura óptima:
   Esto significa que una solución óptima del problema completo contiene dentro de sí soluciones óptimas a subproblemas. Es como decir que si partes la solución en pedazos, esos pedazos también deben ser lo mejor posible.

2. Propiedad de elección voraz:
   Significa que es seguro elegir la mejor opción local en cada paso sin arruinar la solución final. Si esta propiedad no se cumple, el algoritmo puede llevarnos a una solución incorrecta.

#### Ejemplos clásicos que sí funcionan
- Cambio de monedas (cuando las denominaciones son "buenas")
- Árbol de expansión mínima (algoritmo de Prim y Kruskal)
- Codificación de Huffman
- Problema del intervalo máximo sin traslape

En todos estos, aplicar una estrategia voraz sí lleva a una solución óptima.

#### Contraste con programación dinámica

A diferencia de la programación dinámica, que también trabaja con subproblemas, los algoritmos voraces no revisan todas las combinaciones posibles ni almacenan resultados anteriores. Son más rápidos y sencillos, pero solo se pueden usar si las condiciones del problema lo permiten.

#### Ventajas y desventajas
**Ventajas:**

- Son más simples de implementar.
- Consumen menos memoria (no necesitan tablas como la programación dinámica).
- Suelen ser más rápidos en la práctica.

**Desventajas:**

- No garantizan la solución óptima en todos los problemas.
- Se requiere análisis riguroso para comprobar su validez.

Los algoritmos voraces son una herramienta poderosa cuando se puede aplicar correctamente. Este capítulo nos muestra que pensar de forma “codiciosa” puede ser una gran estrategia, pero también que no debemos confiar ciegamente: hay que demostrar que la estrategia funciona. En los próximos capítulos se analizan casos donde sí y donde no funciona este enfoque.










---
# Talleres

## Taller 1 - Comparación de Funciones Asintóticas

Este taller tiene como objetivo aplicar las definiciones de la notación **O-grande** (cota superior) para comparar el crecimiento de funciones. Resolveremos dos ejercicios principales.

### **Parte 1**

Dadas las funciones:

* $f(n) = n^3 + 9n^2 \log n$
* $g(n) = n^2 \log n$

Comprobar que $f(n) \in O(g(n))$ y Comprobar que $f(n) \notin O(n^2)$

#### 1. Comparación entre $f(n)$ y $g(n)$:

* Dividimos $f(n)$ entre $g(n)$:

  ![image](https://github.com/user-attachments/assets/34e11f6c-4cf8-40e9-acb5-6b4520ab7bb1)

* Simplificando:

  ![image](https://github.com/user-attachments/assets/01433e01-b6cb-4839-b0ae-83fb9eccf843)

* Como $\frac{n}{\log n} \to \infty$ cuando $n \to \infty$, eso implica que:

  ![image](https://github.com/user-attachments/assets/28c9ef89-1c88-4635-8434-371aef99a5c4)

**Resultado**:
- **$f(n) \notin O(g(n))$**
- **$f(n) \in \Omega(g(n))$** (ya que f(n) crece estrictamente más rápido)

#### 2. Comprobación de que $f(n) \notin O(n^2)$:

* Consideramos el término dominante de $f(n)$: $n^3$
* Claramente, $n^3 \gg n^2$ cuando $n \to \infty$
* Esto implica que:

  ![image](https://github.com/user-attachments/assets/40267bb0-e1be-486c-bcdf-66496fbc7d91)

> **Resultado**:
> ❌ **$f(n) \notin O(n^2)$**

### **Parte 2**

Dadas las funciones:

* $f(n) = 2^n$
* $g(n) = 2^{2n} = (2^n)^2$

Queremos determinar:

* $f(n) \in O(g(n))$
* $g(n) \in O(f(n))$

Sabemos que:

$$
2^n < 2^{2n} = (2^n)^2
\Rightarrow \frac{f(n)}{g(n)} = \frac{2^n}{2^{2n}} = 2^{-n} \to 0
$$

Esto implica que:

* $f(n) \in O(g(n))$ ✅
* $g(n) \notin O(f(n))$ ❌ (porque la razón tiende a infinito)

> **Resultado**:
>
> * ✅ **$f(n) \in O(g(n))$**
> * ❌ **$g(n) \notin O(f(n))$**
> * ✅ Además, $f(n) \in o(g(n))$, es decir, crece *mucho* más lento

### Conclusión General

| Funciones comparadas                             | Relación O-grande                          |
| ------------------------------------------------ | ------------------------------------------ |
| $f(n) = n^3 + 9n^2 \log n$ y $g(n) = n^2 \log n$ | ❌ $f(n) \notin O(g(n))$                    |
| $f(n) = n^3 + 9n^2 \log n$ y $n^2$               | ❌ $f(n) \notin O(n^2)$                     |
| $f(n) = 2^n$, $g(n) = 2^{2n}$                    | ✅ $f(n) \in O(g(n))$, ❌ $g(n) \in O(f(n))$ |

---
## Taller 2 - Análisis del Algoritmo de Fibonacci

Este taller tiene como objetivo analizar el comportamiento de un algoritmo recursivo clásico: el cálculo de la sucesión de **Fibonacci**. Aplicaremos técnicas de análisis de algoritmos, incluyendo el uso de recurrencias y su resolución.

### 1. Algoritmo de Fibonacci (versión recursiva)

```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)
```

### 2. Identificación de la recurrencia

El algoritmo hace **dos llamadas recursivas** en cada paso (excepto en los casos base). Por lo tanto, el **tiempo de ejecución T(n)** puede modelarse como:

```
T(n) = T(n - 1) + T(n - 2) + Θ(1)
```

Esto representa el costo de hacer dos llamadas recursivas más el trabajo adicional (suma y comparación), que consideramos de **tiempo constante Θ(1)**.

### 3. Obtención de la ecuación general

Para obtener una solución general a esta recurrencia, ignoramos el término constante y analizamos la forma homogénea:

```
T(n) = T(n - 1) + T(n - 2)
```

Esta es una **recurrencia lineal de segundo orden**, idéntica a la definición matemática de los números de Fibonacci. Se puede resolver usando técnicas algebraicas, como asumir una solución de la forma:

```
T(n) = a^n
```

Sustituyendo en la ecuación:

```
a^n = a^(n-1) + a^(n-2)
→ a^n = a^(n-1)(1 + 1/a)
→ a^2 = a + 1
```

Esto nos lleva a resolver la ecuación característica:

```
a^2 - a - 1 = 0
```

Soluciones:

```
a₁ = (1 + √5)/2 ≈ 1.618... (φ, número áureo)
a₂ = (1 - √5)/2 ≈ -0.618...
```

Entonces, la **solución general** de la recurrencia es:

```
T(n) = A · a₁^n + B · a₂^n
```

Donde A y B se determinan según las condiciones iniciales, pero para el análisis asintótico nos quedamos con el **término dominante**:

```
T(n) = Θ(φ^n)
```

Esto significa que el algoritmo crece **exponencialmente** con respecto a `n`.

### 4. Demostración por sustitución (cota inferior)

Queremos probar que:

```
T(n) ≥ c · φ^n  (para alguna constante c > 0)
```

**Hipótesis inductiva**:
Supongamos que para todo `k < n`, se cumple que `T(k) ≥ c · φ^k`.

**Paso inductivo**:

```
T(n) = T(n-1) + T(n-2)
     ≥ c · φ^(n-1) + c · φ^(n-2)
     = c · (φ^(n-1) + φ^(n-2))
     = c · φ^n        (por definición de φ: φ^n = φ^(n-1) + φ^(n-2))
```

Esto demuestra que:

```
T(n) = Ω(φ^n)
```

Como también demostramos previamente que `T(n) = O(φ^n)`, concluimos que:

```
T(n) = Θ(φ^n)
```

### Conclusión

El algoritmo recursivo de Fibonacci es **exponencialmente ineficiente**, con un tiempo de ejecución de:

```
Θ(φ^n), donde φ ≈ 1.618
```

Esto lo convierte en un mal candidato para cálculos grandes, a menos que se optimice con **memorización o programación dinámica**.

---
## Taller 3 - Prueba de Escritorio Algoritmo Burbuja

![image](https://github.com/user-attachments/assets/cbe7bafd-323c-4ff3-bd63-01013d0c5cef)

### Prueba de escritorio del algoritmo de ordenamiento en base al arreglo **[6-8-3-4-1]**

| N | I | J | A[J-1] | A[J] | If(A[J-1]>A[J]) | A[J-1] | A[J] |
|---|---|---|--------|------|------------------|--------|------|
| 5 | 1 | 5 | 4      | 1    | TRUE             | 1      | 4    |
| 5 | 1 | 4 | 3      | 1    | TRUE             | 1      | 3    |
| 5 | 1 | 3 | 8      | 1    | TRUE             | 1      | 8    |
| 5 | 1 | 2 | 6      | 1    | TRUE             | 1      | 6    |
| 5 | 2 | 5 | 3      | 4    | FALSE            |        |      |
| 5 | 2 | 4 | 8      | 3    | TRUE             | 3      | 8    |
| 5 | 2 | 3 | 6      | 3    | TRUE             | 3      | 6    |
| 5 | 3 | 5 | 8      | 4    | TRUE             | 4      | 8    |
| 5 | 3 | 4 | 6      | 4    | TRUE             | 4      | 6    |
| 5 | 4 | 5 | 6      | 8    | FALSE            |        |      |
|   |   |   |        |      | **TERMINA EL PROCESO** |        |      |

### Progeso y cambio del arreglo durante el algoritmo

| N° de Iteración | Arreglo |
|---|---|
| 1 | 6-8-3-4-1 |
| 2 | 6-8-3-**1-4** |
| 3 | 6-8-**1-3**-4 |
| 4 | 6-**1-8**-3-4 |
| 5 | **1-6**-8-3-4 |
| 6 | 1-6-**3-8**-4 |
| 7 | 1-**3-6**-8-4 | 
| 8 | 1-3-6-**4-8** | 
| 9 | 1-3-**4-6**-8 |
|   | FIN - Arreglo Ordenado |

## Taller 4 - Traducción de un algoritmo a Java

### Algoritmo de ordenamiento Merge Sort

```
MERGE(A, p, q, r)
1  nL = q - p + 1  // longitud de A[p..q]
2  nR = r - q      // longitud de A[q+1..r]
3  let L[0..nL-1] y R[0..nR-1] sean nuevos arreglos
4  for i = 0 to nL-1
5      L[i] = A[p + i]
6  for j = 0 to nR-1
7      R[j] = A[q + j + 1]
8  i = 0          // i indexa el elemento restante más pequeño en L
9  j = 0          // j indexa el elemento restante más pequeño en R
10 k = p           // k indexa la posición en A para llenar
11 // Mientras cada uno de los arreglos L y R contengan un elemento sin fusionar,
12 // copia el elemento sin fusionar más pequeño de vuelta en A[p..r].
13 while i < nL and j < nR
14     if L[i] <= R[j]
15         A[k] = L[i]
16         i = i + 1
17     else A[k] = R[j]
18     k = k + 1
19 // Cuando un arreglo se queda sin elementos,
20 // copia el resto del otro arreglo de vuelta en A.
21 while i < nL
22     A[k] = L[i]
23     i = i + 1
24     k = k + 1
25 while j < nR
26     A[k] = R[j]
27     j = j + 1
28     k = k + 1
```

### Algoritmo en Java

```Java
public class MergeSort {

    /**
     * Combina dos sub-arreglos ordenados en un único arreglo ordenado.
     * Este método es un componente central del algoritmo de Ordenamiento por Mezcla (Merge Sort).
     *
     * @param A El arreglo original que contiene los sub-arreglos a ser combinados.
     * @param p El índice inicial del primer sub-arreglo (L).
     * @param q El índice final del primer sub-arreglo (L).
     * @param r El índice final del segundo sub-arreglo (R).
     */
    public static void mezclar(int[] A, int p, int q, int r) {
        // Calcular las longitudes de los dos sub-arreglos
        int nL = q - p + 1; // Longitud de A[p...q]
        int nR = r - q;     // Longitud de A[q+1...r]

        // Crear nuevos arreglos temporales L y R
        int[] L = new int[nL];
        int[] R = new int[nR];

        // Copiar elementos de A a L
        for (int i = 0; i < nL; i++) {
            L[i] = A[p + i];
        }

        // Copiar elementos de A a R
        for (int j = 0; j < nR; j++) {
            R[j] = A[q + 1 + j];
        }

        // Inicializar índices para L, R y el arreglo combinado A
        int i = 0; // i indexa el elemento más pequeño restante en L
        int j = 0; // j indexa el elemento más pequeño restante en R
        int k = p; // k indexa la ubicación en A a rellenar

        // Mientras cada uno de los arreglos L y R contenga un elemento sin combinar,
        // copiar el elemento sin combinar más pequeño de vuelta en A[p...r]
        while (i < nL && j < nR) {
            if (L[i] <= R[j]) {
                A[k] = L[i];
                i = i + 1;
            } else {
                A[k] = R[j];
                j = j + 1;
            }
            k = k + 1;
        }

        // Copiar cualquier elemento restante de L (si R se agotó)
        while (i < nL) {
            A[k] = L[i];
            i = i + 1;
            k = k + 1;
        }

        // Copiar cualquier elemento restante de R (si L se agotó)
        while (j < nR) {
            A[k] = R[j];
            j = j + 1;
            k = k + 1;
        }
    }

    // Ejemplo de uso (opcional, para propósitos de prueba)
    public static void main(String[] args) {
        // int[] arr1 = {2, 5, 8, 1, 3, 7}; // Arreglo de ejemplo donde se usaría la mezcla
        // Para demostrar la mezcla, necesitamos un arreglo parcialmente ordenado
        // Creemos uno directamente:
        int[] arr2 = {1, 3, 5, 2, 4, 6}; // Mezclando {1,3,5} y {2,4,6}

        System.out.println("Arreglo original para la demostración de mezcla:");
        imprimirArreglo(arr2);

        // Aquí, p=0, q=2, r=5 (mezclando A[0..2] y A[3..5])
        mezclar(arr2, 0, 2, 5);

        System.out.println("Arreglo después de la mezcla:");
        imprimirArreglo(arr2);

        int[] arr3 = {10, 20, 30, 5, 15, 25, 35};
        System.out.println("\nArreglo original para otra demostración de mezcla:");
        imprimirArreglo(arr3);
        mezclar(arr3, 0, 2, 6);
        System.out.println("Arreglo después de la mezcla:");
        imprimirArreglo(arr3);
    }

    public static void imprimirArreglo(int[] arr) {
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }
}
```
