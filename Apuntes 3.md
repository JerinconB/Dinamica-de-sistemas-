# Apuntes dinamica de sistemas 3 corte 
### Rincon Benavides Juan Esteban 
## Correccion Segundo parcial---7/05/2025
## Punto 1
Obtener las ecuaciones diferenciales del siguiente sistema. Suponga que no hay fricción entre las ruedas y las respectivas superficies y que el carro que lleva la masa m no tiene masa. (Solo se acepta procedimiento completo visto en clase). Sabiendo que “u” es una fuerza y que “y” y “x” son distancias.

[![image.png](https://i.postimg.cc/28TjWsQg/image.png)](https://postimg.cc/tYZHQmmz)

Para la solucion del primer punto deberemos analizar cada elemento con su respectivo diagrama de bloques esto para analizar las fuerzas que se aplican a cada elemento, emepesaremos por el diagrama de cuerpo libre de la masa y luego la del carrito 

### DCL-- Masa

[![image.png](https://i.postimg.cc/hjG1fv9p/image.png)](https://postimg.cc/p9gFS2cF)

Como podemos ver en el diagrama ambas fuerzas van hacia la masa por ende el analicis de la sumatoria de fuerzas nos quedara de la sigiente manera.

$$F_k + F_b = m \cdot \frac{d^2 y}{dt^2}$$

$$k(y - x) + b\left( \frac{dy}{dt} - \frac{dx}{dt} \right) = m \cdot \frac{d^2 y}{dt^2}$$

### DCL-- Carrito

[![image.png](https://i.postimg.cc/Z5vcd4y1/image.png)](https://postimg.cc/pmxzNNCZ)

En este caso para la solucion veremos que tendremos tres fuerzas que se aplican al carrito, y sabiendo que su aceleracion se va atomar como 0 tendremos que la sumatoria de fuerzas queda de la siguiente manera.

$$U - F_K - F_B = 0$$

$$U - K(y - x) - B(\dot{y} - \dot{x}) = 0$$
## Punto 2
Para el circuito de la figura hallar la/s ecuaciones diferenciales que permiten obtener la función que describe la corriente en el capacitor de 0.2 F. Seleccione el método de análisis que prefiera o considere más adecuado. Asuma que el circuito está totalmente sin energía en t = 0 y que la fuente de voltaje e(t) es constante. 

[![image.png](https://i.postimg.cc/kX6zhZTp/image.png)](https://postimg.cc/2VY01HRQ)

Para la solucion del ejercicio lo desarrolaremos por mallas ya que nos queda mas facil ver cada ecuacion en este caso desarrolaremos primero la malla 1 que sera la de la izquierda teniendo como consecuente lo sigiente 

$$-e(t) + V_H + V_{200} + V_{50} = 0$$

$$-e(t) + 2\frac{dI_1}{dt} + 200I_1 + 50(I_1 - I_2) = 0$$

y para terminar el ejercicio para tener ambas ecuacuaciones en funcion de la corriente del capacitor tendremos el sigiente analizis para la malla 2 

$$V_{50} + V_{20} + V_C = 0$$

$$50(I_2 - I_1) + 20I_2 + \frac{1}{0.2} \int I_2\, dt = 0$$

# Clasificacion de las funciones de transferencia --- 14/05/2025
### Fucnion de transferencia 
Una función de transferencia es una herramienta matemática que se utiliza en ingeniería y control de sistemas para describir la relación entre la entrada y la salida de un sistema dinámico lineal, en el dominio de Laplace.

$$G(s) = \frac{Y(s)}{U(s)}$$

La función de transferencia representa cómo un sistema responde a una entrada en términos de sus componentes dinámicos (como integradores, derivadores, y constantes de ganancia). Incluye el comportamiento transitorio y en estado estacionario.

### Clasificaciones 
Las funciones de transferencia se pueden expresar de diferentes maneras, esto dependera de su denominador y numerador, teniendo tres casos particulares los cuales son 

[![image.png](https://i.postimg.cc/CKXqw3Jn/image.png)](https://postimg.cc/GBP2QSWb)

Teniendo esto en cuenta podremos analizar varios ejemplos como los sigientes 

$$ s^2 + 1 \quad \text{(impropia)} $$
$$ 2 \quad \text{(bipropia)} $$
$$\frac{1}{s + 1} \quad \text{(Estrictamente propia)}$$
$$\frac{s^2 - 1}{s + 1} \quad \text{(impropia)}$$
$$\frac{s - 1}{s + 1} \quad \text{(bipropia)}$$

## Zeros en una funcion de transferencia 
Para la solucion de los zeros debemos igualar el numerador a 0 para obter los valores de (S), si de casualidad el numerador se hace 0 toda la funcion de transferencia se vuelve 0 de ahi el nombre, la solucion de (S) pueden ser numeros reales o complejos esto con el fin de ubicarlos en el plano cartesiano 

$$G(s) = \frac{Y(s)}{U(s)} = \frac{3s-1}{s^2+3s+2} = \frac{N(s)}{D(s)}$$

$$N(s) = 0 \quad \Rightarrow \quad 3s-1=0$$

Como solucion nos da un numero complejo el cual es el sigiente 

$$ s = \frac{1}{3} $$

Una vez hallado el resultado este deberemos graficarlo en el plano cartesiano, este se representara con un circulo de la sigiente forma 

[![image.png](https://i.postimg.cc/jjbjvR8X/image.png)](https://postimg.cc/YvdkCBBG)

## Polos en una funcion de transferencia
En el caso de los polos lo que deberemos hacer es igualar a cero el denomidador de la funcion de transferencia para hallar "S" estos valores tambien puden ser reales o complejos esto con la facilidad de poderlos graficar en el plano cartesiano

### ¿Por qué son importantes los polos?
Los polos determinan el comportamiento dinámico del sistema:

-Si los polos están en el semiplano izquierdo del plano complejo (tienen parte real negativa), el sistema es estable.

-Si uno o más polos están en el semiplano derecho (parte real positiva), el sistema es inestable.

-Si hay polos en el eje imaginario (parte real cero), el sistema puede ser marginalmente estable o inestable, dependiendo del caso.

### Ejemplo

$$G(s) = \frac{Y(s)}{U(s)} = \frac{3s - 1}{s^2 + 3s + 2} = \frac{N(s)}{D(s)}$$

$$D(s) = 0$$

$$s^2 + 3s + 2 = 0$$

$$(s + 1)(s + 2) = 0$$

$$s = -1$$

$$s = -2$$

La ubuicacion de los polos es muy similar ala de los zeros, solo que en este caso tendremos que demarcarlos con una X en el plano carteciano esto lo podremos ver en la sigiente imagen 

[![image.png](https://i.postimg.cc/BvGtxqDQ/image.png)](https://postimg.cc/LJNHSFNr)

## Ubicacion General de los polos 
[![image.png](https://i.postimg.cc/jSXNBvwH/image.png)](https://postimg.cc/4YYm961y)

### Polos complejos conjugados
Representados como un par de “X” simétricas respecto al eje real.

Tienen la forma:

$$s = \sigma \pm j\omega$$

donde:

𝜎 es la parte real (negativa en sistemas estables).

𝜔 es la frecuencia imaginaria.

Característica: generan una respuesta oscilatoria amortiguada.

### Polos reales diferentes
Ubicados sobre el eje real (horizontal), pero en posiciones distintas.

Tienen la forma:

$$s = s_1, \quad s = s_2 \quad \text{con} \quad s_1 \ne s_2, \quad s_1, s_2 \in \mathbb{R}$$

Característica: producen una respuesta compuesta por dos exponentes reales negativos (si el sistema es estable).

### Polos reales iguales (repetidos)
Ubicados sobre el eje real en el mismo punto.

Tienen la forma:

$$s = s_0 \quad \text{con multiplicidad} > 1$$

Característica: generan una respuesta del tipo $t^n e^{s_0 t}$ , más lenta que polos reales simples.

## Teorema del valor final 
El Teorema del Valor Final es una herramienta en el análisis de sistemas dinámicos (especialmente en el dominio de Laplace) que permite encontrar el valor al que tiende una función en el tiempo cuando t→∞, usando su transformada de Laplace.

$$\lim_{t \to \infty} f(t) = \lim_{s \to 0} s F(s)$$

### Ejemplo 

$$G(s) = \frac{Y(s)}{U(s)} = \frac{4}{5s + 1}$$

$$Y(s) = \frac{4 \ast U(s)}{5s + 1}$$

Si la entrada es un escalón:

$$Y(s) = \frac{\frac{4}{s}}{5s + 1}$$

Teorema del valor final:

$$\lim_{s \to 0} sY(s) = \lim_{s \to 0} s \cdot \frac{\frac{4}{s}}{5s + 1}$$

$$\lim_{s \to 0} \frac{4}{5s+1} = 4$$

## Entradas de prueba de un sistema 
En este caso la solución de una ecuación diferencial depende de la entrada, la respuesta de un sistema también.

Es muy difícil conocer las señales que están ocurriendo en un sistema, ya que depende de muchos factores como ruido, tipo de señales, ambiente, entre otros, además, el sistema de control debe diseñarse para que funcione ante cualquier señal.

En control, se utilizan diferentes tipos de señales de prueba para evaluar el desempeño de un sistema.

### Entrada escalon 
Un cambio abrupto en la entrada desde cero a un valor constante A en t=0, Evalúa la respuesta transitoria y el error en estado estacionario de un sistema (ej: tiempo de asentamiento, sobrepico).

Expresión matemática:

$$\mathcal{L}(u(t)) = \frac{A}{s}$$

### Entrada Rampa 
Una señal que aumenta linealmente con el tiempo, Analiza la capacidad del sistema para seguir señales que cambian continuamente (ej: sistemas de seguimiento como radares o motores).

Expresión matemática:

$$\mathcal{L}\{x(t)\} = \frac{A}{s^2}$$

### Entrada Parabola
Una señal que varía cuadráticamente con el tiempo, Estudia sistemas que requieren alta precisión para aceleraciones (ej: cohetes, satélites).

Expresión matemática:

$$\mathcal{L}\{r(t)\} = \frac{A}{s^3}$$

# Modelamiento de sistemas complejos --- 21/05/2025
Podemos modelar sistemas si los representamos como un todo hallando las funciones de transferencia de cada uno de los componentes del sistema analizado, por otra parte seria utilizar modelos que ya estan desarrollados para poder construir modelos mas complejos, mas sin embargo aparte de estos dos sistemas de modelamiento hay muchos tipos mas de modelamiento para los diferentes dispositivos 

## Soleniode 
Un solenoide es un dispositivo electromecánico que convierte energía eléctrica en movimiento mecánico lineal mediante un campo electromagnético. 

[![image.png](https://i.postimg.cc/1zQ3pN9f/image.png)](https://postimg.cc/k2TCCGRm)

$$ L \frac{di}{dt} + R \, i = \nu(t) \quad \text{y} \quad I(s) = V(s) \frac{1}{L \, s + R} $$

El electroiman produce una fuerza mecanica proporcional a la corriente en el embobonado teniendo las sigientes ecuaciones 

$$ f_{, \bar s} = K_{, \bar s}i \quad \text{y} \quad F_{, \bar s}(s) = K_{, \bar s}\,I(s) $$

El electroiman atrae una masa acopladapor medio de un resorte y se considera el amortiguamiento dada por la bobina 

$$m\frac{d^{\,2}\,x}{dt^{\,2}} + b\,\frac{dx}{dt} + k\,x = f(t)$$

$$X(s) = \frac{F(s)}{m\,s^{\,2} + b\,s + k}$$

Con esto ya tendriamos para poder representarlo en un diagrama de bloques posicionando cada uno de ellos y organizandolo para que nos quede reducido, para este caso seria el sigiente diagrama 

[![image.png](https://i.postimg.cc/sg6JxS5C/image.png)](https://postimg.cc/HrMMPrS6)

## Motor DC
En la mayoria de los libros lo representan de esta monera tal y como sale en la imgagen donde popdemos ver la parte movil y su parte estatica teniendo en el medio la transformacion de energia electrica en mecanica 

[![image.png](https://i.postimg.cc/nLPL5VBJ/image.png)](https://postimg.cc/2qnmLD0c)

Estos moteores DC tienen dos formas de modelamiento una de ellas es por corriente de campo y la otra por corriente de armadura.

## Corriente de campo 
como podemos ver en la imagen anterior cada una tiene su nomenclatura diferente teniendo que la sub c es corriente de campo osea la misma corriente del rotor, y para poder ayudarnos alas ecuaciones del modelamiento asumiremos que la corriente de armadura va hacer constante teniendo lo siguiente 

$$ V_{C}(t) = V_{Rc} + V_{Lc} $$

$$ L_C\frac{di_C}{dt} + R_C i_C = \nu_C(t) $$

$$ I_C(s) = \frac{V_C(s)}{s L_C + R_C} $$

Al tener este tipo de modelamiento veremos que aparece una asignacion la cual es el flujo en el entrehierrro el cual va hacer proporcional ala corriente de campo teniendo que:

$$\Phi = K_c i_c$$

Con esto podremos comenzar a analizar el torque proporcionado por el motor 

$$T_m = K_a i_a(t) K_c i_c(t)$$

$$T_m(s) = (K_a K_c I_a) I_c(s) = K_m I_c(s)$$

El torque aplicado a la carga que queramos levantar es el desarrollado por el motor menos la inercia de la carga 

$$T_c(s) = T_m(s) - T_p(s)$$

En el caso de la parte mecanica del motor DC esta se comporta como un sistema rotacional clasico que considera la inercia y la friccion mecanica teniendo lo siguiente 

$$ J \frac{d^2 \theta}{dt^2} + b \frac{d\theta}{dt} + k \theta = \tau(t) $$

$$ \Theta(s) = T_c(s) \frac{1}{s^2 J + b s} $$

La coneccion de los modelos obtenidos de cada uno de los pasos se realizara de la sigiente manera 

$$\Theta(s) = V_c(s) \frac{K_m}{(sL_c + R_c)(Js^2 + bs)} - T_p(s) \frac{1}{(Js^2 + bs)}$$

$$\frac{\Theta(s)}{V_c(s)} = \frac{K_m}{(sL_c + R_c)(Js^2 + bs)}$$

y su respectivo diagrama de bloques quedaria asi 

![image](https://github.com/user-attachments/assets/5045fb1c-5f04-45b7-932e-39429fbaae0b)

## Corriente de armadura 
Para el analizis de un motor DC por corriente de armadura en este caso tendremos en cuenta pasos del de corriente de campo mas sin embargo lo que aremos en esta ocacion para la facicilidad de los calculos es asumir en este caso la corriente de campo constante teniendo que:

$$T_m(s) = (K_a K_c I_c) I_a(s) = K_m I_a(s)$$

Con esto vemos que la corriente de armadura se relaciona con el voltaje aplicado la armadura por 

$$V_a(s) = (sL_a + R_a) I_a(s) + V_b(s)$$

El voltaje inducido por la armadura es proporcinal a la velocidad angular del eje y sabiendo que $V_b$ es

$$V_b(s) = K_b \omega(s)$$

Tendremos que: 

$$V_a(s) = (sL_a + R_a) I_a(s) + V_b(s)$$

Combinando estas ecuaciones se obtiene lo sigiente que es la corriente en la armadura 

$$I_a(s) = \frac{V_a(s) - K_b \omega(s)}{sL_a + R_a}$$

Para la parte mecanica vemos que en este caso se comporta de la misma manera que para el modelamiento anterio un sistema rotacional simple y ya sabiendo lo anterior supondremos que:

$$ T_{C}(s) = T_{m}(s) - T_{p}(s) $$

$$ \Theta(s) = T_{C}(s) \frac{1}{J s^2 + b s} $$

Teniendo como resultado el sigiente diagrama de bloques 

[![image.png](https://i.postimg.cc/gJWHr6YY/image.png)](https://postimg.cc/1gvqjXnT)

## Elementos transmisores de energia 
### Engranajes y poleas 
Los engranajes son mecanismos compuestos por ruedas dentadas que transmiten movimiento rotacional y par mecánico entre ejes, modificando la velocidad, torque o dirección del movimiento, y las poleas son sistemas que transmiten movimiento y fuerza mediante correas o cables que recorren una rueda acanalada, ideal para ejes separados.

[![image.png](https://i.postimg.cc/J423ZF1Y/image.png)](https://postimg.cc/ppKntq5K)

$$ \frac{\tau_2}{\tau_1} = \frac{N_2}{N_1} $$

$$ \frac{N_2}{N_1} = -\frac{\theta_1}{\theta_2} $$

J y Km cambian si se tiene en cuenta el efecto de los engranajes o poleas 

$$ \Theta(s) = \frac{K_m V_c(s)}{(s L_c + R_c)(J s^2 + b s)} - \frac{T_p(s)}{J s^2 + b s} $$

$$ \frac{\Theta(s)}{V_c(s)} = \frac{K_m}{(s L_c + R_c)(J s^2 + b s)} $$

y sus diagramas de bloques son los siguientes 

[![image.png](https://i.postimg.cc/8kH3LTfp/image.png)](https://postimg.cc/rzDQkX93)

## Transmicion rotacional a lineal 
Sistemas que convierten movimiento de rotación (angular) en movimiento lineal (traslacional), fundamentales en aplicaciones mecánicas y de control.

Piñón-Cremallera

Ecuación:

$$x=rθ$$

x: Desplazamiento lineal [m]

r: Radio del piñón [m]

θ: Ángulo rotado [rad]

[![image.png](https://i.postimg.cc/Z5VrJKRQ/image.png)](https://postimg.cc/dhZ7BFGR)

## Palancas
Una palanca como sistema dinámico es un sistema mecánico que transforma una entrada (una fuerza o par aplicado en un punto) en una salida (desplazamiento, velocidad o fuerza en otro punto), a través de la interacción de masas, inercias y torques. Este sistema puede modelarse usando las leyes de la dinámica rotacional.

[![image.png](https://i.postimg.cc/15KFK5pz/image.png)](https://postimg.cc/ykkW1Kpq)

$$-\frac{f_{2}}{f_{1}} = \frac{d_{1}}{d_{2}}$$

$$\frac{d_{1}}{d_{2}} = -\frac{x_{1}}{x_{2}}$$

# Algebra de bloques --- 28/05/2025
El álgebra de bloques es una técnica gráfica y analítica utilizada en ingeniería de control y sistemas dinámicos para representar, simplificar y analizar diagramas de bloques interconectados. Permite reducir sistemas complejos a una función de transferencia equivalente mediante reglas algebraicas.

### Elementos de un diagrama de bloques 
Bloque funcional: es un simbolo para representar la operacion matematica aplicada ala señal de entrada esto con el fin de ver la salida optenida despues de la operacion su simbolo en el diagrama es el siguiente 

[![image.png](https://i.postimg.cc/vHYxqw8H/image.png)](https://postimg.cc/23t5yJBP)

### Flechas
Estas son muy importantes ya que representan las señales dentro del proceso esta solo puede pasar por una direccion, es de total importancia asegurarse en que sentido va la flecha y hacia que bloque se dirique a si sabremos la dispocicion del diagrama 

### Punto suma 
Este bloque es el encargado de hacernos operaciones especificamente una suma o una resta entre señales unicamente, NO bloques, depende de donde este ubicada la señal y el signo deberemos realizar una operacion o la otra, es importante que las cantidades que se sumen o resten tengan las mismas dimenciones y las mismas unidades.

[![image.png](https://i.postimg.cc/zXHY1VGd/image.png)](https://postimg.cc/MvwF7ZRR)

### Ramificacion 
Es un punto donde la señal de un bloque va de modo concurrente a otros bloques o puntos de suma este punto hace que se repita la señal para diferentes calculos 

[![image.png](https://i.postimg.cc/4d2qDgkk/image.png)](https://postimg.cc/qhn1KWvj)

## Interpretacion del diaagrama 
Para los bloques los veremos como una multiplicacion de su entrada por la ecuacion o funcion que este dentro de el bloque acontinuacion una representacion grafica en donde veremos que la salida del sistema Y(s) en el producto de la entrada U(s) y la funcion del bloque G(s)

[![image.png](https://i.postimg.cc/8zyYJGcF/image.png)](https://postimg.cc/FYLp82jm)

$$ Y(s)=U(s)*G(s) $$

## Bloques en cascada 
Es cuando tenemos una combinacion de dos o mas bloques seguidos o en serie es ton el fin de operarlos y reducir el sistme a aun solo bloque 

[![image.png](https://i.postimg.cc/gjtDcVGn/image.png)](https://postimg.cc/jnNNZJwb)

$$Y_1(s) = U_1(s) G_1(s)$$

$$Y_2(s) = U_2(s) G_2(s)$$

Teniendo lo anterior veremos que la entrada del segundo bloque es la salida del primero por lo cual esta señal es la misma esto nos ayudara a simplificar y poder operar el resto teniendo en cuenta las entradas y las salidas analizadas del sistema 

$$Y_2(s) = Y_1(s) G_2(s)$$

$$Y_2(s) = U_1(s) G_1(s) G_2(s)$$

Con esto se reduce el sistema al siguiente diagrama de bloques 

![image](https://github.com/user-attachments/assets/d8545cce-8ca5-48b4-a021-57f6a552eb44)

Este es uno de los casos mas sencillos e intutibos mas sinembargo hay muchas combinaciones de estos diagramas de bloques para ello hay tablas comprobadas para la solucion de cierto bloques 

[![image.png](https://i.postimg.cc/VLSTr6p3/image.png)](https://postimg.cc/bshL4zzT)

## Lazo de realimentacion positivo

[![image.png](https://i.postimg.cc/7LQtZrXx/image.png)](https://postimg.cc/bGk9mMKM)

$$E(s) = X(s) + Y_1(s)$$

$$Y(s) = E(s) G_1(s)$$

$$Y_1(s) = Y(s) G_2(s)$$

$$Y(s) = (X(s) + Y_1(s)) G_1(s)$$

$$Y(s) = (X(s) + Y(s) G_2(s)) G_1(s)$$

$$Y(s) = (X(s) G_1(s) + Y(s) G_2(s) G_1(s))$$

$$Y(s) - Y(s) G_2(s) G_1(s) = X(s) G_1(s)$$

$$Y(s)(1 - G_2(s) G_1(s)) = X(s) G_1(s)$$

$$\frac{Y(s)}{X(s)} = \frac{G_1(s)}{1 - G_2(s) G_1(s)}$$

## Lazo de realimentacion negativo

[![image.png](https://i.postimg.cc/YSqgy469/image.png)](https://postimg.cc/pm4pmL1b)

$$E(s) = X(s) - Y(s) G_2(s)$$

$$Y(s) = E(s) G_1(s)$$

$$Y(s) = \left( X(s) - Y(s) G_2(s) \right) G_1(s)$$

$$Y(s) = X(s) G_1(s) - Y(s) G_2(s) G_1(s)$$

$$Y(s) + Y(s) G_2(s) G_1(s) = X(s) G_1(s)$$

$$Y(s) \left(1 + G_2(s) G_1(s)\right) = X(s) G_1(s)$$

$$\frac{Y(s)}{X(s)} = \frac{G_1(s)}{1 + G_2(s) G_1(s)}$$

## Reduccion de bloques 
Aqui veremos el comportamioento de la tabla mostrada anteriormente para la reduccion de un diagrama de bloques esto se hace con el fin de ver la salida sobre alguna entrada en espesifico en este ejemplo veremos un diagrama de bloque el cual tiene dos entradas y una salida y analizaremos esas dos posibles funciones 

[![image.png](https://i.postimg.cc/G3sDNnyk/image.png)](https://postimg.cc/4nsn7Mwd)

Para el caso poderemos simplificar la primera parte que es la reduccion de G1 y G2 obtenienmdo otro diagrama de bloques para operar, y operaremos la parte de abajo moviendo el punto suma para eliminarlo

[![image.png](https://i.postimg.cc/9XT4bP6b/image.png)](https://postimg.cc/kDJXXSXR)

En este caso vemos que nos quedan dos bloque en serie o segidos, estos los podremos operar como habiamos visto en un principio paara que nos vuelva a quedar un solo bloque

[![image.png](https://i.postimg.cc/0jqyF3Tf/image.png)](https://postimg.cc/ygvKSfYg)

Con esto se da fin al ejercicio obteniendo los dos posibles caminos para hallar las funciones de transferencia correspondientes a cada entrada las cuales son 

$$\frac{Y(s)}{X_1(s)} = G_3 \left( G_1 - G_2 \right)$$

$$\frac{Y(s)}{X_2(s)} = \left( G_4 - 1 \right)$$

# Diagrama de flujo de señales --- 4/6/2025
Este tipo de diagramas permite otra forma de representacion de los sistemas mas complejos para analizar las respuestas de los diagramas de bloques, con este podemos obtener mas sencillamente la funcion de transferencia total del sistema, gracias ala formula de mason que esta hecha para los sistemas mas complejos 

## Elementos de los diagramas de flujo de señal 
### Nodo
Estos representan las señales de entrada o salida del sistema, se representa por medio de un punto con el nombre de la señal puede ser en blanco o en negro 

[![image.png](https://i.postimg.cc/t4PpQDzv/image.png)](https://postimg.cc/Snywc63c)

### Flecha 
Representa la relación entre las variables del sistema

Se representa por medio de flechas que indicando el sentido de la relación

La fleche sale de la señal (Nodo) de entrada y llega a la señal de salida (Nodo)

Se agrega una etiqueta a la flecha para indicar la función de transferencia que relaciona la entrada y la salida

[![image.png](https://i.postimg.cc/zBGsBknr/image.png)](https://postimg.cc/1gbC7wCC)

## Interpretacion 

[![image.png](https://i.postimg.cc/vZwC9yWX/image.png)](https://postimg.cc/0bZtRLXJ)

vemos que cuando es directo se representa por medio de un producto entre lo que esta en la flecha por lo que entra a la flecha esto nos dara el valor de salida, y cuando varias flechas entran a un solo punto estas funciones se suman

## Comparacion entre diagrama de bloques y flujo de señales 
Como nos podemos dar cuenta manejan varias similitudees pues de un diagrama podemos interpretal el otro ya que tienen representados de diferente manera los mismos cuadros y conectores a continuacion una imagen en donde se ve relacionado lo dicho anterior 

[![image.png](https://i.postimg.cc/DyMFKTZG/image.png)](https://postimg.cc/Vdn2j2Xs)

Para el diagrama de flujo tendremos que tener en cuenta varias definiciones las cuales nos ayudaren al desarrollo de estos ejercicios los cuales son:

• Ganancia de lazo: La ganancia de lazo es el producto de las ganancias de ramas de un lazo.

• Trayecto o camino directo: Trayecto directo es el camino o trayecto de un nodo de entrada a un nodo de salida, sin cruzar ningún nodo más de una vez.

• Ganancia de trayecto directo: La ganancia de trayecto directo es el producto de las ganancias de rama de un camino o trayecto directo.

• Lazo: Un lazo es un camino o trayecto cerrado.

• Ganancia de lazo: La ganancia de lazo es el producto de las ganancias de ramas de un lazo.

## Formula de Mason 

$$P = \frac{1}{\Delta} \sum_k P_k \Delta_k$$

• $P_k$ Ganancia de los caminos directos

• Δ = 1 − (suma ganancias de los lazos) + (suma producto de 2 lazos que no se tocan) –(suma producto de 3 lazos que no se tocan)+…

• Δ𝑘 = 1 −(suma ganancias lazos que no toquen la trayectoria 𝑃𝑘)+(suma ganancias 2 lazos que no toquen la trayectoria 𝑃𝑘 y no se toquen entre sí)-(suma ganancias 3 lazos que no toquen la trayectoria 𝑃𝑘 y no se toquen entre sí)+…

## Ejemplo

[![image.png](https://i.postimg.cc/bN30y6ck/image.png)](https://postimg.cc/3d009Fwx)

### Trayectoria directa

$$P_1 = 1 \cdot 1 \cdot G_1 \cdot G_2 \cdot G_3 \cdot 1 = G_1 G_2 G_3$$

### Lazos Cerrados 

$$L_1 = G_1 G_2 H_1$$

$$L_2 = -G_2 G_3 H_2$$

$$L_3 = -G_1 G_2 G_3$$

### Determinante y cofactores

$$\Delta = 1 - (L_1 + L_2 + L_3)$$

$$\Delta_1 = 1$$

### Solucion 

$$\frac{C(s)}{R(s)} = \frac{P_1 \Delta_1}{\Delta} = \frac{G_1 G_2 G_3}{1 - G_1 G_2 H_1 + G_2 G_3 H_2 + G_1 G_2 G_3}$$

## Ejemplo 2

[![image.png](https://i.postimg.cc/0QsZMbtw/image.png)](https://postimg.cc/R3gw2VxS)

### Ganancias de trayectoria directa

$$P_1 = G_1 G_2 G_3 G_4 G_5$$

$$P_2 = G_1 G_6 G_4 G_5$$

$$P_3 = G_1 G_2 G_7$$

### Lazos Cerrados

$$L_1 = -G_4 H_1$$

$$L_2 = -G_2 G_7 H_2$$

$$L_3 = -G_6 G_4 G_5 H_2$$

$$L_4 = -G_2 G_3 G_4 G_5 H_2$$

### Determinante y cofactores

$$\Delta = 1 - (L_1 + L_2 + L_3 + L_4) + L_1 L_2$$

$$\Delta_1 = 1$$

$$\Delta_2 = 1$$

$$\Delta_3 = 1 - L_1$$

### Solucion

$$\frac{C(s)}{R(s)} = \frac{1}{\Delta} (P_1 \Delta_1 + P_2 \Delta_2 + P_3 \Delta_3)$$

% Expresión final expandida del resultado:

$$\frac{G_1 G_2 G_3 G_4 G_5 + G_1 G_6 G_4 G_5 + G_1 G_2 G_7 (1 + G_4 H_1)}{1 + G_4 H_1 + G_2 G_7 H_2 + G_6 G_4 G_5 H_2 + G_2 G_3 G_4 G_5 H_2 + G_4 H_1 G_2 G_7 H_2}$$

## Resumen 
• Los diagramas de flujo de señales facilitan la reducción de diagramas que representan sistemas complejos.

• La reducción de diagramas de bloques requiere experiencia en la aplicación de las propiedades para aplicarlas en sistemas con alta complejidad.

• Los diagramas de flujo de señales utilizan la fórmula de Mason para que sea más sistemática la reducción de los diagramas.

• Los circuitos con amplificadores operacionales permiten realizar pruebas de cualquier Sistema a partir de su modelo.
