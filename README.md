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

### Capítulo 4: Divide-and-Conquer (Divide y vencerás)

Este capítulo se centra en uno de los enfoques más usados (y potentes) para diseñar algoritmos eficientes: el método de **divide y vencerás** (*divide-and-conquer*). Aunque ya se mencionó en capítulos anteriores (como en Merge Sort), aquí se analiza en más profundidad, incluyendo su análisis formal mediante **recurrencias**.

#### ¿En qué consiste?

La estrategia de divide y vencerás se basa en **tres pasos simples**:

1. **Dividir** el problema en varios subproblemas más pequeños.
2. **Conquistar**, es decir, resolver recursivamente cada subproblema.
3. **Combinar** las soluciones de los subproblemas en una solución global del problema original.

Este enfoque funciona especialmente bien cuando los subproblemas **son del mismo tipo que el problema original** (lo que permite aplicar recursión) y **no se solapan**, a diferencia de la programación dinámica.

#### Ejemplo típico: Merge Sort

Se utiliza como ejemplo recurrente para mostrar cómo aplicar divide y vencerás. El arreglo se divide en mitades, cada mitad se ordena recursivamente y luego se **fusionan** los resultados. Esto da como resultado un algoritmo con tiempo de ejecución:

$$
T(n) = 2T(n/2) + Θ(n)
$$

Lo cual se resuelve como:

$$
T(n) = Θ(n \log n)
$$

#### Cómo analizar algoritmos recursivos

El capítulo se enfoca mucho en cómo resolver **recurrencias**, que son ecuaciones que expresan el tiempo de ejecución de un algoritmo en términos de sí mismo.

Se presentan **tres técnicas principales** para resolver recurrencias:

##### 1. **Sustitución (por hipótesis inductiva)**

Supone una forma general para la solución y se prueba por inducción. Es poderosa, pero puede requerir algo de intuición para adivinar la forma correcta.

##### 2. **Árbol de recurrencia**

Se visualiza la ejecución recursiva como un árbol, y se suman los costos por nivel. Ayuda a entender cuántas operaciones se hacen en cada paso del proceso recursivo.

##### 3. **Teorema Maestro**

Esta es la herramienta más directa para casos comunes de divide y vencerás. Se aplica a recurrencias del tipo:

$$
T(n) = aT(n/b) + f(n)
$$

Donde:

* $a$: número de subproblemas
* $b$: tamaño al que se reduce cada subproblema
* $f(n)$: costo de dividir y combinar

El teorema da tres casos que permiten obtener rápidamente la cota asintótica sin tener que resolver todo paso a paso.

#### Otros algoritmos basados en divide and conquer

Además de Merge Sort, el capítulo muestra cómo este enfoque se aplica en otros problemas:

* **Multiplicación rápida de enteros grandes (Karatsuba)**
* **Máximo subarreglo** (para encontrar el mayor segmento contiguo en un arreglo)
* **Ordenación rápida (Quick Sort)** — aunque esta se analiza más adelante, también se basa en este principio

Divide and conquer no solo es una técnica eficiente, sino que también **organiza bien los problemas** al reducirlos a partes más pequeñas. Muchos de los algoritmos más importantes usan este enfoque porque, además de ser eficientes, son conceptualmente elegantes y fáciles de implementar con recursión. Saber resolver las recurrencias es clave para entender cómo se comportan estos algoritmos en términos de tiempo.



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

### Capítulo 6 - Subtema 6.4: Grafos: Caminos mínimos

En esta parte del capítulo se analiza un problema clásico dentro de los grafos: **encontrar el camino más corto** entre nodos. Es un problema súper común en la vida real, desde rutas de GPS hasta redes de comunicación o transmisión de datos.

#### ¿Qué es un camino mínimo?

Dado un **grafo con pesos en las aristas**, un camino mínimo entre dos vértices es la secuencia de aristas que conecta esos vértices con el **menor costo total posible** (donde “costo” puede ser distancia, tiempo, etc.).

#### ¿Qué algoritmo se usa?

El capítulo se enfoca principalmente en el **algoritmo de Dijkstra**, uno de los más famosos para resolver este tipo de problemas cuando **todos los pesos del grafo son positivos**.

#### ¿Cómo funciona Dijkstra?

* Parte desde un **nodo fuente** y va construyendo los caminos más cortos a todos los demás nodos.
* Utiliza una estructura de datos (normalmente una cola de prioridad) para **elegir siempre el nodo con menor costo conocido**.
* A medida que avanza, **actualiza los costos** de llegar a los vecinos de cada nodo.
* Cuando termina, tiene los **caminos más cortos desde el nodo origen a todos los demás**.

