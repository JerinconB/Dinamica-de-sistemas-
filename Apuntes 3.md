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

