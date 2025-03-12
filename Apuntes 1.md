# Apuntes Dinamica de sistemas 1 corte
### Rincon Benavides Juan Esteban
# Dinámica de sistemas 
## Sistema 
Sistema está definido como la combinación de componentes que al actuar conjuntamente alcanzan un objetivo específico la combinación de los mismos se puede representar por medio de reglas y principios simples que relacionan las salidas con las entradas del sistema esto se puede representar con un diagrama muy sencillo

[![image.png](https://i.postimg.cc/DfNFvLkd/image.png)](https://postimg.cc/xqLBgkdc)

## Sistema dinámico 
un sistema dinámico tiene por nombre ese ya que su salida en el presente depende de una entrada en el pasado ya que actúa a través del tiempo dando como resultado  el mismo tipo de entrada a la salida, por otro lado dejaría de ser un sistema dinámico en el caso que su salida en curso dependa únicamente de la entrada en curso a ese sistema se le conoce como estático

[![image.png](https://i.postimg.cc/hvkH98ck/image.png)](https://postimg.cc/SYGT4MXd)

## Planta y proceso
Estos 2 conceptos nos definen parte de lo físico que nos permita llevar a cabo un proceso ya que van de la mano tanto planta como proceso puede ser representado matemáticamente y puede ser también representado a través de uno o varios sisistemas ya que con esto podemos ver la secuencia de pasos que permite el desarrollo o fabricación de un objetivo o producto esto es muy utilizado en el área de control como sinónimo de desarrollo o proceso 

## Modelos dinámicos 
en los modelos dinámicos lo que nos interesa en el tema de control es que allá una ecuación matemática que relacione las variables de interés con respecto al tiempo $f(t)$

Teniendo esto también debemos tener en cuenta que es necesario cuantificar cuánto cambian las variables de interés con respecto al tiempo para ello la función que más nos representa y se utilizará para el análisis de este tipo de modelos serán las derivadas

$$\frac{df(t)}{dt}$$

## Como lucen los modelos de ecuaciones diferenciales 
Los modelos de ecuaciones diferenciales lucen de la siguiente manera son combinaciones lineales de derivadas con diferente orden siendo el grado uno del menor y así sucesivamente tienen un orden específico con unas constantes como podemos ver a continuación

$$a_1 \frac{d^2 F}{dt^2} + a_2 \frac{dF}{dt} + a_3 F = u(t)$$

Dónde F es la salida del sistema, U es la entrada del sistema dependiente del tiempo y la solución por lo general no es un número es una función dependiente también del tiempo

## Características de una ecuación diferencial 
Hay muchas características que definen a las ecuaciones diferenciales para ello veremos los casos más comunes y usados
### Ecuación lineal invariante en el tiempo
$$\frac{d^2x(t)}{dt^2} + 5 \frac{dx(t)}{dt} + 10x(t) = 0$$
### Ecuación lineal variante en el tiempo
$$\frac{d^2x(t)}{dt^2} + (1 - \cos(2t)) x(t) = 0$$
### Ecuación no lineal variante en el tiempo
$$\frac{d^2x(t)}{dt^2} + (x^2(t) - 1) \frac{dx(t)}{dt} + x(t) = 0$$
### Ecuación no lineal invariante en el tiempo
$$\frac{d^2x(t)}{dt^2} + \frac{dx(t)}{dt} + x(t) + x^3(t) = sen(\omega t)$$

## Influencia de parámetros 
Según el sistema dinámico aunque nos encontremos tendremos y veremos una influencia en los parámetros del mismo así como diferentes comportamientos en este caso se analizará un comportamiento en el cual un sistema dinámico de masa resorte se deja oscilando libremente teniendo una onda sinusoidal sin prácticamente pérdidas

[![image.png](https://i.postimg.cc/sDFWBB57/image.png)](https://postimg.cc/xqR8h1x1)

Otra influencia puede ser si digamos el sistema está sumergido o tiene condiciones las cuales lo frenen en este caso es un líquido con una densidad muy grande la cual hace que el movimiento en este caso se ralentice bastante teniendo como resultado un decaimiento exponencial

[![image.png](https://i.postimg.cc/xd7CW7RM/image.png)](https://postimg.cc/v1rbn0CZ)

O a diferencia de los otros 2 podremos ver que siempre las condiciones van a ser diferentes en este caso bueno ver líquidos ciudades medias las cuales nos permitan ver una combinación entre ambas viendo impulso bastante grande al principio y terminando con una oscilación más pequeña hasta un punto final

[![image.png](https://i.postimg.cc/W4QN9ZN7/image.png)](https://postimg.cc/SXfbRJzX)

## Transformada de Laplace
Ya que los sistemas dinámicos representan una complejidad a la hora de resolverse es necesario en ocasiones pasar del dominio del tiempo al dominio de la plaza esto con el fin de facilitar las operaciones resultantes de cada sistema hola continuación se representa cómo lo siguiente

$$\mathbf{x(t)} \rightarrow \mathbf{X(s)}$$

$$X(s) = \int_{0}^{\infty} x(t) \cdot e^{-s t} dt$$

$$s = \alpha + j\omega$$

Algunas de sus propiedades son las siguientes esto con el fin de que sea algo medianamente estandarizado para la solución

[![image.png](https://i.postimg.cc/QMPQ0fKn/image.png)](https://postimg.cc/TyV5Pq9r)

## Tipos de entrada para un sistema
### Escalón unitario
este tipo de entrada es una de las más comunes pues no entiende a variar sino más que todo en su principio a la hora de activarse o podemos ver de un tiempo cero y un tiempo inicial en el cual comienza la subida siendo sus valores de cero para cuando t es menor a cero y uno para cuando t es mayor a cero

[![image.png](https://i.postimg.cc/L4kP19DW/image.png)](https://postimg.cc/MXTXk8h0)
### Rampa 
Para este tipo de entrada lo que observamos es una entrada tipo rampa la cual como su nombre lo indica tiene la forma de una rampa está dependerá hola de su pendiente y del valor el cual este definía hoy representación es la siguiente

[![image.png](https://i.postimg.cc/QtGBFwTs/image.png)](https://postimg.cc/kVsMZjsh)

Al ser algo muy utilizado y el ya haberse realizado varios cálculos de las mismas podemos ver qué se estandarizó una tabla de transformadas ya que si las funciones son una combinación o una composición de varias funciones calcular la integrada No es tan complejo con respecto a unas ciertas modificaciones según el resultado de la ecuación la tabla es la siguiente

[![image.png](https://i.postimg.cc/1tG8wBGF/image.png)](https://postimg.cc/sQ2fRp0f)

## Transformada inversa de Laplace 
Hallando  la transformada inversa de laplace tenemos que damos solución a los sistemas dinámicos o a los modelamientos correspondientes según el ejercicio por lo general la solución de esta se hace realizando una expansión en fracciones parciales para obtener una suma de funciones mucho más simple que se puedan encontrar en las tablas de la transformada para ello la descomposición de fracciones parciales consiste de varios casos
### Caso 1 - Raíces reales distintas
veremos que su expresión general es la siguiente

$$G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s + p_1)(s + p_2) \dots (s + p_n)} $$

Teniendo que la descomposición en fracciones parciales es la siguiente ya que es un denominador el cual no se puede descomponer ni tiene grados correspondientes podremos hacerlo de la siguiente manera

 $$G(s) = \frac{A}{(s + p_1)} + \frac{B}{(s + p_2)} + \dots + \frac{N}{(s + p_n)}$$

Dónde A, B …. N son coeficientes por determinar
### Caso 2 - Raíces reales repetidas
En este caso veremos cómo cambia un poquito la ecuación general del sistema pues su denominador a pesar de ser simple y no poderse descomponer está elevado a un número

$$G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s + p)^n}$$

Su descomposición en fracciones parciales es la siguiente pues al tener un exponente se divide el mismo denominador, pero cada una con un grado independiente, así como se ve a continuación

$$G(s) = \frac{A}{(s + p)} + \frac{B}{(s + p)^2} + \dots + \frac{N}{(s + p)^n}$$
### Caso 3 - Raíces complejas conjugadas
Este tipo de fracciones parciales es un poquito más complejas pues se alarga un poco el procedimiento y su descomposición en fracciones parciales también es mayor pues se aumenta el número de coeficientes por determinar como podemos ver en la imagen dependemos mucho del denominador pues ya que si no se puede descomponer debemos trabajar con sus raíces complejas

$$G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s^2 + b_1s + c_1)(s^2 + b_2s + c_2) \dots (s^2 + b_n s + c_n)}$$

La descomposición en fracciones parciales es de la forma como podemos ver en este caso el número de coeficientes por determinar es mayor pues dependemos de 2 numeradores por cada fracción

$$G(s) = \frac{A s + B}{s^2 + b_1s + c_1} + \frac{C s + D}{s^2 + b_2s + c_2} + \dots + \frac{M s + N}{s^2 + b_n s + c_n}$$

# Transformada inversa de Laplace método resumido
Este método nos resulta más como ya que podemos aprovechar que para la descomposición en fracciones parciales se deben factorizar las raíces del polinomio del numerador esto nos ayuda a que se pueda saber los valores de ese que se van a eliminar en algunos términos, ayuda a reducir el sistema de ecuaciones para una mejor solución y un ahorro de tiempo a la hora de ejercicios largos los casos son los mismos 3 casos presentados anteriormente cada uno con una diferencia
## Caso 1 – Raíces reales diferente 
$$F(s) = \frac{A(s)}{B(s)} = \frac{a_1}{s + p_1} + \frac{a_2}{s + p_2} + \dots + \frac{a_n}{s + p_n}$$

Gracias a este método y sabiendo que $ a_{k}$ son constantes entonces $ a_{k}$ puede hallarse multiplicando a ambos lados de la igualdad por el denominador de la función en este caso $ (s+p_{k})$ y debemos también garantizar que se eliminen ciertos parámetros para ello haremos qué $ s=-p_{k}$ con esto obtendremos el resultado de las constantes necesarias para la solución del sistema

$$\left[ (s + p_k) \frac{A(s)}{B(s)} \right]{s = -p_k} = \left[ \frac{a_1}{s + p_1} (s + p_k) + \frac{a_2}{s + p_2} (s + p_k) + \dots + \frac{a_k}{s + p_k} (s + p_k) + \dots + \frac{a_n}{s + p_n} (s + p_k) \right]$$

$$a_k = \left[ (s + p_k) \frac{A(s)}{B(s)} \right]_{s = -p_k}$$
## Ejemplo 
El siguiente ejemplo explica lo anteriormente mencionado en este caso nos piden la inversa de 

$$F(s) = \frac{s+3}{(s+1)(s+2)}$$

[![Imagen-de-Whats-App-2025-03-10-a-las-15-04-08-1dc80d8b.jpg](https://i.postimg.cc/nrP8SbZQ/Imagen-de-Whats-App-2025-03-10-a-las-15-04-08-1dc80d8b.jpg)](https://postimg.cc/5QLkjrXx)

## Caso 2 – Raíces reales iguales 
Cómo se había explicado anteriormente para la solución de ecuaciones usando el método de fracciones parciales en este caso veremos que el denominador es una ecuación que está elevado a un número, para hallar la solución utilizando el método resumido es prácticamente igual al del caso uno con el método reducido simplemente es tener en cuenta el exponente y acomodarlo de la siguiente forma

$$F(s) = \frac{s^2 + 2s + 3}{(s+1)^3}$$

$$F(s) = \frac{A(s)}{B(s)} = \frac{b_3}{(s+1)^3} + \frac{b_2}{(s+1)^2} + \frac{b_1}{s+1}$$

$$(s+1)^3 \frac{A(s)}{B(s)} = b_3 + b_2(s+1) + b_1(s+1)^2$$

Tomando $s=-1$ garantizaremos que se eliminen ciertas constantes para así poder hallar los coeficientes necesarios para la solución entonces el término se deriva y evalúa sobre $s=-1$ la cantidad de derivadas se irá según el Exponente a mayor sea el número del exponente asimismo la cantidad de derivadas

$$\frac{d}{ds} \left[ (s+1)^3 \frac{A(s)}{B(s)} \right] = b_2 + 2b_1 (s+1)$$

$$\frac{d}{ds} \left[ (s+1)^3 \frac{A(s)}{B(s)} \right] \Big|_{s=-1} = b_2$$

$$\frac{d^2}{ds^2} \left[ (s+1)^3 \frac{A(s)}{B(s)} \right] = 2b_1$$

Una vez teniéndo lo anterior mencionado podremos seguir derivando para así tener los términos de $b_{1}$,$b_{2}$ y $b_{3}$ que necesitamos teniendo lo siguiente 

$$ b_1 = \frac{1}{2!} \left[ \frac{d^2}{ds^2} \left( (s+1)^3 \frac{A(s)}{B(s)} \right) \right]_{s=-1} $$
 
$$ = \frac{1}{2!} \left[ \frac{d^2}{ds^2} (s^2 + 2s + 3) \right]_{s=-1} $$

$$ = \frac{1}{2} (2) = 1 $$

Y así mismo ya se nos facilitan los cálculos tanto para $b_{2}$ y $b_{3}$ teniendo lo siguiente

### Cálculo para $b_{3}$
$$ b_3 = \left[ (s+1)^3 \frac{A(s)}{B(s)} \right]_{s=-1} $$

$$ = \left( s^2 + 2s + 3 \right)_{s=-1} $$

$$ = 2 $$

### Cálculo para $b_{2}$

$$ b_2 = \frac{d}{ds} \left[ (s+1)^3 \frac{A(s)}{B(s)} \right] \bigg|_{s=-1} $$

$$ = \left[ \frac{d}{ds} (s^2 + 2s + 3) \right]_{s=-1} $$

$$ = \left( 2s + 2 \right)_{s=-1} $$

$$ = 0 $$

Teniendo así que la respuesta del sistema al hallar los coeficientes y el realizar la transformada inversa de la plaza nos da como resultado la siguiente ecuación

$$ f(t) = \mathcal{L}^{-1} [F(s)] $$

$$ = \mathcal{L}^{-1} \left[ \frac{2}{(s+1)^3} \right] + \mathcal{L}^{-1} \left[ \frac{0}{(s+1)^2} \right] + \mathcal{L}^{-1} \left[ \frac{1}{s+1} \right] $$

$$ = t^2 e^{-t} + 0 + e^{-t} $$

$$ = (t^2 + 1)e^{-t}, \quad (t \geq 0) $$

## Caso 3 – Raíces complejas conjugadas 
Para el caso 3 la parte de solución de fracciones raíces por métodos resumidos Veremos que forma prácticamente de la misma manera más sin embargo pues las raíces son complejas eso quiere decir que nos regala en su determinante un número imaginario como se puede ver en el siguiente ejemplo

$$ F(s) = \frac{2s + 12}{s^2 + 2s + 5} $$

$$ s^2 + 2s + 5 = (s + 1 + j2)(s + 1 - j2) $$

sabiendo que este tipo de raíces resulta en una suma de una función seno amortiguada con coseno amortiguado esto lo podemos encontrar fácilmente en la tabla de la plaza para ello siempre debemos sumar y restar para poder así acomodar las ecuaciones

$$\mathcal{L}[e^{-\alpha t} \sin \omega t] = \frac{\omega}{(s + \alpha)^2 + \omega^2}$$

$$\mathcal{L}[e^{-\alpha t} \cos \omega t] = \frac{s + \alpha}{(s + \alpha)^2 + \omega^2}$$

A continuación se verá un ejemplo de cómo se puede solucionar y cómo se pueden completar los cuadrados en este caso sumamos y restamos el número cuatro esto con el fin de acomodar el denominador y que así pueda ser consecuente con la tabla de las transformadas inversas de la plaza

$$F(s) = \frac{2s + 12}{s^2 + 2s + 5} = \frac{2s + 12}{s^2 + 2s + 5 - 4 + 4}$$

$$F(s) = \frac{2s + 12}{(s + 1)^2 + 2^2}$$

$$F(s) = \frac{10 + 2(s + 1)}{(s + 1)^2 + 2^2} = \frac{5}{(s + 1)^2 + 2^2} + \frac{2}{(s + 1)^2 + 2^2} (s + 1)$$

$$F(t) = \mathcal{L}^{-1} [F(s)]$$

$$= 5\mathcal{L}^{-1} \left[ \frac{2}{(s+1)^2 + 2^2} \right]+ 2\mathcal{L}^{-1} \left[ \frac{s+1}{(s+1)^2 + 2^2} \right]$$

$$= 5e^{-t} \sin 2t + 2e^{-t} \cos 2t \quad (t \geq 0)$$

## Fracciones parciales en Matlab 
Una de las maneras más fáciles y certeras de garantizar una buena respuesta a la hora de resolver los ejercicios es comprobándolas en la plataforma de m Matlab ya que ella puede calcular los términos de las fracciones parciales conociendo los polinomios del denominador y el numerador de las funciones en el dominio de s, esto lo lograremos por medio de códigos es un código estructurado el cual se realizará para la solución de los ejercicios y para que me Matlab lo entienda

[![image.png](https://i.postimg.cc/VvzjY4T4/image.png)](https://postimg.cc/r0YdjGqt)

[![image.png](https://i.postimg.cc/XJkCDdJ5/image.png)](https://postimg.cc/zb3vyLTD)

Definiremos unas variables teniendo en cuenta que la función es la siguiente y as queda con sus coeficientes 

$$F(s) = \frac{s^2 - s - 3}{s(s-1)(s+3)} = \frac{0.75}{s-3} - \frac{0.75}{s+1} + \frac{1}{s}$$

Gracias a esta aplicación también podremos realizar la transformada inversa de la plaza o la transformada normal en este caso tenemos la transformada y la queremos pasar al dominio de ese para ello haríamos lo siguiente, la ecuación es la siguiente 

$$8\sin(4t) - 5\cos(4t)$$
Una vez teniendo la ecuación que queremos el desarrollo para hacerlo en Matlab nos quedaría así

[![image.png](https://i.postimg.cc/ydDFWkY3/image.png)](https://postimg.cc/DJKWMfG7)

Con esto podemos verificar y dar valores a la respuesta teniendo 

$$\mathcal{L} \{ 8\sin(4t) - 5\cos(4t) \} = \frac{32}{s^2 + 16} - \frac{5s}{s^2 + 16}$$

Algo muy parecido es a la hora de realizar la transformada inversa de laplace para ello debemos formular una ecuación y realizar unos pasos muy parecidos a los anteriores para en este caso darle una solución, la ecuación es la siguiente

$$Y(s) = \frac{6s - 4}{s^2 + 4s + 20}$$

una vez con la ecuación pasaremos a hacer el paso a paso en Matlab

[![image.png](https://i.postimg.cc/NFYfSzVG/image.png)](https://postimg.cc/ZB7SyV4X)

una vez hecho los pasos en Matlab veremos las respuestas y podremos entonces dar solución teniendo que

$$\mathcal{L}^{-1} \{ \frac{6s - 4}{s^2 + 4s + 20} \} = 6e^{-2t} \cos(4t) - 4e^{-2t} sen(4t)$$

# Solucion de ecuaciones diferenciales 
## Metodologia de solucion 
Se representa de una manera diferente a lo ya visto anterior mente pero es mas que todo solo la representacion de la ecuacion, se debe aplicar transformada de Laplace a toda la ecuacion parte por parte de tal manera que se tenga una ecuacion en terminos de la variable $s$, al despejar la variable tendremos como resultado una ecuacion que representa la salida en terminos de $X(s)$ una ves con esto en necesario aplicar transformada inversa de Laplace para optener la solucion en el dominio del tiempo
### Ejemplo 
$$\dot{x} + 3\dot{x} + 2x = 0, \quad x(0) = a, \quad \dot{x}(0) = b$$

Aplicaremos Laplace ala ecuacion teniendo lo siguiente 

$$[s^2X(s) - s x(0) - \dot{x}(0)] + 3[sX(s) - x(0)] + 2X(s) = 0$$

Una vez con esto podremos remplazar las condiciones iniciales para asi poder despejar x

$$[s^2X(s) - as - b] + 3[sX(s) - a] + 2X(s) = 0$$

Despejando x tendriamos que 

$$(s^2 + 3s + 2)X(s) = as + b + 3a$$

$$X(s) = \frac{as + b + 3a}{s^2 + 3s + 2} = \frac{as + b + 3a}{(s+1)(s+2)} = \frac{2a + b}{s+1} - \frac{a + b}{s+2}$$

Con este despeje podremos buscar en las tablas Laplace la solucion mas adecuada 

$$x(t) = \mathcal{L}^{-1}[X(s)] = \mathcal{L}^{-1} \left[ \frac{2a + b}{s+1} \right] - \mathcal{L}^{-1} \left[ \frac{a + b}{s+2} \right]$$

$$= (2a + b)e^{-t} - (a + b)e^{-2t} \quad (t \geq 0)$$

### Ejercicios 
### 1)
$$\dot{x} + 4x = 0, \quad x(0) = 5, \quad \dot{x}(0) = 0$$

Para la solución del ejercicio es necesario pasar la ecuación a Laplace para facilitar el desarrollo de los cálculos quedando así de la siguiente forma.

$$[s^2X(s) - s x(0) - \dot{x}(0)] + 4X(s) = 0$$

Una vez pasada la ecuación en forma de la plaza pasaremos a reemplazar las condiciones iniciales

$$s^2X(s) - 5s - 0 + 4X(s) = 0$$

Distribuyendo mejor los parámetros de la ecuación y teniendo en un lado términos de
$X(s)$ y al otro lado términos de 𝑠 tendremos.

$$s^2X(s) + 4X(s) = 5s$$

Agrupando términos semejantes y despejando $X(s)$ tendríamos

$$X(s)(s^2 + 4) = 5s$$

Acto seguido debemos despejar $X(s)$

$$X(s) = \frac{5s}{s^2 + 4}$$

Al tener esta expresión nos damos cuenta de que se puede hacer la transformada inversa directamente ya que vemos es muy parecida a una de las transformadas de la tabla de Laplace simplemente pasaremos el 5 que es una constante fuera de la transformada quedando de la siguiente manera

$$5 \mathcal{L}^{-1} \{ \frac{s}{s^2 + 4} \}$$

Teniendo esto podremos dar solución al ejercicio según la tabla nos quedaría de la siguiente forma

$$x(t) = 5 \cos(2t)$$