En resumen, **sigue una estrategia voraz**, porque en cada paso elige la opción “más barata” localmente.

#### ¿Por qué es voraz?

Dijkstra es un claro ejemplo de algoritmo voraz porque:

* Siempre elige el **camino aparentemente más corto** en el momento.
* No vuelve atrás ni reconsidera decisiones anteriores.
* Aprovecha la **propiedad de elección voraz** y la **subestructura óptima** del problema para garantizar que el camino encontrado es el óptimo.

#### Limitaciones

* **Solo funciona con pesos positivos.** Si hay aristas con pesos negativos, **Dijkstra puede fallar**, porque asume que una vez encontró el camino más corto a un nodo, no hay mejor opción.
* Para esos casos se usan otros algoritmos, como **Bellman-Ford** (aunque más lento).

#### Ejemplo de aplicación

El libro muestra un ejemplo donde se parte de un nodo y se actualizan los costos mínimos hacia los demás nodos paso a paso. En cada iteración se elige el nodo no visitado con menor costo acumulado.

<img width="646" height="470" alt="image" src="https://github.com/user-attachments/assets/ee8288ac-1faf-455e-a015-eb2123cb46ca" />

Este subtema nos muestra que los algoritmos voraces también pueden aplicarse en grafos, **siempre que se respeten ciertas condiciones**. Dijkstra es un ejemplo brillante de eficiencia y simplicidad, siempre que no haya pesos negativos. El algoritmo es práctico, usado en muchas áreas reales, y demuestra cómo la elección local más prometedora puede llevarnos a una solución global óptima.

### Capítulo 7: Divide y Vencerás

Este capítulo trata sobre una de las estrategias de diseño de algoritmos más conocidas y poderosas: **divide y vencerás** (*divide and conquer*). La idea es súper lógica, pero muy efectiva: **dividir el problema en subproblemas más pequeños, resolverlos por separado y luego combinar las soluciones** para obtener la solución final del problema original.

#### ¿Cómo funciona?

La estrategia de divide y vencerás se compone de tres pasos fundamentales:

1. **Dividir**: separar el problema en subproblemas más pequeños del mismo tipo.
2. **Vencer (resolver)**: resolver recursivamente cada subproblema.
3. **Combinar**: juntar las soluciones de los subproblemas para resolver el problema completo.

Esta técnica **es recursiva por naturaleza**, y por eso, muchas veces su análisis requiere trabajar con **recurrencias** para entender el tiempo de ejecución.

#### Ventajas de esta técnica

* Hace que problemas grandes se vuelvan más manejables.
* Aprovecha la recursión de forma natural.
* Permite desarrollar **algoritmos eficientes** que serían complejos con métodos iterativos.

#### Ejemplos clásicos

En el capítulo se explican varios ejemplos famosos donde divide y vencerás brilla:

* **Merge Sort**: divide el arreglo en dos mitades, ordena cada una por separado y luego las mezcla.
* **Quick Sort**: divide los elementos en los menores y mayores que un pivote, y luego ordena recursivamente cada parte.
* **Búsqueda binaria**: reduce el espacio de búsqueda a la mitad en cada paso.
* **Multiplicación rápida de enteros grandes**: como el algoritmo de Karatsuba, que reduce el número de multiplicaciones necesarias.

<img width="283" height="324" alt="image" src="https://github.com/user-attachments/assets/7bee228b-71b1-4953-86cf-26a89b94e066" />

*Ejemplo de algoritmo Merge Sort*

#### Análisis de eficiencia

Para analizar el costo de los algoritmos con divide y vencerás, se usan **recurrencias**, que describen el tiempo en función del tamaño del problema. Muchas veces se aplica el **Teorema Maestro** para resolver estas recurrencias fácilmente y obtener una cota asintótica.

Ejemplo:
En Merge Sort, el tiempo se expresa como:

```
T(n) = 2T(n/2) + Θ(n)
```

Que se resuelve como:

```
T(n) = Θ(n log n)
```

Esto demuestra que **divide y vencerás puede mejorar bastante el rendimiento** comparado con soluciones ingenuas (como el ordenamiento por inserción, que es Θ(n^2)).

El paradigma de divide y vencerás es una herramienta fundamental para resolver problemas complejos de forma eficiente. No solo ayuda a reducir el tamaño del problema paso a paso, sino que también permite escribir algoritmos más organizados y recursivos. Además, muchos de los algoritmos más rápidos y usados en la práctica (como Merge Sort y búsqueda binaria) **se basan en esta técnica**, por lo que entenderla es clave para cualquier estudiante de algoritmos.

### Capitulo 10: Algoritmos Probabilistas

