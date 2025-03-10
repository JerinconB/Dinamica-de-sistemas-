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
$$\frac{d^2x(t)}{dt^2} + \frac{dx(t)}{dt} + x(t) + x^3(t) = \sen(\omega t)$$




