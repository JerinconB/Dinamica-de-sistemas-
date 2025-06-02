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

## Clasificacion de las funciones de transferencia --- 14/05/2025
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