En este capítulo se nos presenta una forma diferente (y a veces sorprendente) de resolver problemas usando algoritmos: los **algoritmos probabilistas**. A diferencia de los algoritmos tradicionales, que siempre siguen el mismo camino y dan el mismo resultado para una entrada, estos algoritmos **utilizan el azar o valores aleatorios en alguna parte de su ejecución**.

#### ¿Por qué usar el azar en algoritmos?

La idea puede parecer contraintuitiva al principio (¿por qué dejar que la computadora “tire los dados”?), pero el uso del azar puede tener varias **ventajas importantes**:

* Permite resolver ciertos problemas **más rápido** o de forma más sencilla.
* Evita peores casos que ocurren solo con ciertas entradas "malas".
* A veces, **no existe una solución determinista eficiente**, pero sí una aleatoria.

#### Tipos de algoritmos probabilistas

Los autores clasifican estos algoritmos en dos grandes categorías:

1. **Algoritmos de Monte Carlo**

   * Usan aleatoriedad y **pueden dar respuestas incorrectas** con cierta probabilidad.
   * Lo bueno es que **suelen ser muy rápidos**, y esa probabilidad de error se puede hacer muy baja si se repite el proceso.
   * Ejemplo típico: test de primalidad probabilista.

2. **Algoritmos de Las Vegas**

   * También usan azar, pero **nunca se equivocan**.
   * La diferencia es que su **tiempo de ejecución puede variar**, y a veces tardan más de lo esperado.
   * En otras palabras: **si dan una respuesta, es correcta**, pero no sabemos exactamente cuánto tardarán.

#### Ejemplos destacados del capítulo

El libro analiza algunos casos concretos donde los algoritmos probabilistas brillan:

* **Pruebas de primalidad**:
  Por ejemplo, el test de Miller-Rabin puede decir con mucha confianza si un número es primo, y es **más rápido** que los métodos deterministas clásicos.

* **Problemas de búsqueda y selección aleatoria**:
  A veces, seleccionar un elemento al azar o hacer una búsqueda con un poco de suerte puede ser más eficiente que analizar todos los casos.

#### Análisis de estos algoritmos

Cuando analizamos algoritmos probabilistas, no solo se mide el tiempo de ejecución en el peor caso, sino también en el **caso promedio** o la **esperanza matemática** del tiempo.

También se considera la **probabilidad de error** (en los de Monte Carlo), y cómo puede reducirse repitiendo el algoritmo múltiples veces.

Este tema nos abre la mente a otro enfoque para resolver problemas: no todo tiene que ser exacto y determinista. Usar **azar de forma controlada** puede ser una herramienta poderosa en el diseño de algoritmos, especialmente cuando buscamos soluciones rápidas o tratamos con problemas muy difíciles. Lo más importante es saber **cuándo y cómo** usar la aleatoriedad para que nos juegue a favor.












---
# Talleres - 1er Bimestre

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

---
# Talleres - 2do Bimestre
## 1. Prueba de Escitorio - Algoritmo Voraz

```java
import java.util.ArrayList;
import java.util.Arrays;
import java.util.Collections;
import java.util.List;

public class GreedyChange {

    /**
     * Da el cambio de n unidades utilizando el menor número posible de monedas.
     * La constante C especifica las monedas disponibles.
     *
     * @param n La cantidad total de cambio a devolver.
     * @return Una lista de enteros que representan las monedas utilizadas para dar el cambio,
     * o null si no se puede encontrar una solución.
     */
    public List<Integer> devolverCambio(int n) {
        // Monedas disponibles, ordenadas de mayor a menor para el algoritmo voraz
        final List<Integer> C = Arrays.asList(100, 25, 10, 5, 1); 

        List<Integer> S = new ArrayList<>(); // Contendrá la solución (monedas a devolver)
        int s = 0; // Suma de los elementos en S

        while (s != n) {
            int x = -1; // Almacenará la moneda seleccionada en esta iteración

            // Buscar el mayor elemento de C tal que s + x <= n
            for (int coin : C) {
                if (s + coin <= n) {
                    x = coin;
                    break; // Encontramos la moneda más grande que cumple la condición
                }
            }

            // Si no se encontró ninguna moneda que cumpla la condición, no hay solución
            if (x == -1) {
                return null; // "no encuentro la solución"
            }

            S.add(x); // Añadir la moneda seleccionada a la solución
            s += x;   // Actualizar la suma actual
        }

        return S; // Devolver la lista de monedas que conforman el cambio
    }
}
```
### Prueba de Escritorio - Caso 60 y 99 de cambio

<img width="657" height="443" alt="image" src="https://github.com/user-attachments/assets/f5aaef15-5ecc-4405-ba59-319c1c746249" />

