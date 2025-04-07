# Apuntes Dinamica de Sistemas 2 Corte 
### Rincon Benavides Juan Esteban 
## Correccion primer parcial 
Para el primer punto del parcial nos presenta la siguiente ecuación la cual deberemos solucionar según las condiciones iniciales determinadas en este mismo 

$$2\ddot{x} + 2\dot{x} + x = 1$$

$$X(0) = 0, \quad \dot{X}(0) = 2$$

Una vez con esto pasaremos a la solución del primer punto del parcial teniendo en cuenta los temas vistos en el corte quedando de la siguiente forma

$$-s^2 X(s) + sX(0) - \dot{X}(0) + [sX(s) - X(0)] + X(s) = \frac{1}{2s}$$

$$-s^2 X(s) - 2 + sX(s) + X(s) = \frac{1}{2s}$$

$$X(s)(s^2 + s + \frac{1}{2}) = \frac{1}{2s} + 2$$

$$X(s) = \frac{4s + 1}{(s^2 + s + \frac{1}{2})2s}$$

$$\frac{4s + 1}{(s^2 + s + \frac{1}{2})2s} = \frac{A}{2s} + \frac{B s + C}{s^2 + s + \frac{1}{2}}$$

$$4s + 1 = A(s^2 + s + \frac{1}{2}) + (Bs + C)(2s)$$

$$4s + 1 = A s^2 + A s + \frac{A}{2} + 2 B s^2 + 2 C s$$

$$4s + 1 = (A + 2B)s^2 + (A + 2C)s + \frac{A}{2}$$

Una vez con esto podemos hallar las ecuaciones correspondientes con esto podremos encontrar los valores de A B Y C teniendo las siguientes ecuaciones

$$\frac{A}{2} = 1$$

$$A + 2C = 4$$

$$A + 2B = 0$$

Una vez con este sistema de ecuaciones pasaremos a resolver las incógnitas teniendo como resultado lo siguiente para A:

$$A = 2$$

Sustituyendo A en la tercera ecuacion tendremos que el resultado de B es:

$$A + 2B = 0$$

$$B = -1$$

Una vez con lo siguiente podremos reemplazar en la segunda ecuación A también para así poder hallar el resultado de C

$$A + 2C = 4$$

$$2 + 2C = 4$$

$$C = \frac{4 - 2}{2}$$

$$C = 1$$

Una vez teniendo esto podremos reemplazar los valores de A B y C en la ecuación de fracciones parciales esto para dar fin al ejercicio y poder hallar la transformada inversa del mismo

$$\frac{2}{2s} + \frac{-s + 1}{s^2 + s + \frac{1}{2}}$$

$$\mathcal{L}^{-1} \left( \frac{-s + 1}{s^2 + s + \frac{1}{2}} \right)$$

$$s^2 + s + \frac{1}{2} = \left(s + \frac{1}{2}\right)^2 + \frac{3}{4}$$

$$x(t) = 2 + e^{-\frac{1}{2}t} \left( \cos\left( \frac{\sqrt{3}}{2}t \right) - \sqrt{3} \sin\left( \frac{\sqrt{3}}{2}t \right) \right)$$