## 2. Algoritmo de PRIM - Grafos

### Grafo no Dirigido

<img width="2701" height="3561" alt="image" src="https://github.com/user-attachments/assets/76c0f781-fb6b-4151-a381-72d957ac3b55" />

### Grafo Dirigido

<img width="2501" height="3650" alt="image" src="https://github.com/user-attachments/assets/ec6d1fc3-149f-480d-870a-3f6f35b6363f" />


## 3. Prueba de Escritorio - Merge Sort

<img width="484" height="634" alt="image" src="https://github.com/user-attachments/assets/6a2b1a2b-06b5-47cd-8968-310357ea3055" />

### Traduccion a Java

```java
public class OrdenamientoPorMezcla {

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
}
```

### Prueba de Escritorio - Lista [54,26,93,17,77,31,44,55,20]

<img width="1622" height="610" alt="image" src="https://github.com/user-attachments/assets/de891c79-2a6e-4ee2-82c0-5ef0f03f841a" />

<img width="1610" height="1631" alt="Sin título" src="https://github.com/user-attachments/assets/10680473-0964-4d44-94ff-9584982c2184" />

## 4. Prueba de Escritorio - Divide y Venceras
### 1er Algoritmo Busqueda Binaria 

```java
public static int BinRec(int[] T, int i, int j, int x) {
    if (i == j)
        return i;
    int k = (i + j) / 2;
    if (x <= T[k])
        return BinRec(T, i, k, x);
    else
        return BinRec(T, k + 1, j, x);
}

public static int BusquedaBin(int[] T, int x) {
    int n = T.length;
    if (n == 0 || x > T[n - 1])
        return n + 1;
    else
        return BinRec(T, 0, n, x);
}
```

### Prueba de Escritorio en tupla T = [8, 10, 14, 24, 28, 35, 49, 56, 98] / Buscar x = 14

<img width="1787" height="286" alt="image" src="https://github.com/user-attachments/assets/b549b485-76e7-4ba8-b6d4-bcf18d8e1e03" />

### 2do Algoritmo de Busqueda Binaria

```java
public static int BinIter(int[] T, int x) {
    int n = T.length;
    if (x > T[n - 1])
        return n + 1;

    int i = 0;
    int j = n;

    while (i < j) {
        int k = (i + j) / 2;
        if (x <= T[k])
            j = k;
        else
            i = k + 1;
    }
    return i;
}
```

### Prueba de Escritorio en tupla T = [8, 10, 14, 24, 28, 35, 49, 56, 98] / Buscar x = 14

<img width="1783" height="323" alt="image" src="https://github.com/user-attachments/assets/1ff5f086-cc63-4e90-a80b-76a5f9c61d1f" />

## 5. Prueba de Escritorio - Algoritmo QuickSort

```java
import java.util.Arrays;

public class QuickSort {

    // Umbral para usar Insertion Sort. Para arrays muy pequeños, es más eficiente.
    // Un valor común es entre 7 y 20.
    private static final int THRESHOLD = 7; 

    /**
     * Implementación del algoritmo Quicksort.
     * Ordena el sub-array T[i..j] por orden no decreciente.
     *
     * @param T El array de enteros.
     * @param i El índice inicial del sub-array.
     * @param j El índice final del sub-array.
     */
    public void quicksort(int[] T, int i, int j) {
        // Si el sub-array es lo suficientemente pequeño, usar un método de ordenación más simple (como Insertion Sort)
        // En Java, Arrays.sort() para sub-arrays es eficiente.
        if (j - i + 1 <= THRESHOLD) {
            Arrays.sort(T, i, j + 1); // El segundo argumento de Arrays.sort es exclusivo (j+1)
        } else {
            // Particionar el array y obtener la posición final del pivote
            int l = pivote(T, i, j);

            // Llamadas recursivas para los sub-arrays izquierdo y derecho
            quicksort(T, i, l - 1);
            quicksort(T, l + 1, j);
        }
    }

    /**
     * Permuta los elementos de la matriz T[i..j] alrededor de un pivote,
     * y proporciona un valor 'l' (la posición final del pivote 'p')
     * tal que:
     * - T[k] <= p para todo i <= k < l
     * - T[l] = p
     * - T[k] > p para todo l < k <= j
     * El valor inicial de 'p' es T[i].
     * Este método implementa una variación de la partición de Hoare.
     *
     * @param T El array de enteros.
     * @param i El índice inicial del sub-array.
     * @param j El índice final del sub-array.
     * @return El índice final del pivote después de la partición.
     */
    private int pivote(int[] T, int i, int j) {
        int p = T[i]; // El pivote es el primer elemento del sub-array
        int k = i;    // Puntero izquierdo
        int l = j;    // Puntero derecho (inicialmente j, no j+1 para evitar AIOOBE en el primer T[l])

        // Bucle principal de partición
        while (k < l) {
            // Mover 'k' hacia la derecha hasta encontrar un elemento mayor que el pivote
            // Asegurarse de que k no exceda los límites del sub-array o cruce l
            while (T[k] <= p && k < l) { // Nota: he ajustado la condición k < j a k < l para evitar posibles bucles infinitos
                                         // o accesos fuera de rango si k = j y T[j] <= p.
                                         // El pseudocódigo original es un poco ambiguo aquí.
                k++;
            }
            // Mover 'l' hacia la izquierda hasta encontrar un elemento menor o igual que el pivote
            while (T[l] > p) { // Aquí no necesitamos l > k porque el while principal (k < l) lo controla
                l--;
            }

            // Si los punteros no se han cruzado, intercambiar los elementos
            if (k < l) {
                intercambiar(T, k, l);
                // Después del intercambio, avanza k y l para continuar la búsqueda
                // (esto es un detalle de algunas implementaciones de Hoare, no estrictamente en el pseudo original,
                // pero asegura progreso si T[k] o T[l] son iguales al pivote)
                // Aunque el pseudocódigo original tiene 'repetir k <- k+1 hasta que T[k] > p' etc. DENTRO
                // del 'mientras k < l', lo que puede ser redundante o llevar a un doble avance si no se maneja bien.
                // Mi implementación simplifica esto al dejar los avances dentro de los bucles 'while' de escaneo.
            }
        }
        
        // Final: Ahora que k >= l (punteros cruzados o encontrados), el elemento en T[l] es el lugar para el pivote
        // Intercambiar el pivote original (que está en T[i]) con el elemento en T[l]
        intercambiar(T, i, l); 
        
        return l; // 'l' es la posición final del pivote
    }

    /**
     * Método auxiliar para intercambiar dos elementos en un array.
     * @param T El array.
     * @param idx1 Índice del primer elemento.
     * @param idx2 Índice del segundo elemento.
     */
    private void intercambiar(int[] T, int idx1, int idx2) {
        int temp = T[idx1];
        T[idx1] = T[idx2];
        T[idx2] = temp;
    }
}
```

### Prueba de Escritorio - Array [3,1,4,1,5,9,2]

<img width="1271" height="884" alt="image" src="https://github.com/user-attachments/assets/ce7d4222-6011-42ac-9d0c-e58772094278" />

## 6. Generación de Pseudoaleatorios
### Enunciado
Desarrollar un generador pseudoaleatorio utilizando el método congruencial lineal, programado en Java. A partir de dicho generador deberán:
1. Implementar el algoritmo con los siguientes parámetros:
   <img width="652" height="294" alt="image" src="https://github.com/user-attachments/assets/4a647c95-cab9-4f98-8dec-3458aecc66af" />
2. Generar una secuencia de 100 números normalizados en el intervalo [0,1).
3. Mostrar los primeros 10 valores generados.

### Codigo en Java

```java
package generaddorpseudoaleatorio;

/**
 *
 * @author Byron Alvarez
 */
public class GeneradorPseudoaleatorio {

    private long a; // Multiplicador
    private long c; // Constante aditiva
    private long m; // Módulo (2^32)
    private long semilla; // Semilla inicial (X0)
    private long ultimoValorGenerado; // Almacena el último valor generado (Xn)

    /**
     * Constructor del generador pseudoaleatorio.
     * @param semilla La semilla inicial (X0) para comenzar la generación.
     */
    public GeneradorPseudoaleatorio(long semilla) {
        this.a = 1664525L;
        this.c = 1013904223L;
        // El módulo 2^32 es 1L << 32.
        // Como los resultados de (aXn + c) pueden exceder Long.MAX_VALUE si no se maneja bien,
        // la operación de módulo implícita de Java para long numbers (que es 2^64) no es lo que necesitamos.
        // Para simular módulo 2^32 con tipos long en Java, podemos usar un & (m-1) si m es una potencia de 2,
        // o simplemente permitir que la operación de overflow de long maneje el módulo si lo deseamos,
        // pero la forma más segura es manejarlo explícitamente o usar BigInteger si los números se hacen muy grandes.
        // Sin embargo, para 2^32, los números se ajustarán bien dentro de un 'long' de Java.
        // La operación de módulo de Java (%) funciona con números negativos también, pero aquí siempre esperamos positivos.
        // Para simular (Xn+1) = (a*Xn + c) mod 2^32 correctamente con longs, podemos simplemente hacer el casting a int
        // y luego a long de nuevo, porque los int son de 32 bits y su overflow se comporta como mod 2^32.
        // O más explícitamente, para asegurarse de que el módulo sea 2^32 y no 2^64 (implícito de long):
        this.m = 1L << 32; // Equivale a 2 elevado a la potencia de 32

        // Aseguramos que la semilla esté dentro del rango [0, m-1]
        this.semilla = semilla % m;
        if (this.semilla < 0) { // Si la semilla inicial es negativa
            this.semilla += m;
        }
        this.ultimoValorGenerado = this.semilla;
    }

    /**
     * Genera el siguiente número pseudoaleatorio en la secuencia.
     * La fórmula utilizada es: X_{n+1} = (aX_n + c) mod m
     * Se usa un truco con int para manejar el módulo 2^32 eficientemente.
     * Las operaciones con 'long' se comportan de manera que el resultado es 64 bits.
     * Pero queremos un resultado de 32 bits módulo 2^32.
     * Castear a 'int' truncará el valor a 32 bits, logrando el efecto de mod 2^32.
     * Después se vuelve a castear a 'long' para que el método devuelva un 'long'.
     *
     * Nota: Si 'aXn + c' excede el rango de un 'int' antes del truncamiento, esto puede
     * introducir un comportamiento no deseado si no se entiende cómo Java maneja esto.
     * Sin embargo, para los valores dados (a, c, y Xn siendo de 32 bits), el producto
     * aXn puede exceder los 32 bits, pero la suma aXn + c aún cabe dentro de un long.
     * Al hacer el casting a int, el overflow del int maneja el módulo 2^32 automáticamente.
     *
     * Ejemplo: (1L << 31) + (1L << 31) - 1 + 1013904223L * 1664525L
     * podría ser un número muy grande. Sin embargo, (a*Xn + c)
     * se calcula como un long, y luego (int) para truncar a 32 bits.
     *
     * Una forma más explícita y segura para valores muy grandes sería usar BigInteger.
     * Pero para 2^32, el truco de int es comúnmente usado y efectivo.
     *
     * Otra forma de manejar el módulo 2^32 con long sin BigInteger:
     * `(a * ultimoValorGenerado + c) & (m - 1)`
     * esto funciona cuando m es una potencia de 2. m - 1 es un número con todos los bits bajos en 1.
     * Para m = 2^32, m-1 es 0x00000000FFFFFFFFL. Un AND con esto efectivamente trunca a 32 bits.
     * Usaré esta técnica ya que es más directa y robusta.
     */
    public long generarSiguiente() {
        // Calcula el siguiente valor utilizando la fórmula del LCG
        // La operación (a * ultimoValorGenerado + c) puede exceder el rango de un long de 64 bits si a y Xn son muy grandes.
        // Pero en nuestro caso, 2^32 es el módulo, por lo que los valores de Xn siempre serán menores que 2^32.
        // a y c son también números que caben en 32 bits.
        // El producto de dos números de 32 bits puede ser de hasta 64 bits, por lo que el resultado cabe en un 'long'.
        // Usamos el operador & (bitwise AND) con (m-1) para simular la operación de módulo cuando m es una potencia de 2.
        // Esto es equivalente a (a * ultimoValorGenerado + c) % m, pero más eficiente para potencias de 2.
        ultimoValorGenerado = (a * ultimoValorGenerado + c) & (m - 1);
        return ultimoValorGenerado;
    }

    /**
     * Normaliza un número pseudoaleatorio generado (que está en el rango [0, m-1])
     * al intervalo [0, 1).
     * @param valorPseudoaleatorio El número entero generado por el LCG.
     * @return El número normalizado en el intervalo [0, 1).
     */
    public double normalizar(long valorPseudoaleatorio) {
        // Casting a double antes de la división para asegurar una división de punto flotante
        return (double) valorPseudoaleatorio / m;
    }

    public static void main(String[] args) {
        // 1. Implementar el algoritmo con los parámetros dados:
        long semillaInicial = 12345; // número arbitrario como 12345.
        System.out.println("Semilla inicial (X0): " + semillaInicial);

        GeneradorPseudoaleatorio generador = new GeneradorPseudoaleatorio(semillaInicial);

        // 2. Generar una secuencia de 100 números normalizados en el intervalo [0,1].
        System.out.println("\nGenerando 100 números pseudoaleatorios normalizados:");
        double[] secuenciaNormalizada = new double[100];
        for (int i = 0; i < 100; i++) {
            long valorBruto = generador.generarSiguiente();
            secuenciaNormalizada[i] = generador.normalizar(valorBruto);
        }

        // 3. Mostrar los primeros 10 valores generados.
        System.out.println("\nPrimeros 10 valores normalizados generados:");
        for (int i = 0; i < 10; i++) {
            System.out.println("Valor #" + (i + 1) + ": " + secuenciaNormalizada[i]);
        }
    }
}
```

### Salida / Resultado del Programa (Semilla inicial: 12345)

<img width="771" height="345" alt="image" src="https://github.com/user-attachments/assets/fd7c15e3-df7c-4008-a563-29830ff298ae" />

### Analizar la distribucion

<img width="1094" height="420" alt="image" src="https://github.com/user-attachments/assets/cc5e9f4f-2a5c-410a-bf77-1b24bf66e211" />

Responder:

**✴ ¿La distribución es aproximadamente uniforme?**

| **Intervalo** | **Cantidad** |
| ------------- | ------------ |
| \[0.0, 0.2)   | 20           |
| \[0.2, 0.4)   | 18           |
| \[0.4, 0.6)   | 21           |
| \[0.6, 0.8)   | 22           |
| \[0.8, 1.0)   | 19           |

**Sí**, los valores se distribuyen de manera bastante uniforme entre los 5 intervalos definidos, lo cual es característico de un buen generador congruencial lineal.

**✴ ¿Qué efecto tiene cambiar la semilla?**

Cambiar la semilla modifica completamente la secuencia generada. Sin embargo, la forma de la distribución (uniforme) se mantiene si el generador está bien implementado.

## 7. Aplicación encontrar el árbol de recubrimiento mínimo a partir de un grafo no dirigido (Algoritmo de Prim)
### Código Java con interfaz gráfica
```java
package algoritmosgrafos;

/**
 *
 * @author bvalv
 */
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;
import java.util.Arrays;

public class AlgoritmoPrim extends JFrame {

    private int vertices;
    private int[][] graph;
    private JTextArea logArea;
    private JPanel graphPanel;
    private JTextField verticesField;
    private JButton generateButton, runButton;
    private Point[] nodePositions; // Posiciones de los nodos
    private int[] parent;          // Para MST

    public AlgoritmoPrim() {
        setTitle("Algoritmo de Prim - Árbol de Recubrimiento Mínimo");
        setSize(800, 600);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(new BorderLayout());

        // Panel superior: entrada
        JPanel topPanel = new JPanel();
        topPanel.add(new JLabel("Número de vértices:"));
        verticesField = new JTextField(5);
        topPanel.add(verticesField);
        generateButton = new JButton("Generar Grafo Aleatorio");
        runButton = new JButton("Ejecutar Prim");
        topPanel.add(generateButton);
        topPanel.add(runButton);
        add(topPanel, BorderLayout.NORTH);

        // Panel central: dibujo del grafo
        graphPanel = new JPanel() {
            @Override
            protected void paintComponent(Graphics g) {
                super.paintComponent(g);
                if (graph != null) drawGraph(g);
            }
        };
        graphPanel.setBackground(Color.WHITE);
        add(graphPanel, BorderLayout.CENTER);

        // Panel inferior: área de logs
        logArea = new JTextArea(10, 50);
        logArea.setEditable(false);
        JScrollPane scroll = new JScrollPane(logArea);
        add(scroll, BorderLayout.SOUTH);

        // Listeners
        generateButton.addActionListener(e -> generateGraph());
        runButton.addActionListener(e -> runPrim());

        setVisible(true);
    }

    // Generar un grafo aleatorio
    private void generateGraph() {
        try {
            vertices = Integer.parseInt(verticesField.getText());
            graph = new int[vertices][vertices];
            nodePositions = new Point[vertices];

            // Generar posiciones circulares de nodos
            int radius = Math.min(graphPanel.getWidth(), graphPanel.getHeight()) / 2 - 50;
            int centerX = graphPanel.getWidth() / 2;
            int centerY = graphPanel.getHeight() / 2;
            for (int i = 0; i < vertices; i++) {
                double angle = 2 * Math.PI * i / vertices;
                int x = centerX + (int) (radius * Math.cos(angle));
                int y = centerY + (int) (radius * Math.sin(angle));
                nodePositions[i] = new Point(x, y);
            }

            // Llenar matriz con pesos aleatorios
            for (int i = 0; i < vertices; i++) {
                for (int j = i + 1; j < vertices; j++) {
                    if (Math.random() < 0.6) { // 60% probabilidad de arista
                        int weight = 1 + (int) (Math.random() * 20);
                        graph[i][j] = weight;
                        graph[j][i] = weight;
                    }
                }
            }

            logArea.setText("Grafo generado aleatoriamente.\n");
            repaint();
        } catch (NumberFormatException ex) {
            JOptionPane.showMessageDialog(this, "Ingrese un número válido de vértices.", "Error", JOptionPane.ERROR_MESSAGE);
        }
    }

    // Dibujar grafo
    private void drawGraph(Graphics g) {
        g.setFont(new Font("Arial", Font.BOLD, 14));
        // Dibujar aristas
        for (int i = 0; i < vertices; i++) {
            for (int j = i + 1; j < vertices; j++) {
                if (graph[i][j] != 0) {
                    g.setColor(Color.GRAY);
                    g.drawLine(nodePositions[i].x, nodePositions[i].y, nodePositions[j].x, nodePositions[j].y);
                    // Peso en el medio
                    int midX = (nodePositions[i].x + nodePositions[j].x) / 2;
                    int midY = (nodePositions[i].y + nodePositions[j].y) / 2;
                    g.setColor(Color.BLACK);
                    g.drawString(String.valueOf(graph[i][j]), midX, midY);
                }
            }
        }
        // Dibujar aristas del MST (si existen)
        if (parent != null) {
            g.setColor(Color.RED);
            for (int i = 1; i < vertices; i++) {
                if (parent[i] != -1) {
                    g.drawLine(nodePositions[i].x, nodePositions[i].y, nodePositions[parent[i]].x, nodePositions[parent[i]].y);
                }
            }
        }
        // Dibujar nodos
        for (int i = 0; i < vertices; i++) {
            g.setColor(Color.CYAN);
            g.fillOval(nodePositions[i].x - 20, nodePositions[i].y - 20, 40, 40);
            g.setColor(Color.BLACK);
            g.drawOval(nodePositions[i].x - 20, nodePositions[i].y - 20, 40, 40);
            g.drawString(String.valueOf(i), nodePositions[i].x - 5, nodePositions[i].y + 5);
        }
    }

    // Ejecutar Prim y mostrar pasos
    private void runPrim() {
        if (graph == null) {
            JOptionPane.showMessageDialog(this, "Primero genere un grafo.", "Error", JOptionPane.ERROR_MESSAGE);
            return;
        }
        parent = new int[vertices];
        int[] key = new int[vertices];
        boolean[] mstSet = new boolean[vertices];

        Arrays.fill(key, Integer.MAX_VALUE);
        Arrays.fill(mstSet, false);
        parent[0] = -1;
        key[0] = 0;

        logArea.append("\nEjecución del Algoritmo de Prim:\n");
        for (int count = 0; count < vertices - 1; count++) {
            int u = minKey(key, mstSet);
            mstSet[u] = true;

            logArea.append("\nIteración " + (count + 1) + ": Vértice agregado = " + u + "\n");
            logArea.append("Claves actuales: " + Arrays.toString(key) + "\n");
            logArea.append("Vertices en MST: " + Arrays.toString(mstSet) + "\n");

            for (int v = 0; v < vertices; v++) {
                if (graph[u][v] != 0 && !mstSet[v] && graph[u][v] < key[v]) {
                    parent[v] = u;
                    key[v] = graph[u][v];
                }
            }
            repaint();
            try { Thread.sleep(500); } catch (InterruptedException e) {}
        }

        int total = 0;
        logArea.append("\nÁrbol de Recubrimiento Mínimo:\n");
        for (int i = 1; i < vertices; i++) {
            logArea.append(parent[i] + " - " + i + " (Peso: " + graph[i][parent[i]] + ")\n");
            total += graph[i][parent[i]];
        }
        logArea.append("Peso total: " + total + "\n");

        repaint();
    }

    // Obtener el índice del vértice con clave mínima
    private int minKey(int[] key, boolean[] mstSet) {
        int min = Integer.MAX_VALUE, minIndex = -1;
        for (int v = 0; v < vertices; v++) {
            if (!mstSet[v] && key[v] < min) {
                min = key[v];
                minIndex = v;
            }
        }
        return minIndex;
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(AlgoritmoPrim::new);
    }
}
```

### Ejemplo de Ejecución

Nosotros como usuarios ingresamos en la parte superior la cantidad de vértices que deseamos que se generen en nuestro gráfo, damos clic en "GENERAR GRAFO ALEATORIO" y la aplicación se encarga de generar un gráfo con la cantidad de vértices especificados, con caminos y pesos aleatorios, se puede dar clic al botón las veces que guste hasta tener un grafo a nuestro gusto; al tener el grafo que prefiramos, damos clic en "EJECUTAR PRIM" y la app se encarga de realizar el algoritmo de Prim, resalta en el gráfo dibujado el camino, y nos da el árbol de recubrimiento mínimo con su peso total  

<img width="1455" height="971" alt="image" src="https://github.com/user-attachments/assets/2a27c77e-7e54-4a48-b26a-6f7d50deda51" />

